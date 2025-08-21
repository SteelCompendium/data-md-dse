---
agility: 3
ancestry:
- Human
- Humanoid
ev: '20'
file_basename: Human Bandit Chief
file_dpath: Monsters/Humans/Statblocks
free_strike: 5
intuition: 3
item_id: human-bandit-chief
item_index: '165'
item_name: Human Bandit Chief
level: 3
might: 2
presence: 2
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:human-bandit-chief
scdc:
- 1.1.1:2:165
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '120'
type: monster
---

```ds-statblock
name: Human Bandit Chief
level: 3
roles:
  - Leader
ancestry:
  - Human
  - Humanoid
ev: "20"
stamina: "120"
immunities:
  - Corruption 4
  - psychic 4
speed: 5
size: 1M
stability: 2
free_strike: 5
might: 2
agility: 3
reason: 2
intuition: 3
presence: 2
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the bandit chief can take 5 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - name: Supernatural Insight
    effects:
      - effect: The bandit chief ignores concealment if it's granted by a supernatural
          effect
abilities:
  - name: Whip and Magic Longsword
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two enemies or objects
    effects:
      - roll: Power Roll + 2
        t1: 8 damage; pull 1
        t2: 12 damage; pull 2
        t3: 15 damage; pull 3
      - effect: Any target who is adjacent to the bandit chief after the power roll is
          resolved takes 3 corruption damage.
        name: Effect
      - effect: This ability targets one additional target.
        cost: 2 Malice
  - name: Kneel, Peasant!
    keywords:
      - Melee
    type: Maneuver
    distance: Melee 1
    target: One enemy
    effects:
      - cost: ≤11
        effect: Push 1; M < 1 prone
        t2: Push 2; M < 2 prone
        t3: Push 4; M < 3 prone
      - effect: The ability takes the Area keyword, loses the Melee keyword, and is a 1
          burst that targets each enemy in the area.
        cost: 2 Malice
  - name: Bloodstones
    keywords:
      - Magic
    type: Triggered action
    distance: Self
    target: Self
    trigger: The bandit chief makes a power roll.
    effects:
      - effect: The bandit chief takes 5 corruption damage and increases the outcome of
          the power roll by one tier. This damage can't be reduced in any way.
        name: Effect
  - name: Shoot!
    cost: Villain Action 1
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Each artillery ally in the area
    effects:
      - effect: Each target makes a ranged free strike.
        name: Effect
  - name: Form Up!
    cost: Villain Action 2
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - effect: Each target shifts up to their speed. Additionally, until the end of the
          encounter, while the bandit chief or any ally is adjacent to a target,
          they have damage immunity 2.
        name: Effect
  - name: Lead From the Front
    cost: Villain Action 3
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: The bandit chief shifts up to 10 squares regardless of their speed.
          During or after this movement, they can use their Whip and Magic
          Longsword against up to four targets. Additionally, one ally adjacent
          to each target can make a free strike against that target.
        name: Effect
```