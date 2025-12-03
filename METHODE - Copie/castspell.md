# castSpell

{% hint style="success" %}
Méthode permettant de lancer un sort sur une cellule.

* Quand cette fonction est appelée, l'exécution de la fonction [fight\_action()](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/utilisation-de-lia-avancee/style-1) est interrompu.
  {% endhint %}

## 🔍 Prototype

```lua
fight.castSpell(spellId, cellId, force)
```

## 📝 Paramètres

| Paramètre                 | Type                                | Description                                                                                                                                                                                                         |
| ------------------------- | ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>spellId</li></ul> | <ul><li>int</li></ul>               | <ul><li>L'identifiant du sort.</li></ul>                                                                                                                                                                            |
| <ul><li>cellId</li></ul>  | <ul><li>int</li></ul>               | <ul><li>La cellule ciblée.</li></ul>                                                                                                                                                                                |
| <ul><li>force</li></ul>   | <ul><li>bool (facultatif)</li></ul> | <ul><li>false : la fonction ne vérifie pas si le personnage est capable de lancer le sort, utile pour utiliser l'arme.</li><li>true : la fonction vérifie si le personnage est capable de lancer le sort.</li></ul> |

## 🔙 Retour

| Type                    | Description                                                    |
| ----------------------- | -------------------------------------------------------------- |
| <ul><li>false</li></ul> | <ul><li>Si le combattant ne peut pas lancer le sort.</li></ul> |
| <ul><li>nil</li></ul>   | <ul><li>Si le sort a été lancé.</li></ul>                      |
