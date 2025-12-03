# adjacentCells

{% hint style="success" %}
Méthode permettant retourner les cellules adjacentes à une cellule spécifique.

* Cette méthode ne vérifie pas que les cellules retournées contiennent un obstacle ou un autre combattant.
  {% endhint %}

## 🔍 Prototype

```lua
fight.adjacentCells(cellId)
```

## 📝 Paramètres

| Paramètre                | Type                  | Description                               |
| ------------------------ | --------------------- | ----------------------------------------- |
| <ul><li>cellId</li></ul> | <ul><li>int</li></ul> | <ul><li>Une cellule spécifique.</li></ul> |

## 🔙 Retour

| Type                           | Description                                                               |
| ------------------------------ | ------------------------------------------------------------------------- |
| <ul><li>Liste de int</li></ul> | <ul><li>Liste des cellules adjacentes à une cellule spécifique.</li></ul> |
