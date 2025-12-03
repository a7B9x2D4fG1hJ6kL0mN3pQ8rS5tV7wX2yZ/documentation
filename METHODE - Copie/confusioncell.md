# confusionCell

{% hint style="success" %}
Méthode permettant de retourner la cellule qu'il faut viser pour cibler une cible dans un combat à confusion.
{% endhint %}

## 🔍 Prototype

```lua
fight.confusionCell(confusion, centerCell, targetCell)
```

## 📝 Paramètres

| Paramètre                    | Type                  | Description                                                               |
| ---------------------------- | --------------------- | ------------------------------------------------------------------------- |
| <ul><li>confusion</li></ul>  | <ul><li>int</li></ul> | <ul><li>Retourné par <a href="confusion">fight.confusion()</a>.</li></ul> |
| <ul><li>centerCell</li></ul> | <ul><li>int</li></ul> | <ul><li>La cellule du du lancement du sort.</li></ul>                     |
| <ul><li>targetCell</li></ul> | <ul><li>int</li></ul> | <ul><li>La cellule à cibler.</li></ul>                                    |

## 🔙 Retour

| Type                  | Description                                                                                                |
| --------------------- | ---------------------------------------------------------------------------------------------------------- |
| <ul><li>int</li></ul> | <ul><li>La cellule qu'il faut viser pour cibler <mark style="color:$primary;">targetCell</mark>.</li></ul> |
