# addSpells

{% hint style="success" %}
Méthode permettant d'ajouter des sorts au combattant dans l'IA basique.
{% endhint %}

## 🔍 Prototype

```lua
basicFight.addSpells(spells)
```

## 📝 Paramètres

| Paramètre                | Type                                                                    | Description                                  |
| ------------------------ | ----------------------------------------------------------------------- | -------------------------------------------- |
| <ul><li>spells</li></ul> | <ul><li>Liste d'objets <a href="../../objets/spell">Spell</a></li></ul> | <ul><li>Liste des sorts à ajouter.</li></ul> |

## 🔙 Retour

| Type | Description |
| ---- | ----------- |
|      |             |

### <mark style="color:$primary;">Exemple d'utilisation</mark>

```lua
function fight_action()
  local spells = {
    {
      ["priority"] = 1,
      ["spell_id"] = 12744,
      ["target_type"] = enum_SpellTargetType.EnemyAdjacent,
      ["target_ids"] = "",
      ["life_condition"] = enum_LifeCondition.Greater,
      ["life_value"] = 1,
      ["starting_turn_condition"] = enum_TurnCondition.GreaterThanOrEqual,
      ["starting_turn"] = 2,
      ["starting_turn_mod"] = 4,
      ["every_x_turn"] = 1,
      ["repeat_max"] = 0,
      ["max_per_target"] = 0,
      ["hand_to_hand"] = enum_HandToHandType.Any,
      ["cast_distance_condition"] = enum_DistanceCondition.GreaterThanOrEqual,
      ["cast_distance"] = 2,
      ["target_vulnerable"] = true,
      ["target_invulnerable"] = true,
      ["target_invulnerable_melee"] = true,
      ["target_invulnerable_range"] = true,
      ["adjacent_type"] = enum_AdjacentType.Free,
    },
    {
      ["priority"] = 2,
      ["spell_id"] = 12728,
      ["target_type"] = enum_SpellTargetType.Enemy,
      ["target_ids"] = "494",
      ["life_condition"] = enum_LifeCondition.Greater,
      ["life_value"] = 3,
      ["starting_turn_condition"] = enum_TurnCondition.GreaterThanOrEqual,
      ["starting_turn"] = 2,
      ["starting_turn_mod"] = 4,
      ["every_x_turn"] = 1,
      ["repeat_max"] = 0,
      ["max_per_target"] = 0,
      ["hand_to_hand"] = enum_HandToHandType.Any,
      ["cast_distance_condition"] = enum_DistanceCondition.GreaterThanOrEqual,
      ["cast_distance"] = 2,
      ["target_vulnerable"] = true,
      ["target_invulnerable"] = true,
      ["target_invulnerable_melee"] = true,
      ["target_invulnerable_range"] = true,
      ["adjacent_type"] = enum_AdjacentType.Free,
    }
  }
  basicFight.clearSpells();
  basicFight.addSpells(spells)
  basicFight.play(false, enum_TacticType.Distance, enum_FocusType.Closest, enum_TacklePathType.AllPaths, 3)
end
```
