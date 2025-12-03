# objectQuantity

{% hint style="success" %}
Méthode permettant de retourner la quantité d'un objet dans l'espace de stockage.
{% endhint %}

## 🔍 Prototype

```lua
storage.objectQuantity(gid, all)
```

## 📝 Paramètres

| Paramètre             | Type                                                                                                                                | Description                                                                                                                                                                                                                                                                                                                                          |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>gid</li></ul> | <ul><li>int</li></ul>                                                                                                               | <ul><li>Identifiant <a href="https://www.frigost.dev/API/Dofus%203.0/Data/Items.json">GID</a> de l'objet.</li></ul>                                                                                                                                                                                                                                  |
| <ul><li>all</li></ul> | <ul><li>bool</li><li>Ce paramètre est facultatif, s'il n'est pas défini, la valeur par défaut est <strong>false</strong>.</li></ul> | <ul><li>false = retourne la quantité du premier objet <a href="https://www.frigost.dev/API/Dofus%203.0/Data/Items.json">GID</a> présent dans l'espace de stockage.</li><li>true = retourne le total des quantités des objets <a href="https://www.frigost.dev/API/Dofus%203.0/Data/Items.json">GID</a> présents dans l'espace de stockage.</li></ul> |

## 🔙 Retour

| Type                  | Description                                                                                                         |
| --------------------- | ------------------------------------------------------------------------------------------------------------------- |
| <ul><li>int</li></ul> | <ul><li>La quantité de l'objet <a href="https://www.frigost.dev/API/Dofus%203.0/Data/Items.json">GID</a>.</li></ul> |

{% hint style="success" %}
Rendez-vous sur [cette page](https://www.frigost.dev/API/Dofus%203.0/Data/) pour récupérer des identifiants.
{% endhint %}
