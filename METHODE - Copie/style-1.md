# Style 1

Au <mark style="color:$primary;">début du tour</mark> du combattant, et après <mark style="color:$primary;">chaque action</mark> (sort ou déplacement), la fonction <mark style="color:$primary;">fight\_action()</mark> dans votre script sera appelée.

C'est dans cette fonction que vous devez construire votre logique avec les [méthodes de l'IA avancée](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/methodes), et effectuer l'une des [actions](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/methodes/actions) :&#x20;

* Lancer un sort.
* Effectuer un déplacement.
* Passer le tour.
* Abandonner le combat.
* Jouer avec l'[IA basique](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/methodes/ia-basique).

Voici les méthodes disponibles pour effectuer ces actions :&#x20;

{% content-ref url="../methodes/actions" %}
[actions](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/methodes/actions)
{% endcontent-ref %}

Quand l'une de ces [méthodes](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/methodes/actions) est appelée, le personnage effectue l'action, et l'exécution de la fonction <mark style="color:$primary;">fight\_action()</mark> est interrompu, pour mieux comprendre ça, voici un exemple :

```lua
function fight_action()
	console.print("Hello") 	-- "Hello" est affiché dans la console.
	fight.finishTurn() 	-- Passe le tour et interrompt l'exécution.
	console.print("Hey") 	-- "Hey" n'est pas affiché dans la console.
end
```

Si l'exécution de la fonction <mark style="color:$primary;">fight\_action()</mark> se termine sans aucune [action](https://doc.frigost.dev/abonnement-frigost-bot/ia-avancee-de-combat/methodes/actions), le personnage ne fait rien.

### <mark style="color:$primary;">Exemple</mark>

```lua
function fight_action()

	-- Afficher
	console.print("Round: "..fight.currentRound())
	console.print("Action: "..fight.currentAction())

	-- Récupérer mon combattant
	local me = fight.currentFighter()

	-- Récupérer l'ennemi le plus proche
	local nearestEnemy = fight.nearestEnemy()

	-- S'approcher de l'ennemi
	fight.moveTowardCell(nearestEnemy.cellId)

	-- Lancer le sort "Stase" sur l'ennemi
	if fight.canCastSpell(12728, me.cellId, nearestEnemy.cellId) == enum_SpellCastError.NoError then
		fight.castSpell(12728, nearestEnemy.cellId)
	end

	-- Passer le tour
	fight.finishTurn()
end
```
