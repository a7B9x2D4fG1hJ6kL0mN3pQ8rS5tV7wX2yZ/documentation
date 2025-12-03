# discordMessage

{% hint style="success" %}
Méthode permettant d'envoyer un message complet via un WebHook Discord.
{% endhint %}

## 🔍 Prototype

```lua
web.discordMessage(webhook_url, message)
```

## 📝 Paramètres

| Paramètre                      | Type                     | Description                     |
| ------------------------------ | ------------------------ | ------------------------------- |
| <ul><li>webhook\_url</li></ul> | <ul><li>string</li></ul> | <ul><li>Lien WebHook.</li></ul> |
| <ul><li>message</li></ul>      | <ul><li>string</li></ul> | <ul><li>JSON complet.</li></ul> |

## 🔙 Retour

| Type | Description |
| ---- | ----------- |
|      |             |

## 📌 Exemple

{% code fullWidth="false" %}

```lua
web.discordMessage("WEBHOOK_ICI", "{\"content\":\"hello\"}")
```

{% endcode %}
