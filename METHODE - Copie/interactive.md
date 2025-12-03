# interactive

{% hint style="success" %}
Méthode permettant d'utiliser un interactif.
{% endhint %}

## 🔍 Prototype

```lua
map.interactive(elementId, skillInstanceUid, changeMap, timeout)
```

## 📝 Paramètres

| Paramètre                          | Type                                                                                                                                | Description                                                                                                                                                                                                              |
| ---------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <ul><li>elementId</li></ul>        | <ul><li>int</li></ul>                                                                                                               | <ul><li>La cellule de l'interactif, à récupérer avec <a href="../../outils-pour-les-scripts/elements-de-la-carte">cet outil</a>.</li></ul>                                                                               |
| <ul><li>skillInstanceUid</li></ul> | <ul><li>int</li></ul>                                                                                                               | <ul><li>L'identifiant de la réponse.</li></ul><ul><li>Si négatif, correspond à l'index de la réponse, par exemple -1 pour choisir la première réponse, -2 pour choisir la deuxième réponse ...</li></ul>                 |
| <ul><li>changeMap</li></ul>        | <ul><li>bool</li><li>Ce paramètre est facultatif, s'il n'est pas défini, la valeur par défaut est <strong>false</strong>.</li></ul> | <ul><li>true = l'utilisation a pour but de changer la carte, dans ce cas la méthode va attendre le changement de carte.</li><li>false = la méthode retourne immédiatement après l'utilisation de l'interactif.</li></ul> |
| <ul><li>timeout</li></ul>          | <ul><li>int</li><li>Ce paramètre est facultatif, s'il n'est pas défini, la valeur par défaut est <strong>10000</strong>.</li></ul>  | <ul><li>La durée maximale à attendre avant de retourner en cas d'échec, en millisecondes.</li></ul>                                                                                                                      |

## 🔙 Retour

| Type                   | Description                                           |
| ---------------------- | ----------------------------------------------------- |
| <ul><li>bool</li></ul> | <ul><li>Indiquant le succès de l'opération.</li></ul> |
