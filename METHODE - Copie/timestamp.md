# timestamp

{% hint style="success" %}
Méthode permettant de retourner le unix timestamp.
{% endhint %}

## 🔍 Prototype

```lua
global.timestamp(inMs)
```

## 📝 Paramètres

| Paramètre              | Type                                                                                                                                | Description                                                                                                             |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| <ul><li>inMs</li></ul> | <ul><li>bool</li><li>Ce paramètre est facultatif, s'il n'est pas défini, la valeur par défaut est <strong>false</strong>.</li></ul> | <ul><li>false = la valeur retournée est en secondes.</li><li>true = la valeur retournée est en millisecondes.</li></ul> |

## 🔙 Retour

| Type                  | Description                          |
| --------------------- | ------------------------------------ |
| <ul><li>int</li></ul> | <ul><li>Le unix timestamp.</li></ul> |
