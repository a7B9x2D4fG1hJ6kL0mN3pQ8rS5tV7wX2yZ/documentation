# objectPosition

{% hint style="success" %}
Méthode permettant de retourner la position d'un objet dans l'inventaire.
{% endhint %}

## 🔍 Prototype

```lua
inventory.objectPosition(gid)
```

## 📝 Paramètres

| Paramètre             | Type                  | Description                                                                                                         |
| --------------------- | --------------------- | ------------------------------------------------------------------------------------------------------------------- |
| <ul><li>gid</li></ul> | <ul><li>int</li></ul> | <ul><li>Identifiant <a href="https://www.frigost.dev/API/Dofus%203.0/Data/Items.json">GID</a> de l'objet.</li></ul> |

## 🔙 Retour

| Type                  | Description                                                                                                                                                |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>int</li></ul> | <ul><li>La position de l'objet <a href="https://www.frigost.dev/API/Dofus%203.0/Data/Items.json">GID</a>.</li><li>-1 si l'objet est introuvable.</li></ul> |

{% hint style="success" %}
Rendez-vous sur [cette page](https://www.frigost.dev/API/Dofus%203.0/Data/) pour récupérer des identifiants.
{% endhint %}
