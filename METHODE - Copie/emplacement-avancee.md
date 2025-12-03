# Emplacement avancée

Pour utiliser l'emplacement avancée en phase de préparation d'un combat, activez l'option :&#x20;

<figure><img src="https://3373271050-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-Mfulp0LhbJrdkH_fl5w%2Fuploads%2FGzSywtBhOp2Sxciq6RRE%2Fimage.png?alt=media&#x26;token=4965273d-df42-4eb1-befc-28153d9c1747" alt="" width="563"><figcaption></figcaption></figure>

Au moment de l'emplacement, la fonction <mark style="color:$primary;">fight\_placement()</mark> dans votre script sera appelée, et devra <mark style="color:$primary;">retourner la cellule</mark> où votre personnage doit se placer :&#x20;

* Voici le prototype de cette fonction :&#x20;

```lua
function fight_placement(possiblePositions, availablePositions)
    return CELL
end
```

* <mark style="color:$primary;">possiblePositions</mark> est une liste qui contient toutes les cellules possibles (vides + occupés).
* <mark style="color:$primary;">availablePositions</mark> est une liste qui contient toutes les cellules possibles vides.
* La fonction doit <mark style="color:$primary;">retourner la cellule</mark> où votre personnage doit se placer.
* Si la cellule retournée est -1, le personnage restera sur sa propre cellule.
* Si la cellule retournée est occupée, le personnage demandera un échange de position.
* Vous pouvez utiliser les méthodes des [combattants](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/methodes/combattants) et des [cellules](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/methodes/autres) pour construire votre logique et retourner une cellule.
