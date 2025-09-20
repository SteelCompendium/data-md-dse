---
agility: 3
ancestry:
- Horror
- Voiceless Talker
ev: '32'
file_basename: Voiceless Talker Artillerist
file_dpath: Monsters/Voiceless Talkers/Statblocks
free_strike: 7
intuition: 2
item_id: voiceless-talker-artillerist
item_index: '342'
item_name: Voiceless Talker Artillerist
level: 6
might: 0
presence: 1
reason: 3
roles:
- Elite Artillery
scc:
- mcdm.monsters.v1:monster:voiceless-talker-artillerist
scdc:
- 1.1.1:2:342
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '140'
type: monster
---

~~~ds-statblock
type: statblock
name: Voiceless Talker Artillerist
level: 6
roles:
  - Elite Artillery
ancestry:
  - Horror
  - Voiceless Talker
ev: "32"
stamina: "140"
immunities:
  - Psychic 6
speed: 5
movement: Hover, teleport
size: 1M
stability: 2
free_strike: 7
might: 0
agility: 3
reason: 3
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Psionic Rifle Burst
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 11 damage
        tier2: 19 damage; the strike spreads 1 square
        tier3: 22 damage; the strike spreads 2 squares
      - name: Effect
        effect: The strike's spread is the distance it expands from a target to nearby
          enemies. Each enemy within that distance takes 3 damage.
      - cost: 2 Malice
        effect: Each enemy within the strike spread takes an extra 3 damage.
  - type: feature
    feature_type: ability
    name: Mind Jolt
    icon: 🔳
    keywords:
      - Area
      - Psionic
    usage: Main action
    distance: 10 x 1 line within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 6 lightning damage
        tier2: 10 lightning damage; I < 2 slowed (save ends)
        tier3: 13 lightning damage; I < 3 slowed (save ends)
  - type: feature
    feature_type: ability
    name: In Our Sights
    icon: 🏹
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: One creature
    effects:
      - name: Effect
        effect: Until the start of the artillerist's next turn, the next psionic ability
          used against the target automatically treats its initial power roll as
          a 17. The creature using the ability can still roll to determine if
          they score a critical hit.
  - type: feature
    feature_type: ability
    name: Tactical Reposition
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The artillerist takes damage.
    effects:
      - name: Effect
        effect: The artillerist can teleport up to 5 squares and ignores any effects
          associated with the damage
  - type: feature
    feature_type: trait
    name: Psionic Conductor
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion voiceless talker within 5 squares of the
          artillerist uses a psionic ability, they can do so as if they were in
          the artillerist's space.
  - type: feature
    feature_type: trait
    name: Locked On
    icon: ⭐️
    effects:
      - effect: The artillerist ignores invisibility, cover, and concealment. A creature
          can't hide from the artillerist while the artillerist has line of
          effect to the.
~~~