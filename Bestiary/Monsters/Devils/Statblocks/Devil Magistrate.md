---
agility: 3
ancestry:
- Devil
- Infernal
ev: '32'
file_basename: Devil Magistrate
file_dpath: Monsters/Devils/Statblocks
free_strike: 7
intuition: 1
item_id: devil-magistrate
item_index: '300'
item_name: Devil Magistrate
level: 6
might: 1
presence: 2
reason: 0
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:devil-magistrate
scdc:
- 1.1.1:2:300
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '160'
type: monster
---

~~~ds-statblock
name: Devil Magistrate
level: 6
roles:
  - Elite Harrier
ancestry:
  - Devil
  - Infernal
ev: "32"
stamina: "160"
immunities:
  - Fire 5
speed: 7
size: 1M
stability: 0
free_strike: 7
might: 1
agility: 3
reason: 0
intuition: 1
presence: 2
traits:
  - name: Leading
    effects:
      - effect: Whenever the magistrate moves away from an enemy who is adjacent to one
          of the magistrate's allies, they can shift instead.
  - name: True Name
    effects:
      - effect: If a creature within 10 squares speaks the magistrate's true name, the
          magistrate loses their damage immunities, any nondamaging effects of
          their signature ability, and their Devilish Charm ability until the
          end of the encounter.
abilities:
  - name: Edge of the Law
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 10 damage
        t2: 15 damage
        t3: 18 fire damage; R < 3 dazed (save ends)
      - effect: The magistrate shifts up to 3 squares before or after using this
          ability, or between each strike.
        name: Effect
  - name: Verdict
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature
    effects:
      - effect: "**Power Roll + 3**"
        t1: 11 damage
        t2: 17 damage
        t3: 21 damage
      - effect: This ability has a double edge if the magistrate was hidden from the
          target, and deals an extra 5 damage if the target is dazed.
        name: Effect
  - name: Justice Turns Its Gaze
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The magistrate turns invisible until the start of their next turn, and
          can attempt to hide as a free maneuver before the end of the current
          turn.
        name: Effect
  - name: Devilish Charm
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    type: Triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature targets the magistrate with a strike.
    effects:
      - name: Effect
        effect: The target makes a Presence test
        t1: The magistrate chooses a new target for the strike.
        t2: The magistrate halves the triggering damage.
        t3: The target takes a bane on the strike.
~~~