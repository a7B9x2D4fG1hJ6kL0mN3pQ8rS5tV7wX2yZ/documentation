# findPath

{% hint style="success" %}
Méthode permettant calculer le chemin entre deux cellules tout en évitant des obstacles.

* Peut aussi être utilisée pour calculer la distance entre deux cellules suivant un chemin.
  {% endhint %}

## 🔍 Prototype

```lua
fight.findPath(fromCellId, toCellId, obstacles)
```

## 📝 Paramètres

| Paramètre                    | Type                           | Description                                                                 |
| ---------------------------- | ------------------------------ | --------------------------------------------------------------------------- |
| <ul><li>fromCellId</li></ul> | <ul><li>int</li></ul>          | <ul><li>Cellule du départ</li></ul>                                         |
| <ul><li>toCellId</li></ul>   | <ul><li>int</li></ul>          | <ul><li>Cellule d'arrivé.</li></ul>                                         |
| <ul><li>obstacles</li></ul>  | <ul><li>Liste de int</li></ul> | <ul><li>Liste des cellules à éviter pendant le calcule du chemin.</li></ul> |

## 🔙 Retour

| Type                           | Description                                                                                                                           |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>Liste de int</li></ul> | <ul><li>Liste contenant les cellules du chemin calculé.</li><li>Liste vide <code>{ }</code> si aucun chemin n'a été trouvé.</li></ul> |
