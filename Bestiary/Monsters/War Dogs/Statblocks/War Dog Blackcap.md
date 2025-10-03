---
agility: 4
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '9'
file_basename: War Dog Blackcap
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 4
intuition: 2
item_id: war-dog-blackcap
item_index: '373'
item_name: War Dog Blackcap
level: 7
might: 1
presence: 0
reason: 4
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster:war-dog-blackcap
scdc:
- 1.1.1:2:373
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '45'
type: monster
---

~~~ds-statblock
type: statblock
name: War Dog Blackcap
level: 7
roles:
  - Horde Ambusher
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "9"
stamina: "45"
speed: 6
movement: Teleport
size: 1M
stability: 0
free_strike: 4
might: 1
agility: 4
reason: 4
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Flesh-Eater Knife
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 8 damage
        tier2: 11 damage
        tier3: 12 damage; M < 4 bleeding and weakened (save ends)
      - name: Effect
        effect: The blackcap can teleport up to their speed before using this ability,
          creating an ash clone (see below) in their original square.
  - type: feature
    feature_type: ability
    name: Ashes to Ashes
    icon: 🏹
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 20
    target: Up to three ash clones
    effects:
      - name: Effect
        effect: Each target makes a free strike.
  - type: feature
    feature_type: trait
    name: Ash Clones
    icon: ⭐️
    effects:
      - effect: An ash clone created by the blackcap has the blackcap's statistics but
          has 1 Stamina. Ash clones don't take turns in combat, but they can act
          when the blackcap allows them to and can move when the blackcap
          willingly moves.
  - type: feature
    feature_type: trait
    name: Duplicating Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the blackcap or any of their ash clones is reduced to 0 Stamina,
          that creature's loyalty collar explodes, dealing 3d6 poison damage to
          each adjacent enemy and object. If any adjacent enemy has A < 3 they
          are also weakened (save ends)
~~~