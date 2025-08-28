---
agility: 2
ancestry:
- Human
- Humanoid
ev: '6'
file_basename: Human Scoundrel
file_dpath: Monsters/Humans/Statblocks
free_strike: 4
intuition: 0
item_id: human-scoundrel
item_index: '163'
item_name: Human Scoundrel
level: 1
might: 0
presence: 1
reason: 0
roles:
- Platoon Ambusher
scc:
- mcdm.monsters.v1:monster:human-scoundrel
scdc:
- 1.1.1:2:163
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

~~~ds-statblock
name: Human Scoundrel
level: 1
roles:
  - Platoon Ambusher
ancestry:
  - Human
  - Humanoid
ev: "6"
stamina: "30"
immunities:
  - Corruption 1
  - psychic 1
speed: 5
size: 1M
stability: 0
free_strike: 4
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Supernatural Insight
    effects:
      - effect: The scoundrel ignores concealment if it's granted by a supernatural
          effect.
abilities:
  - name: Rapier and Dagger
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
        t2: 9 damage
        t3: 12 damage
      - effect: If this ability gains an edge or has a double edge, it deals an extra 2
          damage.
        cost: 2 Malice
  - name: Dagger Storm
    icon: 🌀
    cost: 5 Malice
    keywords:
      - "-"
    type: Main action
    distance: "-"
    target: "-"
    effects:
      - effect: The scoundrel uses Rapier and Dagger against up to three targets. They
          shift up to 2 squares before or after each strike
~~~