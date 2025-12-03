# moveTowardCell

{% hint style="success" %}
Méthode permettant de se déplacer à une cellule.

* Si la cellule est inaccessible, le combattant se déplace à la cellule la plus proche de cette dernière.
* Quand cette fonction est appelée, l'exécution de la fonction [fight\_action()](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/utilisation-de-lia-avancee/style-1) est interrompu.
  {% endhint %}

## 🔍 Prototype

```lua
fight.moveTowardCell(cellId)
```

## 📝 Paramètres

| Paramètre               | Type                  | Description                          |
| ----------------------- | --------------------- | ------------------------------------ |
| <ul><li>index</li></ul> | <ul><li>int</li></ul> | <ul><li>La cellule ciblée.</li></ul> |

## 🔙 Retour

| Type                    | Description                                                                      |
| ----------------------- | -------------------------------------------------------------------------------- |
| <ul><li>false</li></ul> | <ul><li>En cas d'échec ou si le combattant est déjà sur cette cellule.</li></ul> |
| <ul><li>nil</li></ul>   | <ul><li>Le déplacement a été effectué.</li></ul>                                 |
