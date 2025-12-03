# pressInWindow

{% hint style="success" %}
Méthode permettant de simuler un appui de la souris sur une fenêtre spécifique.
{% endhint %}

## 🔍 Prototype

```lua
mouse.pressInWindow(hwnd, x, y, rightClick, ctrl, alt, shift)
```

## 📝 Paramètres

| Paramètre                    | Type                       | Description                                                                                                     |
| ---------------------------- | -------------------------- | --------------------------------------------------------------------------------------------------------------- |
| <ul><li>hwnd</li></ul>       | <ul><li>HWND</li></ul>     | <ul><li>Identifiant de la fenêtre à récupérer avec l'une des méthodes <a href="../window">window</a>.</li></ul> |
| <ul><li>x, y</li></ul>       | <ul><li>int, int</li></ul> | <ul><li>Les coordonnées du clique relatives à la fenêtre (et non pas à l'écran).</li></ul>                      |
| <ul><li>rightClick</li></ul> | <ul><li>bool</li></ul>     | <ul><li>false = clique gauche.</li><li>true = clique droit.</li></ul>                                           |
| <ul><li>ctrl</li></ul>       | <ul><li>bool</li></ul>     | <ul><li>Pour indiquer si la touche CTRL devrait être appuyée.</li></ul>                                         |
| <ul><li>alt</li></ul>        | <ul><li>bool</li></ul>     | <ul><li>Pour indiquer si la touche ALT devrait être appuyée.</li></ul>                                          |
| <ul><li>shift</li></ul>      | <ul><li>bool</li></ul>     | <ul><li>Pour indiquer si la touche SHIFT devrait être appuyée.</li></ul>                                        |

## 🔙 Retour

| Type | Description |
| ---- | ----------- |
|      |             |
