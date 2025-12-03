# content

{% hint style="success" %}
Méthode permettant de retourner le contenu de l'espace de stockage.
{% endhint %}

## 🔍 Prototype

```lua
storage.content()
```

## 📝 Paramètres

| Paramètre | Type | Description |
| --------- | ---- | ----------- |
|           |      |             |

## 🔙 Retour

| Type                             | Description                                           |
| -------------------------------- | ----------------------------------------------------- |
| <ul><li>Liste d'objets</li></ul> | <ul><li>Le contenu de l'espace de stockage.</li></ul> |

{% hint style="success" %}
Rendez-vous sur [cette page](https://www.frigost.dev/API/Dofus%203.0/Data/) pour récupérer des identifiants.
{% endhint %}

## 📌 Exemple

{% code fullWidth="false" %}

```lua
local content = storage.content()
for _, object in ipairs(content) do
    console.print("---------------------------------------")
    console.print("Gid: "..object["gid"])
    console.print("Uid: "..object["uid"])
    console.print("Quantity: "..object["quantity"])
    console.print("Position: "..object["position"])
    console.print("Name: "..object["name"])
end
```

{% endcode %}
