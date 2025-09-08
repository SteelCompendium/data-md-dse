---
agility: 2
ancestry:
- Devil
- Infernal
ev: '28'
file_basename: Devil Jurist
file_dpath: Monsters/Devils/Statblocks
free_strike: 7
intuition: 1
item_id: devil-jurist
item_index: '301'
item_name: Devil Jurist
level: 5
might: 0
presence: 3
reason: 1
roles:
- Elite Artillery
scc:
- mcdm.monsters.v1:monster:devil-jurist
scdc:
- 1.1.1:2:301
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '120'
type: monster
---

~~~ds-statblock
name: Devil Jurist
level: 5
roles:
  - Elite Artillery
ancestry:
  - Devil
  - Infernal
ev: "28"
stamina: "120"
immunities:
  - Fire 5
speed: 6
movement: Fly
size: 1M
stability: 0
free_strike: 7
might: 0
agility: 2
reason: 1
intuition: 1
presence: 3
traits:
  - name: Hellfire
    effects:
      - effect: Fire damage dealt by the jurist ignores damage immunity.
  - name: True Name
    effects:
      - effect: If a creature within 10 squares speaks the jurist's true name, the
          jurist loses their fire immunity, any nondamaging effects of their
          signature ability, and their Devilish Charm ability until the end of
          the encounter.
abilities:
  - name: Fire and Brimstone
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 12
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 10 fire damage
        t2: 15 fire damage; A < 2 burning (save ends)
        t3: 18 fire damage; A < 3 burning (save ends)
      - effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
        name: Effect
      - effect: The jurist can target one additional creature or object for each Malice
          spent.
        cost: 1+ Malice
  - name: Dismissal with Prejudice
    icon: ❇️
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - effect: "**Power Roll + 3**"
        t1: 6 damage; slide 1
        t2: 10 damage; slide 3
        t3: 12 damage; slide 5
      - effect: If the target has M < 2, the forced distance movement gains a +3 bonus.
        name: Effect
  - name: Ashes to Ashes
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 12
    target: One creature
    effects:
      - effect: If the target is burning (see Fire and Brimstone), they take 6 fire
          damage.
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
    trigger: A creature targets the jurist with a strike.
    effects:
      - name: Effect
        effect: The target makes a Presence test
        t1: The jurist chooses a new target for the strike.
        t2: The jurist halves the triggering damage.
        t3: The target takes a bane on the strike.
~~~