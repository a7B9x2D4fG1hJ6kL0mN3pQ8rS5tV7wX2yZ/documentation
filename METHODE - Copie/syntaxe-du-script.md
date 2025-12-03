# Syntaxe du script

### <mark style="color:$primary;">Exemple</mark>

Voici un exemple simple de script LUA compatible avec <mark style="color:$primary;">Frigost</mark> :&#x20;

```lua
MIN_MONSTERS = 4 -- Le groupe doit contenir au minimum 4 monstres
MAX_MONSTERS = 8 -- Le groupe doit contenir au maximum 8 monstres
FORCE_MONSTERS = { 490, 489 } -- Le groupe doit contenir piou rouge ou piou vert
FORBIDDEN_MONSTERS = { 491 } -- Le groupe ne doit pas contenir piou bleu

function astrub()
    npc.talk(4398)
    npc.reply(-1)
    npc.reply(-1)
end

function move()
    return {
        { map = "153880835", custom = astrub },
        { map = "192416776", path = "bottom" },
        { map = "6,-19", path = "left", fight = true },
        { map = "5,-19", path = "left", fight = true },
        { map = "4,-19", path = "bottom", fight = true },
        { map = "4,-18", path = "bottom", fight = true },
        { map = "4,-17", path = "right", fight = true },
        { map = "5,-17", path = "right", fight = true },
        { map = "6,-17", path = "top", fight = true },
        { map = "6,-18", path = "top", fight = true },
    }
end
```

### <mark style="color:$primary;">Explications</mark>&#x20;

* Quand vous lancez le script, il va exécuter immédiatement la fonction <mark style="color:$primary;">move()</mark>.
* Après chaque changement de carte, il va exécuter la fonction <mark style="color:$primary;">move()</mark>.
* La fonction <mark style="color:$primary;">move()</mark> doit retourner un tableau qui contient les cartes (soit avec leurs <mark style="color:$primary;">coordonnées</mark> ou avec leurs <mark style="color:$primary;">MapId</mark>), et les actions à effectuer sur chaque carte.
* Par exemple dans la carte <mark style="color:$primary;">"4,-18"</mark>, on dit au script de combattre (<mark style="color:$primary;">fight = true</mark>), et après se diriger vers le bas (<mark style="color:$primary;">path = "bottom"</mark>).
* Par exemple dans la carte <mark style="color:$primary;">"153880835"</mark>, on dit au script d'exécuter la fonction <mark style="color:$primary;">astrub()</mark> (<mark style="color:$primary;">custom = astrub</mark>), cette fonction s'occupe de parler au PNJ pour sortir d'Incarnam.

### <mark style="color:$primary;">Actions possibles</mark>

