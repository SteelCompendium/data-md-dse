---
agility: 2
ancestry:
- Human
- Humanoid
ev: '12'
file_basename: Human Blackguard
file_dpath: Monsters/Humans/Statblocks
free_strike: 4
intuition: 0
item_id: human-blackguard
item_index: '166'
item_name: Human Blackguard
level: 1
might: 3
presence: 2
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:human-blackguard
scdc:
- 1.1.1:2:166
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '80'
type: monster
---

```ds-statblock
name: Human Blackguard
level: 1
roles:
  - Leader
ancestry:
  - Human
  - Humanoid
ev: "12"
stamina: "80"
immunities:
  - Corruption 2
  - psychic 2
speed: 5
size: 1M
stability: 2
free_strike: 4
might: 3
agility: 2
reason: 2
intuition: 0
presence: 2
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the blackguard can take 5 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - name: Supernatural Insight
    effects:
      - effect: The blackguard ignores concealment if it's granted by a supernatural
          effect
abilities:
  - name: Zweihander Swing
    icon: ❇️
    cost: Signature Ability
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 3 damage; M < 1 slowed (save ends)
        t2: 6 damage; M < 2 slowed (save ends)
        t3: 8 damage; M < 3 slowed (save ends)
      - effect: One ally within 10 squares can make a free strike.
        name: Effect
      - effect: One ally within 10 squares can use their signature ability instead.
        cost: 1 Malice
  - name: You!
    icon: 🏹
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One enemy
    effects:
      - effect: The target is marked until the start of the blackguard's next turn. The
          blackguard and each of their allies gain an edge on abilities used
          against targets marked by the blackguard.
        name: Effect
  - name: Parry!
    icon: ❗️
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 1
    target: Self or one ally
    trigger: A creature makes a strike against the blackguard or an ally adjacent to
      them.
    effects:
      - effect: The damage is halved.
        name: Effect
  - name: Advance!
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: The blackguard shifts up to their speed. During or after this movement,
          they can use their Zweihander Swing twice.
        name: Effect
  - name: Back!
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - effect: The blackguard slides each target up to 5 squares.
        name: Effect
  - name: I Can Throw My Blade and So Should You!
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
      - Ranged
      - Weapon
    type: "-"
    distance: 3 cube within 5
    target: Each enemy in the area
    effects:
      - effect: The blackguard uses their Zweihander Swing against each target. Each
          ally within 5 squares of the area can then make a free strike against
          a target (one target per ally)
        name: Effect
```