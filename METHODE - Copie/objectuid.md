# objectUid

{% hint style="success" %}
Méthode permettant de retourner le UID d'un objet dans l'espace de stockage.
{% endhint %}

## 🔍 Prototype

```lua
storage.objectUid(gid)
```

## 📝 Paramètres

| Paramètre             | Type                  | Description                                                                                                         |
| --------------------- | --------------------- | ------------------------------------------------------------------------------------------------------------------- |
| <ul><li>gid</li></ul> | <ul><li>int</li></ul> | <ul><li>Identifiant <a href="https://www.frigost.dev/API/Dofus%203.0/Data/Items.json">GID</a> de l'objet.</li></ul> |

## 🔙 Retour

| Type                  | Description                                                                                                                                     |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>int</li></ul> | <ul><li>UID l'objet <a href="https://www.frigost.dev/API/Dofus%203.0/Data/Items.json">GID</a>.</li><li>-1 si l'objet est introuvable.</li></ul> |

{% hint style="success" %}
Rendez-vous sur [cette page](https://www.frigost.dev/API/Dofus%203.0/Data/) pour récupérer des identifiants.
{% endhint %}
