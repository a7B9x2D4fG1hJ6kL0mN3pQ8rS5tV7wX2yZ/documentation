# color

{% hint style="success" %}
Méthode permettant de retourner la couleur d'un pixel.
{% endhint %}

{% hint style="danger" %}
Ne pas réduire la fenêtre en question sinon cette méthode va toujours retourner la couleur noire "#000000".
{% endhint %}

## 🔍 Prototype

```lua
pixel.color(x, y)
```

## 📝 Paramètres

| Paramètre              | Type                       | Description                                                                               |
| ---------------------- | -------------------------- | ----------------------------------------------------------------------------------------- |
| <ul><li>x, y</li></ul> | <ul><li>int, int</li></ul> | <ul><li>Les coordonnées du pixel relatives à la fenêtre (et non pas à l'écran).</li></ul> |

## 🔙 Retour

| Type                     | Description                                           |
| ------------------------ | ----------------------------------------------------- |
| <ul><li>string</li></ul> | <ul><li>La couleur sous la forme "#XXXXXX".</li></ul> |
