# input

{% hint style="success" %}
Méthode permettant d'afficher une boîte de dialogue avec un champs de texte à saisir et à retourner.
{% endhint %}

## 🔍 Prototype

```lua
global.input(text)
```

## 📝 Paramètres

| Paramètre              | Type                     | Description                                                      |
| ---------------------- | ------------------------ | ---------------------------------------------------------------- |
| <ul><li>text</li></ul> | <ul><li>string</li></ul> | <ul><li>Le texte à afficher dans la boîte de dialogue.</li></ul> |

## 🔙 Retour

| Type                     | Description                       |
| ------------------------ | --------------------------------- |
| <ul><li>string</li></ul> | <ul><li>Le texte saisi.</li></ul> |

## 📌 Exemple

{% code fullWidth="false" %}

```lua
local output = global:input("Identifiant de l'objet à supprimer :")
```

{% endcode %}

<figure><img src="https://3373271050-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-Mfulp0LhbJrdkH_fl5w%2Fuploads%2FXy0BhwEkQuhXtdvnEJoo%2Fimage.png?alt=media&#x26;token=9f757de6-57ee-4d5c-a613-dc090ef8b72a" alt=""><figcaption></figcaption></figure>
