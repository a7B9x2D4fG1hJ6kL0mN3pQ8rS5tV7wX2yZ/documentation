# autotripDistance

{% hint style="success" %}
Méthode permettant de calculer la distance entre deux cartes, c'est la même distance qui sera parcourue par un autopilotage.
{% endhint %}

## 🔍 Prototype

```lua
map.autotripDistance(fromMapId, toMapId)
```

## 📝 Paramètres

| Paramètre                   | Type                  | Description                    |
| --------------------------- | --------------------- | ------------------------------ |
| <ul><li>fromMapId</li></ul> | <ul><li>int</li></ul> | <ul><li>Départ.</li></ul>      |
| <ul><li>toMapId</li></ul>   | <ul><li>int</li></ul> | <ul><li>Destination.</li></ul> |

## 🔙 Retour

| Type                  | Description                                                        |
| --------------------- | ------------------------------------------------------------------ |
| <ul><li>int</li></ul> | <ul><li>La distance, sinon -1 en cas d'échec ou timeout.</li></ul> |
