# change

{% hint style="success" %}
Méthode permettant de changer la carte
{% endhint %}

## 🔍 Prototype

```lua
map.change(direction)
```

## 📝 Paramètres

| Paramètre                   | Type                     | Description                     |
| --------------------------- | ------------------------ | ------------------------------- |
| <ul><li>direction</li></ul> | <ul><li>string</li></ul> | <ul><li>La direction.</li></ul> |

## 🔙 Retour

| Type                   | Description                                           |
| ---------------------- | ----------------------------------------------------- |
| <ul><li>bool</li></ul> | <ul><li>Indiquant le succès de l'opération.</li></ul> |

## 📌 Exemple

{% hint style="success" %}
C'est la même syntaxe que [path](https://doc.frigost.dev/abonnement-frigost-bot/syntaxe-du-script).
{% endhint %}

{% code fullWidth="false" %}

```lua
map.change("left")
map.change("top(11)")
map.change("216")
```

{% endcode %}
