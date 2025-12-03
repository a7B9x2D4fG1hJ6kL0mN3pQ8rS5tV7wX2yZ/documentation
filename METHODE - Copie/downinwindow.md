# downInWindow

{% hint style="success" %}
Méthode permettant de simuler un appui d'une touche du clavier sur une fenêtre spécifique.
{% endhint %}

## 🔍 Prototype

```lua
keyboard.downInWindow(hwnd, key)
```

## 📝 Paramètres

| Paramètre              | Type                   | Description                                                                                                                                                                                                   |
| ---------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>hwnd</li></ul> | <ul><li>HWND</li></ul> | <ul><li>Identifiant de la fenêtre à récupérer avec l'une des méthodes <a href="../window">window</a>.</li></ul>                                                                                               |
| <ul><li>key</li></ul>  | <ul><li>int</li></ul>  | <ul><li>Identifiant de la touche à récupérer <a href="https://learn.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes">ici</a>.</li><li>Par exemple pour simuler la touche H c'est 0x48.</li></ul> |

## 🔙 Retour

| Type | Description |
| ---- | ----------- |
|      |             |
