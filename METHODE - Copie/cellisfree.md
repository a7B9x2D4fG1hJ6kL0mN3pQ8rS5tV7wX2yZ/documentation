# cellIsFree

{% hint style="success" %}
Méthode permettant d'indiquer si une cellule est [walkable](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/methodes/cellules/celliswalkable) et libre (ne contient aucun combattant).
{% endhint %}

## 🔍 Prototype

```lua
fight.cellIsFree(cellId)
```

## 📝 Paramètres

| Paramètre                | Type                  | Description                              |
| ------------------------ | --------------------- | ---------------------------------------- |
| <ul><li>cellId</li></ul> | <ul><li>int</li></ul> | <ul><li>La cellule à vérifier.</li></ul> |

## 🔙 Retour

| Type                   | Description                                                                         |
| ---------------------- | ----------------------------------------------------------------------------------- |
| <ul><li>bool</li></ul> | <ul><li>Indiquant si la cellule est libre (ne contient aucun combattant).</li></ul> |
