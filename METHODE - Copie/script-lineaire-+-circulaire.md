# Script linéaire + circulaire

Dans un [script normal](https://doc.frigost.dev/abonnement-frigost-bot/syntaxe-du-script), si une carte est définie plusieurs fois, le bot va toujours choisir la première ligne, par exemple :&#x20;

```lua
function move()
    return {
        { map = "6,-18", path = "left", fight = true },
        { map = "5,-18", path = "left" }, -- Première ligne pour 5,-18
        { map = "4,-18", path = "right", fight = true },
        { map = "5,-18", path = "right" }, -- Sera ignoré car y'a 5,-18 en haut
    }
end
```

Le genre de script qu'on va présenter est fait pour remédier à cette situation :

* **Linéaire :** le bot peut passer par la meme map plusieurs fois.
* **Circulaire :** possibilité de recommencer le script depuis le debut.

```lua
-- true = recommencer le script depuis le début, necessite que la dernière carte vous mène à la première carte.
RC_CIRCULAR = true

-- Tableau des actions
mapActionsTable =
{
    { map = "5,-18", path = "top" },
    { map = "5,-19", path = "bottom", fight = true },
    { map = "5,-18", path = "right" },
    { map = "6,-18", path = "left", fight = true },
    { map = "5,-18", path = "bottom" },
    { map = "5,-17", path = "top", fight = true },
    { map = "5,-18", path = "left" },
    { map = "4,-18", path = "right", fight = true },
}
for _, element in ipairs(mapActionsTable) do element.done = false end

-- Ne pas toucher à cette fonction
function getMapActions()

    -- Retourner la première carte non visitée
    for _, mapActions in ipairs(mapActionsTable) do
        if map.onMap(mapActions.map) and not mapActions.done then
            mapActions.done = true
            return mapActions
        end
        mapActions.done = true
    end

    -- Toutes les cartes sont visitées ? on réinitialise
    for _, mapActions in ipairs(mapActionsTable) do
        mapActions.done = false
    end

    -- Script circulaire ?
    if RC_CIRCULAR then
        -- Retourner la première carte non visitée
        for _, mapActions in ipairs(mapActionsTable) do
            if map.onMap(mapActions.map) and not mapActions.done then
                mapActions.done = true
                return mapActions
            end
            mapActions.done = true
        end
    end

    -- Aucune carte ?
    return nil
end

-- Fonction d'entrée
function move()
    -- Ajouter ce que vous voulez ici

    -- Ne pas toucher à cette partie au-dessous
    if character.wasInFight() and mapActions ~= nil and map.onMap(mapActions.map) then
        return { mapActions }
    end
    mapActions = getMapActions()
    if mapActions ~= nil then
        return { mapActions }
    end
end
```

* Remarquez que la carte "5,-18" (Zaap Astrub) est répétée plusieurs fois.
* Cet exemple à lancer sur le Zaap Astrub.
* Pour vous, il suffit juste de modifier la table **mapActionsTable** et ne rien toucher.
