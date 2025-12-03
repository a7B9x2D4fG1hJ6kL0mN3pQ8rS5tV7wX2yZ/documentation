# putAllObjects

{% hint style="success" %}
Méthode permettant de transférer tout son inventaire dans l'espace de stockage, à l'exception des objets spécifiés.
{% endhint %}

## 🔍 Prototype

```lua
storage.putAllObjects(exceptions)
```

## 📝 Paramètres

| Paramètre                    | Type                                                                                                                                     | Description                                                                                                                                        |
| ---------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>exceptions</li></ul> | <ul><li>{ int }</li><li>Ce paramètre est facultatif, s'il n'est pas défini, il transférera tout son inventaire sans exception.</li></ul> | <ul><li>Liste des identifiants <a href="https://www.frigost.dev/API/Dofus%203.0/Data/Items.json">GID</a> des objets à ne pas transférer.</li></ul> |

## 🔙 Retour

| Type | Description |
| ---- | ----------- |
|      |             |

{% hint style="success" %}
Rendez-vous sur [cette page](https://www.frigost.dev/API/Dofus%203.0/Data/) pour récupérer des identifiants.
{% endhint %}
