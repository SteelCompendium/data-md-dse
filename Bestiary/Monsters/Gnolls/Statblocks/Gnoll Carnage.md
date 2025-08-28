---
agility: 3
ancestry:
- Abyssal
- Gnoll
ev: '16'
file_basename: Gnoll Carnage
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 5
intuition: 0
item_id: gnoll-carnage
item_index: '38'
item_name: Gnoll Carnage
level: 2
might: 3
presence: 3
reason: 0
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:gnoll-carnage
scdc:
- 1.1.1:2:38
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '100'
type: monster
---

```ds-statblock
name: Gnoll Carnage
level: 2
roles:
  - Leader
ancestry:
  - Abyssal
  - Gnoll
ev: "16"
stamina: "100"
speed: 5
size: 1M
stability: 1
free_strike: 5
might: 3
agility: 3
reason: 0
intuition: 0
presence: 3
traits:
  - name: Death Rampage
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the carnage is reduced to
          0 Stamina, the carnage can move up to their speed, then can either
          make a melee free strike against two creatures or use Shrapnel Whip
          against one creature.
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the carnage can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - name: Endless Hunger
    effects:
      - effect: If the carnage is reduced to 0 Stamina while there are still gnolls on
          the encounter map, one gnoll on the map is transformed into a gnoll
          carnage, keeping their current Stamina.
abilities:
  - name: Shrapnel Whip
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 8 damage; A < 1 bleeding (save ends)
        t2: 11 damage; A < 2 bleeding (save ends)
        t3: 14 damage; A < 3 bleeding and dazed (save ends)
      - effect: An ally targeted by this ability ignores the damage and can make a free
          strike.
        name: Effect
  - name: Carnage's Cackletongue
    icon: ❇️
    cost: 4 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 5 burst
    target: Self and each ally in the area
    effects:
      - effect: Each target deals an extra 3 damage with their next strike until the
          start of the carnage's next turn. If any target hasn't used their own
          Cackletongue maneuver on this turn, they can use it immediately at no
          cost.
        name: Effect
  - name: Call Up From the Abyss
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Magic
      - Ranged
    type: "-"
    distance: Ranged 10
    target: Special
    effects:
      - effect: The carnage summons four abyssal hyenas into unoccupied spaces within
          distance.
        name: Effect
  - name: Edacity
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Self and three allies
    effects:
      - effect: Each target moves up to their speed and can make a free strike. Any
          creature damaged by one of these free strikes who has M < 2 is knocked
          prone.
        name: Effect
  - name: Deepest Wounds
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each winded enemy in the area
    effects:
      - name: Effect
        effect: The carnage's eyes and all exposed blood within distance glow bright
          red. Each target makes a **Presence test**.
        t1: The target can't regain Stamina until the end of the encounter.
        t2: The target can't regain Stamina (save ends).
        t3: No effect
      - effect: Until the end of the encounter, all gnolls have a double edge on power
          rolls that target a winded enemy.
        name: Effect
```