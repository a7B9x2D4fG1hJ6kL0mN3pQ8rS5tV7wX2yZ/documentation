# teleport

{% hint style="success" %}
Méthode permettant d'utiliser le zaap/zaapi présent dans la carte pour se téléporter à une destination.
{% endhint %}

## 🔍 Prototype

```lua
map.teleport(destinationMapId, isZaapi, timeout)
```

## 📝 Paramètres

| Paramètre                          | Type                                                                                                                                        | Description                                                                                         |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| <ul><li>destinationMapId</li></ul> | <ul><li>int</li></ul>                                                                                                                       | <ul><li>La destination.</li></ul>                                                                   |
| <ul><li>isZaapi</li></ul>          | <ul><li>bool</li><li>Ce paramètre est facultatif, s'il n'est pas défini, la valeur par défaut est <strong>false</strong>.</li></ul>         | <ul><li>false = zaap.</li><li>true = zaapi.</li></ul>                                               |
| <ul><li>timeout</li></ul>          | <ul><li>int</li></ul><ul><li>Ce paramètre est facultatif, s'il n'est pas défini, la valeur par défaut est <strong>10000</strong>.</li></ul> | <ul><li>La durée maximale à attendre avant de retourner en cas d'échec, en millisecondes.</li></ul> |

## 🔙 Retour

| Type                   | Description                                           |
| ---------------------- | ----------------------------------------------------- |
| <ul><li>bool</li></ul> | <ul><li>Indiquant le succès de l'opération.</li></ul> |
