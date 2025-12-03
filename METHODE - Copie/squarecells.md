# squareCells

{% hint style="success" %}
Méthode permettant de récupérer la liste des cellules formant un carré autour d'un centre, avec un rayon minimal et et un rayon maximal.

* Cette méthode ne vérifie pas que les cellules retournées contiennent un obstacle ou un autre combattant.
  {% endhint %}

## 🔍 Prototype

```lua
fight.squareCells(centerCellId, minRadius, maxRadius)
```

## 📝 Paramètres

| Paramètre                      | Type                  | Description                         |
| ------------------------------ | --------------------- | ----------------------------------- |
| <ul><li>centerCellId</li></ul> | <ul><li>int</li></ul> | <ul><li>Le centre.</li></ul>        |
| <ul><li>minRadius</li></ul>    | <ul><li>int</li></ul> | <ul><li>Le rayon minimal.</li></ul> |
| <ul><li>maxRadius</li></ul>    | <ul><li>int</li></ul> | <ul><li>La rayon maximal.</li></ul> |

## 🔙 Retour

| Type                           | Description                           |
| ------------------------------ | ------------------------------------- |
| <ul><li>Liste de int</li></ul> | <ul><li>Liste des cellules.</li></ul> |

<figure><img src="https://3373271050-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-Mfulp0LhbJrdkH_fl5w%2Fuploads%2F6xrhzClrjNYgDdRzmQHb%2Fimage.png?alt=media&#x26;token=136f5cdc-5a3a-4933-81c0-1f95e967906a" alt=""><figcaption></figcaption></figure>
