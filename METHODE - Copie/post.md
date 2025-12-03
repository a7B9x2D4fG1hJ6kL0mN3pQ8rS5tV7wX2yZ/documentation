# post

{% hint style="success" %}
Méthode permettant d'envoyer une requête POST.
{% endhint %}

## 🔍 Prototype

```lua
web.post(url, data, ua, headers)
```

## 📝 Paramètres

| Paramètre                 | Type                                           | Description                                                                       |
| ------------------------- | ---------------------------------------------- | --------------------------------------------------------------------------------- |
| <ul><li>url</li></ul>     | <ul><li>string</li></ul>                       | <ul><li>URL.</li></ul>                                                            |
| <ul><li>data</li></ul>    | <ul><li>string</li></ul>                       | <ul><li>Les données (POST) au format application/x-www-form-urlencoded.</li></ul> |
| <ul><li>ua</li></ul>      | <ul><li>string (facultatif)</li></ul>          | <ul><li>UserAgent à envoyer.</li></ul>                                            |
| <ul><li>headers</li></ul> | <ul><li>Liste de string (facultatif)</li></ul> | <ul><li>Headers à envoyer.</li></ul>                                              |

## 🔙 Retour

| Type                           | Description                                  |
| ------------------------------ | -------------------------------------------- |
| <ul><li>false (bool)</li></ul> | <ul><li>En cas d'échec ou timeout.</li></ul> |
| <ul><li>string</li></ul>       | <ul><li>La réponse à la requête.</li></ul>   |

## 📌 Exemple

{% code fullWidth="false" %}

```lua
local response = web.post("https://api.ipify.org/?format=json", "key1=value1&key2=value2")
local response = web.post("https://api.ipify.org/?format=json", "key1=value1&key2=value2", "Frigost")
local response = web.post("https://api.ipify.org/?format=json", "key1=value1&key2=value2", "Frigost", {"Header1: Value1", "Header2: Value2"})
```

{% endcode %}
