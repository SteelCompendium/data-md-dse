---
agility: 1
ancestry:
- Soulless
- War Dog
ev: '48'
file_basename: Logostician Vesper
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 10
intuition: 4
item_id: logostician-vesper
item_index: '394'
item_name: Logostician Vesper
level: 10
might: 2
presence: 1
reason: 5
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:logostician-vesper
scdc:
- 1.1.1:2:394
size: '2'
source: mcdm.monsters.v1
speed: 10
stability: 3
stamina: '253'
type: monster
---

~~~ds-statblock
type: statblock
name: Logostician Vesper
level: 10
roles:
  - Elite Controller
ancestry:
  - Soulless
  - War Dog
ev: "48"
stamina: "253"
speed: 10
size: "2"
stability: 3
free_strike: 10
might: 2
agility: 1
reason: 5
intuition: 4
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Portal to the Firing Line
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Main action
    distance: 5 x 3 line within 15
    target: Each creature and object in the area
    effects:
      - name: Special
        effect: This ability targets only non-prone creatures.
      - roll: Power Roll + 5
        tier1: 8 damage
        tier2: 12 damage; I < 4 slowed (save ends)
        tier3: 15 damage; I < 5 slowed (save ends)
      - name: Effect
        effect: A target creature can choose to drop prone, in which case the ability
          takes a bane against them.
      - cost: 2 Malice
        effect: The area remains active until Vesper is reduced to 0 Stamina or until
          the end of the encounter. Any non-prone enemy who enters the area for
          the first time in a round or starts their turn there takes 15 damage,
          or 7 damage if they choose to fall prone.
  - type: feature
    feature_type: ability
    name: Portal to the Mantle
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main action
    distance: 3 cube within 15
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 5
        tier1: 8 fire damage
        tier2: 12 fire damage
        tier3: 15 fire damage
      - name: Effect
        effect: The area is difficult terrain. Any creature who enters the area for the
          first time in a round or starts their turn there takes 10 fir damage.
          Until the end of the encounter, the size of the area increases by 1 at
          the start of each round.
  - type: feature
    feature_type: ability
    name: Portal to the Void
    icon: 🔳
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Maneuver
    distance: 5 cube within 15
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 5
        tier1: A < 4 pull 3 toward the center of the area
        tier2: A < 5 pull 3 toward the center of the area
        tier3: Pull 3 toward the center of the area
      - name: Effect
        effect: A portal appears at the center of the area. Any creature at the center
          of the area when this ability is used or who is pulled into the center
          for the first time in a round takes 10 sonic damage.
      - cost: 2 Malice
        effect: The area remains active and deals its damage until Vesper is reduced to
          0 Stamina or until the end of the encounter. Any creature who enters
          the area and has A < 4 is pulled 3 squares toward the center of the
          area. Any creature who starts their turn in the area and has M < 4 is
          slowed until the end of their turn.
  - type: feature
    feature_type: ability
    name: Portal to the Sky
    icon: ❗️
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 3
    target: One enemy
    trigger: The target moves within distance of Vesper.
    effects:
      - name: Effect
        effect: The target is dropped through a portal, which teleports them up to 7
          squares above a space within 15 squares.
  - type: feature
    feature_type: trait
    name: Living Logistics Network
    icon: ⭐️
    effects:
      - effect: Each ally who starts their turn within 10 squares of Vesper can teleport
          whenever they willingly move until the end of their turn. Whenever an
          affected ally teleports, they deal an extra 5 damage on their next
          strike.
  - type: feature
    feature_type: trait
    name: Crash and Burn
    icon: ⭐️
    effects:
      - effect: When Vesper is reduced to 0 Stamina, they move up to their speed and
          then explode, dealing 4d6 damage to each adjacent enemy and object.
          Any enemy who takes more than 14 damage this way vertically slides 5
          squares.
~~~