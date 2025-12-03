# Paramètres du script

### <mark style="color:$primary;">**MAX\_MONSTERS**</mark> <a href="#max_monsters" id="max_monsters"></a>

Pour définir le nombre **maximum** de monstres dans un groupe à combattre.

```lua
MAX_MONSTERS = 8
```

### <mark style="color:$primary;">**MIN\_MONSTERS**</mark> <a href="#min_monsters" id="min_monsters"></a>

Pour définir le nombre **minimum** de monstres dans un groupe à combattre.

```lua
MIN_MONSTERS = 2
```

### <mark style="color:$primary;">**FORBIDDEN\_MONSTERS**</mark> <a href="#forbidden_monsters" id="forbidden_monsters"></a>

Pour définir les monstres **interdits** dans un groupe à combattre.

Si l’un des monstres interdits est présent dans le groupe de monstre, alors le personnage ne le choisira pas.

```lua
FORBIDDEN_MONSTERS = { 5896, 4564 }
```

{% hint style="success" %}
Les identifiants sont ici : [cliquez-ici](https://www.frigost.dev/API/Dofus%203.0/Data/Monsters.json).
{% endhint %}

### <mark style="color:$primary;">**FORCE\_MONSTERS**</mark> <a href="#force_monsters" id="force_monsters"></a>

Pour définir les monstres **obligatoires** dans un groupe à combattre.

Si l’un des monstres obligatoires n’est pas présent dans le groupe de monstre, alors le personnage ne le choisira pas.

```lua
FORCE_MONSTERS = { 4845, 2321, 4236 }
```

{% hint style="success" %}
Les identifiants sont ici : [cliquez-ici](https://www.frigost.dev/API/Dofus%203.0/Data/Monsters.json).
{% endhint %}

Si l'Identifiant est négatif alors il correspond à l'ID du groupe (par exemple -20005).

### <mark style="color:$primary;">AMOUNT\_MONSTERS</mark> <a href="#amount_monsters" id="amount_monsters"></a>

Pour définir le nombre minimum et maximum de l'occurence d'un monstre dans un groupe de monstres.

* **Utilisation :**

```lua
AMOUNT_MONSTERS = { {id1, nbrMin1, nbrMax1}, {id2, nbrMin2, nbrMax2} }
```

{% hint style="success" %}
Les identifiants sont ici : [cliquez-ici](https://www.frigost.dev/API/Dofus%203.0/Data/Monsters.json).
{% endhint %}

* **Exemple :**

```lua
AMOUNT_MONSTERS = { {236, 2, 4}, {489, 4, 4} }
```

* 236 = l'ID du **piou violet**.
* 489 = l'ID du **piou rouge**.
* **Si** un groupe de monstre contient le **piou violet**, ce dernier ne sera lancé que s'il contient au moins **2 piou violet** et au plus **4 piou violet**.
* **Si** un groupe de monstre contient le **piou rouge**, ce dernier ne sera lancé que s'il contient exactement **4 piou rouge**.

### <mark style="color:$primary;">**GATHER**</mark> <a href="#gather" id="gather"></a>

Pour définir les éléments de récoltes que votre personnage pourra récolter (en négatif les éléments de récoltes que votre personnage ne doit pas récolter).

```lua
GATHER = { 254, 255, -67 }
```

{% hint style="success" %}
Les identifiants sont ici : [cliquez-ici](https://www.frigost.dev/API/Dofus%203.0/Data/Interactives.json).
{% endhint %}

### <mark style="color:$primary;">**AUTO\_DELETE**</mark> <a href="#auto_delete" id="auto_delete"></a>

Pour définir les objets qui devront être supprimés lorsque le pourcentage de retour en banque est atteint.

```lua
AUTO_DELETE = { 156, 5478, 546, 1221 }
```

{% hint style="success" %}
Les identifiants sont ici : [cliquez-ici](https://www.frigost.dev/API/Dofus%203.0/Data/Items.json).
{% endhint %}

<mark style="color:$primary;">Frigost</mark> supprimera les objets demandés lorsque le pourcentage de retour en banque est atteint.

Si, après la suppression, le personnage est toujours au dessus ou égal au pourcentage, Frigost lira la fonction <mark style="color:$primary;">bank()</mark> afin de vider l'inventaire.

### <mark style="color:$primary;">**PLANNING**</mark> <a href="#planning" id="planning"></a>

Pour définir les heures de déconnexion pour votre personnage.

Les heures sont comprises entre 0 et 23 inclus.

```lua
PLANNING = { 1, 2, 4, 20, 21, 22 }
```

### <mark style="color:$primary;">TEAM\_MEMBER\_LOST\_INTERVAL</mark>

En groupe, le chef vérifie régulièrement si tous les membres sont présents dans la meme carte, ce paramètre contrôle l'interval de vérification.

```lua
TEAM_MEMBER_LOST_INTERVAL = 10
```

Ici par exemple, le chef va vérifier la présence des membres chaque 10 secondes, si l'un des membres n'est pas présent, la fonction [team\_member\_lost()](https://doc.frigost.dev/abonnement-frigost-bot/syntaxe-du-script) sera exécutée.

Si ce paramètre n'est pas définie, la valeur par défaut est 60s.
