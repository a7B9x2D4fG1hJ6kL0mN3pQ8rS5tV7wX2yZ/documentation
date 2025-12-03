# reply

{% hint style="success" %}
Méthode permettant de répondre à un dialogue avec un PNJ.
{% endhint %}

## 🔍 Prototype

```lua
npc.reply(replyId)
```

## 📝 Paramètres

| Paramètre                 | Type                  | Description                                                                                                                                                                                     |
| ------------------------- | --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>replyId</li></ul> | <ul><li>int</li></ul> | <ul><li>L'identifiant de la réponse.</li><li>Si négatif, correspond à l'index de la réponse, par exemple -1 pour choisir la première réponse, -2 pour choisir la deuxième réponse ...</li></ul> |

## 🔙 Retour

| Type                   | Description                                           |
| ---------------------- | ----------------------------------------------------- |
| <ul><li>bool</li></ul> | <ul><li>Indiquant le succès de l'opération.</li></ul> |
