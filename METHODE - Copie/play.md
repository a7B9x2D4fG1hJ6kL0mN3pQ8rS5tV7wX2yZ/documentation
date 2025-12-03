# play

{% hint style="success" %}
Méthode permettant de jouer avec l'IA basique.

* Quand cette fonction est appelée, l'exécution de la fonction <mark style="color:green;">fight\_action()</mark> est interrompu.
  {% endhint %}

## 🔍 Prototype

```lua
basicFight.play(permanent, tactic, focus, tacklePath, distanceCondition)
```

## 📝 Paramètres

<figure><img src="https://3373271050-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-Mfulp0LhbJrdkH_fl5w%2Fuploads%2F5RfMZfjzgyoO8QN48IJb%2Fimage.png?alt=media&#x26;token=78f1e38a-a040-4b03-9ddc-76b91cf44e7e" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="204">Paramètre</th><th width="126">Type</th><th>Description</th></tr></thead><tbody><tr><td><ul><li>permanent</li></ul></td><td><ul><li>bool</li></ul></td><td><ul><li>true = le personnage va jouer la suite du tour avec l'IA basique.</li><li>false = le personnage va jouer une seule action avec l'IA basique.</li></ul></td></tr><tr><td><ul><li>tactic</li></ul></td><td><ul><li>enum</li></ul></td><td><ul><li>enum_TacticType.HandToHand</li></ul><ul><li>enum_TacticType.Distance</li><li>enum_TacticType.Immobile</li></ul></td></tr><tr><td><ul><li>focus</li></ul></td><td><ul><li>enum</li></ul></td><td><ul><li>enum_FocusType.Closest</li></ul><ul><li>enum_FocusType.Weakest</li></ul></td></tr><tr><td><ul><li>tacklePath</li></ul></td><td><ul><li>enum</li></ul></td><td><ul><li>enum_TacklePathType.AllPaths</li></ul><ul><li>enum_TacklePathType.OnlyNonTackledPaths</li></ul></td></tr><tr><td><ul><li>distanceCondition</li></ul></td><td><ul><li>int</li></ul></td><td><ul><li>Voir l'option de l'interface.</li></ul></td></tr></tbody></table>

## 🔙 Retour

| Type | Description |
| ---- | ----------- |
|      |             |
