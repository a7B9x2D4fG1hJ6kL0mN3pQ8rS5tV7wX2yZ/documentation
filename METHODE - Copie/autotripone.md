# autotripOne

{% hint style="success" %}
Méthode permettant de se déplacer d'une carte vers une destination en utilisant l'autopilotage.
{% endhint %}

## 🔍 Prototype

```lua
map.autotripOne(mapId)
```

## 📝 Paramètres

| Paramètre               | Type                  | Description                    |
| ----------------------- | --------------------- | ------------------------------ |
| <ul><li>mapId</li></ul> | <ul><li>int</li></ul> | <ul><li>Destination.</li></ul> |

## 🔙 Retour

| Type                           | Description                                                                  |
| ------------------------------ | ---------------------------------------------------------------------------- |
| <ul><li>false (bool)</li></ul> | <ul><li>Si aucun changement de carte n'a été effectué pendant 10s.</li></ul> |
