# setObjectPosition

{% hint style="success" %}
Méthode permettant de changer la position (équiper ou déséquiper) un objet.
{% endhint %}

## 🔍 Prototype

```lua
inventory.setObjectPosition(gid, new_position)
```

## 📝 Paramètres

| Paramètre                       | Type                  | Description                                                                                                         |
| ------------------------------- | --------------------- | ------------------------------------------------------------------------------------------------------------------- |
| <ul><li>gid</li></ul>           | <ul><li>int</li></ul> | <ul><li>Identifiant <a href="https://www.frigost.dev/API/Dofus%203.0/Data/Items.json">GID</a> de l'objet.</li></ul> |
| <ul><li>new\_position</li></ul> | <ul><li>int</li></ul> | <ul><li>La nouvelle position.</li></ul>                                                                             |

## 🔙 Retour

| Type | Description |
| ---- | ----------- |
|      |             |

{% hint style="success" %}
Rendez-vous sur [cette page](https://www.frigost.dev/API/Dofus%203.0/Data/) pour récupérer des identifiants.
{% endhint %}

### Tableau des positions :

| Emplacement         | Position |
| ------------------- | :------: |
| Amulette            |     0    |
| Arme                |     1    |
| Anneau (gauche)     |     2    |
| Ceinture            |     3    |
| Anneau (droite)     |     4    |
| Bottes              |     5    |
| Chapeau             |     6    |
| Cape                |     7    |
| Familier            |     8    |
| Trophée / Dofus  1  |     9    |
| Trophée / Dofus 2   |    10    |
| Trophée / Dofus 3   |    11    |
| Trophée / Dofus 4   |    12    |
| Trophée / Dofus 5   |    13    |
| Trophée / Dofus 6   |    14    |
| Bouclier            |    15    |
| Monture             |    16    |
| Mutation            |    20    |
| Boost (Consommable) |    21    |
| Bonus 1             |    22    |
| Bonus 2             |    23    |
| Malus 1             |    24    |
| Malus 2             |    25    |
| Buff (Rôle-Play)    |    26    |
| Entité suiveuse     |    27    |
| Entité              |    28    |
| Harnachement        |    29    |
| Costume             |    30    |
| Non équipé          |    63    |
