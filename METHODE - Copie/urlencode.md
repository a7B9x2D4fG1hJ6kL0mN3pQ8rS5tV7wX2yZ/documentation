# urlEncode

{% hint style="success" %}
Méthode permettant l'encodage d'une chaîne de caractères à utiliser dans la partie d'une URL.
{% endhint %}

## 🔍 Prototype

```lua
web.urlEncode(input)
```

## 📝 Paramètres

| Paramètre               | Type                     | Description                                        |
| ----------------------- | ------------------------ | -------------------------------------------------- |
| <ul><li>input</li></ul> | <ul><li>string</li></ul> | <ul><li> Chaîne de caractères à encoder.</li></ul> |

## 🔙 Retour

| Type                     | Description                                             |
| ------------------------ | ------------------------------------------------------- |
| <ul><li>string</li></ul> | <ul><li>Chaîne de caractères (input) encodée.</li></ul> |

## 📌 Exemple

{% code fullWidth="false" %}

```lua
local encodedValue = web.urlEncode("some=&fvdsvalue@ç&=")
local content = web.post("https://api.ipify.org/?format=json", "key1="..encodedValue)
```

{% endcode %}
