# dragAndDropInWindow

{% hint style="success" %}
Méthode permettant de simuler un glisser-déposer sur une fenêtre spécifique.
{% endhint %}

## 🔍 Prototype

```lua
mouse.dragAndDropInWindow(hwnd, from_x, from_y, to_x, to_y, ctrl, alt, shift)
```

## 📝 Paramètres

| Paramètre                          | Type                       | Description                                                                                                     |
| ---------------------------------- | -------------------------- | --------------------------------------------------------------------------------------------------------------- |
| <ul><li>hwnd</li></ul>             | <ul><li>HWND</li></ul>     | <ul><li>Identifiant de la fenêtre à récupérer avec l'une des méthodes <a href="../window">window</a>.</li></ul> |
| <ul><li>from\_x, from\_y</li></ul> | <ul><li>int, int</li></ul> | <ul><li>Les coordonnées du départ, relatives à la fenêtre (et non pas à l'écran).</li></ul>                     |
| <ul><li>to\_x, to\_y</li></ul>     | <ul><li>int, int</li></ul> | <ul><li>Les coordonnées de la fin, relatives à la fenêtre (et non pas à l'écran).</li></ul>                     |
| <ul><li>ctrl</li></ul>             | <ul><li>bool</li></ul>     | <ul><li>Pour indiquer si la touche CTRL devrait être appuyée.</li></ul>                                         |
| <ul><li>alt</li></ul>              | <ul><li>bool</li></ul>     | <ul><li>Pour indiquer si la touche ALT devrait être appuyée.</li></ul>                                          |
| <ul><li>shift</li></ul>            | <ul><li>bool</li></ul>     | <ul><li>Pour indiquer si la touche SHIFT devrait être appuyée.</li></ul>                                        |

## 🔙 Retour

| Type | Description |
| ---- | ----------- |
|      |             |
