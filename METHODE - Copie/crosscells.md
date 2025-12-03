# crossCells

{% hint style="success" %}
Méthode permettant de récupérer la liste des cellules formant une croix autour d'un centre, avec un rayon minimal et et un rayon maximal.

* Cette méthode ne vérifie pas que les cellules retournées contiennent un obstacle ou un autre combattant.
  {% endhint %}

## 🔍 Prototype

```lua
fight.crossCells(centerCellId, minRadius, maxRadius)
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

<figure><img src="https://3373271050-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-Mfulp0LhbJrdkH_fl5w%2Fuploads%2FrB5ZtiA2w42FwrcpWPIP%2Fimage.png?alt=media&#x26;token=d0151740-8831-4afc-8e18-50630a12095a" alt=""><figcaption></figcaption></figure>
