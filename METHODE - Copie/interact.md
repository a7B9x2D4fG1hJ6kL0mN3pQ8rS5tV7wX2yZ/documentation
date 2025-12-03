# interact

{% hint style="success" %}
Méthode permettant d'intéragir avec un PNJ.
{% endhint %}

## 🔍 Prototype

```lua
npc.interact(npcId, actionId)
```

## 📝 Paramètres

| Paramètre                  | Type                  | Description                                                                                                                                                    |
| -------------------------- | --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>npcId</li></ul>    | <ul><li>int</li></ul> | <ul><li>Identifiant du PNJ à récupérer avec <a href="../../outils-pour-les-scripts/elements-de-la-carte">cet outil</a>.</li></ul>                              |
| <ul><li>actionId</li></ul> | <ul><li>int</li></ul> | <ol><li>Achat / Vente.</li></ol><ol start="3"><li>Conversation.</li></ol><ol start="5"><li>Vente en hôtel de vente.</li><li>Achat en hôtel de vente.</li></ol> |

## 🔙 Retour

| Type                   | Description                                           |
| ---------------------- | ----------------------------------------------------- |
| <ul><li>bool</li></ul> | <ul><li>Indiquant le succès de l'opération.</li></ul> |
