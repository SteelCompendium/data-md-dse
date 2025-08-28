---
agility: 2
ancestry:
- Humanoid
- Orc
ev: '8'
file_basename: Orc Rampart
file_dpath: Monsters/Orcs/Statblocks
free_strike: 4
intuition: 2
item_id: orc-rampart
item_index: '134'
item_name: Orc Rampart
level: 2
might: 2
presence: 2
reason: 2
roles:
- Platoon Defender
scc:
- mcdm.monsters.v1:monster:orc-rampart
scdc:
- 1.1.1:2:134
size: 1L
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '59'
type: monster
---

```ds-statblock
name: Orc Rampart
level: 2
roles:
  - Platoon Defender
ancestry:
  - Humanoid
  - Orc
ev: "8"
stamina: "59"
speed: 6
size: 1L
stability: 2
free_strike: 4
might: 2
agility: 2
reason: 2
intuition: 2
presence: 2
traits:
  - name: Relentless
    effects:
      - effect: If the rampart is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the rampart is reduced to 1 Stamina instead.
abilities:
  - name: My Spear, My Foe
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 6 damage
        t2: 9 damage; taunted (EoT)
        t3: 12 damage; taunted (EoT)
      - effect: This ability has a double edge against any target who dealt damage to
          the rampart this round.
        name: Effect
  - name: Castling
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self; see below
    target: One ally
    effects:
      - effect: The rampart moves or shifts up to their speed adjacent to the target,
          then can swap places with the target.
        name: Effect
  - name: No.
    icon: ❗️
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: A creature targets an ally adjacent to the rampart with an ability that
      doesn't also target the rampart.
    effects:
      - effect: The rampart becomes the target of the triggering ability instead.
        name: Effect
```