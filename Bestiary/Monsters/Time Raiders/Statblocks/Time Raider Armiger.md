---
agility: 2
ancestry:
- Humanoid
- Time Raider
ev: '10'
file_basename: Time Raider Armiger
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 5
intuition: 2
item_id: time-raider-armiger
item_index: '141'
item_name: Time Raider Armiger
level: 3
might: 0
presence: 0
reason: 2
roles:
- Platoon Defender
scc:
- mcdm.monsters.v1:monster:time-raider-armiger
scdc:
- 1.1.1:2:141
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '60'
type: monster
---

```ds-statblock
name: Time Raider Armiger
level: 3
roles:
  - Platoon Defender
ancestry:
  - Humanoid
  - Time Raider
ev: "10"
stamina: "60"
immunities:
  - Psychic 3
speed: 5
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 2
reason: 2
intuition: 2
presence: 0
traits:
  - name: Foresight
    effects:
      - effect: The armiger doesn't take a bane on strikes against creatures with
          concealment.
  - name: Kuran'zoi Heraldry
    effects:
      - effect: Any time raider who starts their turn with line of effect to the armiger
          can end one condition affecting the.
abilities:
  - name: Serrated Saber
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 7 damage
        t2: 10 damage
        t3: 13 damage; R < 2 weakened (save ends)
      - effect: A creature weakened this way is also bleeding.
        cost: 2 Malice
  - name: Shared Sickness
    icon: ❗️
    keywords:
      - Psionic
      - Ranged
    type: Triggered action
    distance: Ranged 20
    target: The triggering creature
    trigger: A creature deals damage to any ally of the armiger who the armiger has
      line of effect to
    effects:
      - roll: Power Roll + 2
        t1: 4 psychic damage; R < 0 5 poison damage
        t2: 6 psychic damage; R < 1 5 poison damage
        t3: 9 psychic damage; R < 2 5 poison damage
```