---
agility: 1
ancestry:
- Devil
- Infernal
ev: '32'
file_basename: Devil Adjudicator
file_dpath: Monsters/Devils/Statblocks
free_strike: 7
intuition: 1
item_id: devil-adjudicator
item_index: '297'
item_name: Devil Adjudicator
level: 6
might: 0
presence: 3
reason: 2
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:devil-adjudicator
scdc:
- 1.1.1:2:297
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 1
stamina: '140'
type: monster
---

```ds-statblock
name: Devil Adjudicator
level: 6
roles:
  - Elite Controller
ancestry:
  - Devil
  - Infernal
ev: "32"
stamina: "140"
immunities:
  - Fire 5
speed: 6
movement: Fly
size: 1M
stability: 1
free_strike: 7
might: 0
agility: 1
reason: 2
intuition: 1
presence: 3
traits:
  - name: Vexatious Litigation
    effects:
      - effect: Any creature within 10 squares of the adjudicator who has P < 3 takes a
          −2 penalty to saving throws.
  - name: True Name
    effects:
      - effect: If a creature within 10 squares speaks the adjudicator's true name, the
          adjudicator loses their damage immunities, any nondamaging effects of
          their signature ability, and their Devilish Charm ability until the
          end of the encounter.
abilities:
  - name: Infernal Injunction
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 10 fire damage; I < 1 frightened (save ends)
        t2: 15 fire damage; I < 1 frightened (save ends)
        t3: 18 fire damage; I < 1 frightened (save ends)
      - effect: The adjudicator can slide a target frightened by this ability up to 2
          squares.
        name: Effect
  - name: Adjudicator's Interdiction
    keywords:
      - Magic
      - Ranged
    type: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - name: Effect
        effect: The target makes a Presence test
        t1: The target is slowed, takes a bane on power rolls, and can't regain Stamina
          (save ends).
        t2: The target is slowed and takes a bane on power rolls (save ends).
        t3: Slowed (save ends)
  - name: Quid Pro Quo
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One ally or frightened creature
    effects:
      - effect: The adjudicator and the target teleport to switch places.
        name: Effect
  - name: Devilish Charm
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    type: Triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature targets the adjudicator with a strike.
    effects:
      - effect: The target makes a Presence test
        name: Effect
```