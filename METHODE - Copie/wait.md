# wait

{% hint style="success" %}
Méthode permettant de mettre en pause le script jusqu'à ce qu'un pixel atteigne (ou cesse d'avoir) une couleur spécifique.
{% endhint %}

{% hint style="danger" %}
Ne pas réduire la fenêtre en question sinon cette méthode ne marchera pas.
{% endhint %}

## 🔍 Prototype

```lua
pixel.wait(x, y, color, equal, timeout, step)
```

## 📝 Paramètres

| Paramètre                 | Type                       | Description                                                                                                                                                           |
| ------------------------- | -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li>x, y</li></ul>    | <ul><li>int, int</li></ul> | <ul><li>Les coordonnées du pixel relatives à la fenêtre (et non pas à l'écran).</li></ul>                                                                             |
| <ul><li>color</li></ul>   | <ul><li>string</li></ul>   | <ul><li>La couleur sous la forme "#XXXXXX".</li></ul>                                                                                                                 |
| <ul><li>equal</li></ul>   | <ul><li>bool</li></ul>     | <ul><li>true = attendre que la couleur du pixel devient <code>color</code>.</li><li>false = attendre que la couleur du pixel n'est plus <code>color</code>.</li></ul> |
| <ul><li>timeout</li></ul> | <ul><li>int</li></ul>      | <ul><li>Durée maximal à attendre, 0 = infini.</li></ul>                                                                                                               |
| <ul><li>step</li></ul>    | <ul><li>int</li></ul>      | <ul><li>Par exemple si step est 100, la fonction va vérifier le pixel chaque 100ms, mettre une valeur très basse peut augmenter la consommation du CPU.</li></ul>     |

## 🔙 Retour

| Type                   | Description                                                                       |
| ---------------------- | --------------------------------------------------------------------------------- |
| <ul><li>bool</li></ul> | <ul><li>true = succès.</li><li>false = le timeout est écoulé ou erreur.</li></ul> |
