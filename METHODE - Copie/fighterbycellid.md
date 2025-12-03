# fighterByCellId

{% hint style="success" %}
Méthode permettant de retourner l'objet [Fighter](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/objets/fighter) représentant un combattant.
{% endhint %}

## 🔍 Prototype

```lua
fight.fighterByCellId(cellId)
```

## 📝 Paramètres

| Paramètre                | Type                  | Description                              |
| ------------------------ | --------------------- | ---------------------------------------- |
| <ul><li>cellId</li></ul> | <ul><li>int</li></ul> | <ul><li>Cellule du combattant.</li></ul> |

## 🔙 Retour

| Type                                                         | Description                                                                                    |
| ------------------------------------------------------------ | ---------------------------------------------------------------------------------------------- |
| <ul><li><a href="../../objets/fighter">Fighter</a></li></ul> | <ul><li>Objet <a href="../../objets/fighter">Fighter</a> représentant le combattant.</li></ul> |
| <ul><li>nil</li></ul>                                        | <ul><li>Si introuvable.</li></ul>                                                              |
