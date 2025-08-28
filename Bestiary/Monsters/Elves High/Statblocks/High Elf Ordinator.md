---
agility: 2
ancestry:
- Fey
- High Elf
- Humanoid
ev: '20'
file_basename: High Elf Ordinator
file_dpath: Monsters/Elves High/Statblocks
free_strike: 5
intuition: 2
item_id: high-elf-ordinator
item_index: '114'
item_name: High Elf Ordinator
level: 3
might: 0
presence: 3
reason: 3
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:high-elf-ordinator
scdc:
- 1.1.1:2:114
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '120'
type: monster
---

~~~ds-statblock
name: High Elf Ordinator
level: 3
roles:
  - Leader
ancestry:
  - Fey
  - High Elf
  - Humanoid
ev: "20"
stamina: "120"
speed: 5
movement: Fly
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 2
reason: 3
intuition: 2
presence: 3
traits:
  - name: Otherworldly Blessing
    effects:
      - effect: At the start of each of their turns, the ordinator can choose one or
          more effects on them that can be ended by a saving throw. The effects
          instead end at the end of the ordinator's turn
abilities:
  - name: Lightning Rod
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 9 lightning damage; R < 1 dazed (save ends)
        t2: 14 lightning damage; R < 2 dazed (save ends)
        t3: 17 lightning damage; R < 3 dazed (save ends)
      - effect: Until the start of the ordinator's next turn, each ally high elf in the
          encounter gains an edge on ability rolls against the target.
        name: Effect
  - name: Elemental Uproar
    icon: ❇️
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 10 burst
    target: Each elemental ally in the area
    effects:
      - effect: Each target can move up to their speed or make a free strike. Elemental
          mote targets can, instead, use their Spark of Life trait.
        name: Effect
  - name: Summon Elemental
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: Special
    effects:
      - effect: The ordinator summons four elemental motes or four soot crows into
          unoccupied space within distance.
        name: Effect
      - effect: The ordinator instead summons one ceramic horse or one winded
          brambleguard into an unoccupied space within distance.
        cost: 3 Malice
  - name: Enough!
    icon: ❗️
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering enemy
    trigger: An enemy within distance uses an ability against the ordinator or any
      ally within distance.
    effects:
      - effect: The ordinator uses Lightning Rod against the target after the ability is
          resolved.
        name: Effect
  - name: Fountains Roar, Now Free From the Earth
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - effect: Each target glows briefly, and can end one effect on themself then move
          up to their speed.
        name: Effect
  - name: And the Sun Forsook Her Children
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
      - Magic
      - Ranged
    type: "-"
    distance: 5 cube within 10
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target makes a **Presence test**.
        t1: 12 corruption damage; pull 5 toward the center of the cube
        t2: 9 corruption damage; pull 3 toward the center of the cube
        t3: Pull 1 toward the center of the cube
      - effect: The area turns dark and distorted, and is difficult terrain for enemies.
        name: Effect
  - name: But We Will Change Her Mind
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 10 burst
    target: Self and each ally in the area
    effects:
      - effect: Each target's free strike now has the Magic keyword and can target two
          creatures or objects. Additionally, each target glows with magic.
        name: Effect
~~~