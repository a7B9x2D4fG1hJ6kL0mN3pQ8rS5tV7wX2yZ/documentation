# onMap

{% hint style="success" %}
Méthode permettant d'indiquer si le personage est sur une carte.
{% endhint %}

## 🔍 Prototype

```lua
map.onMap(map)
```

## 📝 Paramètres

| Paramètre             | Type                     | Description                            |
| --------------------- | ------------------------ | -------------------------------------- |
| <ul><li>map</li></ul> | <ul><li>string</li></ul> | <ul><li>La carte à vérifier.</li></ul> |

## 🔙 Retour

| Type                   | Description                                                   |
| ---------------------- | ------------------------------------------------------------- |
| <ul><li>bool</li></ul> | <ul><li>Indiquant si le personage est sur la carte.</li></ul> |

## 📌 Exemple

{% code fullWidth="false" %}

```lua
-- Par les coordonnées
if map.onMap("5,-18") then

end

-- Par MapId
if map.onMap("164859940") then

end
```

{% endcode %}
