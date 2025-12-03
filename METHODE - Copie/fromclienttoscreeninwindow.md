# fromClientToScreenInWindow

{% hint style="success" %}
Méthode permettant de convertir les coordonnées client (relatives à une fenêtre spécifique) en coordonnées écran (relatives à l'écran entier).
{% endhint %}

## 🔍 Prototype

```lua
pixel.fromClientToScreenInWindow(hwnd, x, y)
```

## 📝 Paramètres

| Paramètre              | Type                       | Description                                                                                                     |
| ---------------------- | -------------------------- | --------------------------------------------------------------------------------------------------------------- |
| <ul><li>hwnd</li></ul> | <ul><li>HWND</li></ul>     | <ul><li>Identifiant de la fenêtre à récupérer avec l'une des méthodes <a href="../window">window</a>.</li></ul> |
| <ul><li>x, y</li></ul> | <ul><li>int, int</li></ul> | <ul><li>Les coordonnées à convertir.</li></ul>                                                                  |

## 🔙 Retour

| Type                       | Description                    |
| -------------------------- | ------------------------------ |
| <ul><li>{ x, y }</li></ul> | <ul><li>Le résultat.</li></ul> |