| Action                                        | Explication                                                                                                                                                                                                                                           |                |                                                                                                     |         |                |
| --------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- | --------------------------------------------------------------------------------------------------- | ------- | -------------- |
| <ul><li>fight = true</li></ul>                | <ul><li>Pour combattre tous les groupes de monstres possibles dans la carte.</li></ul>                                                                                                                                                                |                |                                                                                                     |         |                |
| <ul><li>forceFight = true</li></ul>           | <ul><li>Pour combattre tous les groupes de monstres possibles dans la carte, et attendre à l'infini leur réapparition.</li></ul>                                                                                                                      |                |                                                                                                     |         |                |
| <ul><li>gather = true</li></ul>               | <ul><li>Pour effectuer toutes les récoltes possibles dans la carte.</li></ul>                                                                                                                                                                         |                |                                                                                                     |         |                |
| <ul><li>forceGather = true</li></ul>          | <ul><li>Pour effectuer toutes les récoltes possibles dans la carte, et attendre à l'infini leur réapparition.</li></ul>                                                                                                                               |                |                                                                                                     |         |                |
| <ul><li>path = "cellule"</li></ul>            | <ul><li>Pour changer la carte à travers une cellule (soleil).</li><li>Par exemple : <br>path = "318"</li></ul>                                                                                                                                        |                |                                                                                                     |         |                |
| <ul><li>path = "direction"</li></ul>          | <p></p><ul><li>Pour changer la carte en allant vers une direction.<br>top = aller vers le haut<br>bottom = aller vers le bas<br>right = aller vers la droite<br>left = aller vers la gauche</li></ul><ul><li>Par exemple : <br>path = "top"</li></ul> |                |                                                                                                     |         |                |
| <ul><li>path = "direction(cellule)"</li></ul> | <p></p><ul><li>Pour changer la carte en allant vers une direction et à travers une cellule spécifique.</li></ul><ul><li>Par exemple : <br>path = "top(10)"</li></ul>                                                                                  |                |                                                                                                     |         |                |
| <ul><li>path = "direction1                    | direction2                                                                                                                                                                                                                                            | ..."</li></ul> | <ul><li>Pour dire au bot de choisir une direction aléatoire.</li><li>Par exemple : <br>path = "left | top(10) | 367"</li></ul> |
| <ul><li>path = "havenbag"</li></ul>           | <ul><li>Pour entrer ou sortir de l'havre sac.</li></ul>                                                                                                                                                                                               |                |                                                                                                     |         |                |
| <ul><li>path = "zaap(map\_id)"</li></ul>      | <ul><li>Pour utiliser le zaap présent dans la carte, et se téléporter à la carte map\_id.</li></ul>                                                                                                                                                   |                |                                                                                                     |         |                |
| <ul><li>path = "zaapi(map\_id)"</li></ul>     | <ul><li>Pour utiliser le zaapi présent dans la carte, et se téléporter à la carte map\_id.</li></ul>                                                                                                                                                  |                |                                                                                                     |         |                |
| <ul><li>door = cellule</li></ul>              | <ul><li>Pour utiliser une porte située située sur une cellule X.</li><li>Par exemple :<br>door = 137</li></ul>                                                                                                                                        |                |                                                                                                     |         |                |
| <ul><li>custom = fonction</li></ul>           | <ul><li>Pour exécuter une fonction.                                                                                                                                                                                                                   |                |                                                                                                     |         |                |

</li><li>Par exemple :<br>custom = UtiliserPotion</li><li>La fonction UtiliserPotion doit être déjà définie sur votre script)</li><li>En groupe, la fonction sera exécutée en même temps par tous les membres.</li></ul> |
| <ul><li>lockedCustom = fonction</li></ul>            | <ul><li>Utilisable uniquement en groupe.</li><li>La même chose que custom, sauf que la fonction sera exécuté par chaque membre 1 par 1.</li><li>Utile pour les échanges ou pour l'utilisation d'un coffre de maison.</li></ul>                                |

```lua
-- Exemple
{ map = "6,-18", gather = true, fight = true, path = "top|right", custom = Pain }
```

### <mark style="color:$primary;">Priorité des actions</mark>

1. Récolter (gather et forceGather).
2. Combattre (fight et forceFight).
3. locked\_custom.
4. custom.
5. door.
6. path.

### <mark style="color:$primary;">Autres fonctions</mark>

* La fonction <mark style="color:$primary;">script\_stopped()</mark> qui sera exécutée quand le script s'arrete d'une manière involontaire.

```lua
function script_stopped()
    -- Faire ce que vous voulez ici
end
```

* La fonction <mark style="color:$primary;">team\_member\_lost()</mark> qui sera exécutée sur un membre du groupe lorsque qu'il est perdu du chef.

```lua
function team_member_lost(bossMapId)
    map.autotripOne(bossMapId)
end
```

```lua
function team_member_lost(bossMapId)
    return {
        { map = "5,-18", path = "top" },
    }
end
```

* La fonction <mark style="color:$primary;">bank()</mark> qui sera exécutée selon votre configuration ici :&#x20;

<figure><img src="https://3373271050-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-Mfulp0LhbJrdkH_fl5w%2Fuploads%2FJErxKLOWEebFcqEUxzxw%2Fimage.png?alt=media&#x26;token=f4c66c3f-f559-45df-8bfd-af7ae05c3874" alt=""><figcaption></figcaption></figure>

```lua
function bank()
    -- Faire ce que vous voulez ici, par exemple :
    -- Prendre le Zaap vers Astrub
    -- Aller à la banque
    -- Se vider
end
```
