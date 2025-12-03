# accessibleCells

{% hint style="success" %}
Méthode permettant de retourner la liste des [cellules accessibles](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/objets/accessiblecell) par un combattant.
{% endhint %}

## 🔍 Prototype

```lua
fight.accessibleCells(id)
```

## 📝 Paramètres

| Paramètre            | Type                                                                                                                                                                                                                                              | Description                                  |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| <ul><li>id</li></ul> | <ul><li>int</li><li>Ce paramètre est facultatif, s'il n'est pas défini, la valeur par défaut est <strong>l'</strong><a href="../combattants/currentfighterid"><strong>identifiant du combattant en train de jouer le tour</strong></a>.</li></ul> | <ul><li>Identifiant du combattant.</li></ul> |

## 🔙 Retour

| Type                                                                                       | Description                                                                                                      |
| ------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------- |
| <ul><li>Liste d'objets <a href="../../objets/accessiblecell">AccessibleCell</a>.</li></ul> | <ul><li>La liste des <a href="../../objets/accessiblecell">cellules accessibles</a> par le combattant.</li></ul> |
