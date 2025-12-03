# canCastSpell

{% hint style="success" %}
Méthode permettant d'indiquer si un sort peut être lancé par le combattant.

* Retourne <mark style="color:$primary;">enum\_SpellCastError.NoError</mark> si le sort peut être lancé.
  {% endhint %}

## 🔍 Prototype

```lua
fight.canCastSpell(spellId, launchCellId, targetCellId)
```

## 📝 Paramètres

| Paramètre                      | Type                  | Description                                        |
| ------------------------------ | --------------------- | -------------------------------------------------- |
| <ul><li>spellId</li></ul>      | <ul><li>int</li></ul> | <ul><li>L'identifiant du sort.</li></ul>           |
| <ul><li>launchCellId</li></ul> | <ul><li>int</li></ul> | <ul><li>La cellule du lancement du sort.</li></ul> |
| <ul><li>targetCellId</li></ul> | <ul><li>int</li></ul> | <ul><li>La cellule ciblée.</li></ul>               |

## 🔙 Retour

<table><thead><tr><th width="208">Type</th><th>Description</th></tr></thead><tbody><tr><td><ul><li>enum</li></ul></td><td><ul><li>enum_SpellCastError.NoError</li></ul><ul><li>enum_SpellCastError.DontHaveSpell</li><li>enum_SpellCastError.UnknownError</li><li>enum_SpellCastError.DataNotInitialized</li><li>enum_SpellCastError.HasCooldown</li><li>enum_SpellCastError.HasInitialCooldown</li><li>enum_SpellCastError.MaxCastPerTurnReached</li><li>enum_SpellCastError.MaxCastPerTargetReached</li><li>enum_SpellCastError.BadState</li><li>enum_SpellCastError.CellIsOccupied</li><li>enum_SpellCastError.CellIsFree</li><li>enum_SpellCastError.SummonLimitReached</li><li>enum_SpellCastError.NotEnoughAP</li><li>enum_SpellCastError.NotInRange</li><li>enum_SpellCastError.NotInLine</li><li>enum_SpellCastError.NotInDiagonal</li><li>enum_SpellCastError.NotInLineAndNotInDiagonal</li><li>enum_SpellCastError.NotInLineOfSight</li></ul></td></tr></tbody></table>
