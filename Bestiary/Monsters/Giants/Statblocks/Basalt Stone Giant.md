---
agility: 2
ancestry:
- Giant
- Stone Giant
ev: '40'
file_basename: Basalt Stone Giant
file_dpath: Monsters/Giants/Statblocks
free_strike: 8
intuition: 2
item_id: basalt-stone-giant
item_index: '196'
item_name: Basalt Stone Giant
level: 8
might: 4
presence: 1
reason: 1
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:basalt-stone-giant
scdc:
- 1.1.1:2:196
size: '4'
source: mcdm.monsters.v1
speed: 7
stability: 10
stamina: '207'
type: monster
---

~~~ds-statblock
type: statblock
name: Basalt Stone Giant
level: 8
roles:
  - Elite Controller
ancestry:
  - Giant
  - Stone Giant
ev: "40"
stamina: "207"
speed: 7
movement: Burrow
size: "4"
stability: 10
free_strike: 8
might: 4
agility: 2
reason: 1
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Rune-Signed Blade
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 12 damage; M < 2 slowed (save ends)
        tier2: 17 damage; M < 3 slowed (save ends)
        tier3: 21 damage; M < 4 slowed (save ends)
      - name: Effect
        effect: If a target was already slowed, that condition continues but their speed
          is 0 until the end of their next turn.
  - type: feature
    feature_type: ability
    name: Forked Knife
    icon: ⚔️
    cost: 3 Malice
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3 or ranged 12
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 10 damage; A < 2 restrained (save ends)
        tier2: 16 damage; A < 3 restrained (save ends)
        tier3: 20 damage; prone; A < 4 restrained (save ends)
      - name: Effect
        effect: The knife lands in the target's square, and has 30 Stamina and damage
          immunity 5. Whenever the knife takes damage, it deals 4 sonic damage
          to each enemy within 3 squares. The knife lasts until the end of the
          encounter, and can't be picked up or manipulated.
  - type: feature
    feature_type: ability
    name: Cobblestone Shape
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The basalt stone giant moves up to their speed. Each square that they
          leave during this move is difficult terrain for enemies. Giants ignore
          this difficult terrain.
  - type: feature
    feature_type: ability
    name: Resonate Rune
    icon: ❗️
    keywords:
      - Area
      - Magic
    usage: Triggered action
    distance: 2 burst
    target: Each enemy in the area
    trigger: The basalt stone giant takes damage.
    effects:
      - name: Effect
        effect: The target is pushed up to 3 squares, or if they have A < 3, they are
          pushed up to 6 squares and knocked prone.
  - type: feature
    feature_type: trait
    name: Stonebreaker Flesh
    icon: ⭐️
    effects:
      - effect: Whenever an enemy obtains a tier 1 outcome on a melee ability used
          against the basalt stone giant, they take a bane on that ability until
          the end of the encounter.
  - type: feature
    feature_type: trait
    name: Stone Steps
    icon: ⭐️
    effects:
      - effect: The basalt stone giant ignores difficult terrain
  - type: feature
    feature_type: trait
    name: Stone Swim
    icon: ⭐️
    effects:
      - effect: The basalt stone giant can burrow through stone, but can't drag other
          creatures underground when they do so.
~~~