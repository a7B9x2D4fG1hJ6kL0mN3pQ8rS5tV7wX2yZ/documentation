# hasLineOfSight

{% hint style="success" %}
Méthode permettant d'indiquer si un combattant possède la ligne de vue entre deux cellules.
{% endhint %}

## 🔍 Prototype

```lua
fight.hasLineOfSight(launchCell, targetCell, id)
```

## 📝 Paramètres

| Paramètre                                       | Type                                                                                                                                                                                                                                                       | Description                                  |
| ----------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| <ul><li>launchCell</li><li>targetCell</li></ul> | <ul><li>int</li></ul>                                                                                                                                                                                                                                      | <ul><li>Les deux cellules.</li></ul>         |
| <ul><li>id</li></ul>                            | <ul><li>int</li></ul><ul><li>Ce paramètre est facultatif, s'il n'est pas défini, la valeur par défaut est <strong>l'</strong><a href="../combattants/currentfighterid"><strong>identifiant du combattant en train de jouer le tour</strong></a>.</li></ul> | <ul><li>Identifiant du combattant.</li></ul> |

## 🔙 Retour

| Type                   | Description                                                                                                                      |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>bool</li></ul> | <ul><li>true = possède la ligne de vue.</li><li>false = ne possède pas la ligne de vue, ou le combattant n'existe pas.</li></ul> |
