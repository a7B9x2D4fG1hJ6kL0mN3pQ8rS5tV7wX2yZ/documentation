# moveToAccessibleCell

{% hint style="success" %}
Méthode permettant de se déplacer à une cellule par son [index](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/objets/accessiblecell).

* Quand cette fonction est appelée, l'exécution de la fonction [fight\_action()](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/utilisation-de-lia-avancee/style-1) est interrompu.
  {% endhint %}

## 🔍 Prototype

```lua
fight.moveToAccessibleCell(index)
```

## 📝 Paramètres

| Paramètre               | Type                  | Description                                                                        |
| ----------------------- | --------------------- | ---------------------------------------------------------------------------------- |
| <ul><li>index</li></ul> | <ul><li>int</li></ul> | <ul><li>L'<a href="../../objets/accessiblecell">index</a> de la cellule.</li></ul> |

## 🔙 Retour

| Type                    | Description                                                                      |
| ----------------------- | -------------------------------------------------------------------------------- |
| <ul><li>false</li></ul> | <ul><li>En cas d'échec ou si le combattant est déjà sur cette cellule.</li></ul> |
| <ul><li>nil</li></ul>   | <ul><li>Le déplacement a été effectué.</li></ul>                                 |
