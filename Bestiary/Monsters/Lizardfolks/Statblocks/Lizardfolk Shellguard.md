---
agility: 1
ancestry:
- Humanoid
- Lizardfolk
ev: 3 for four minions
file_basename: Lizardfolk Shellguard
file_dpath: Monsters/Lizardfolks/Statblocks
free_strike: 1
intuition: 0
item_id: lizardfolk-shellguard
item_index: '51'
item_name: Lizardfolk Shellguard
level: 1
might: 2
presence: 0
reason: 0
roles:
- Minion Defender
scc:
- mcdm.monsters.v1:monster:lizardfolk-shellguard
scdc:
- 1.1.1:2:51
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '6'
type: monster
---

~~~ds-statblock
name: Lizardfolk Shellguard
level: 1
roles:
  - Minion Defender
ancestry:
  - Humanoid
  - Lizardfolk
ev: 3 for four minions
stamina: "6"
speed: 5
movement: Swim
size: 1L
stability: 1
free_strike: 1
with_captain: +2 bonus to Stamina
might: 2
agility: 1
reason: 0
intuition: 0
presence: 0
traits:
  - name: Reptilian Escape
    effects:
      - effect: While the shellguard has a tail, whenever they are grabbed, prone,
          slowed, or weakened, they can lose their tail to immediately end that
          condition, then shift up to 2 squares.
abilities:
  - name: Shield Smash
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 1 damage
        t2: 2 damage
        t3: 3 damage
      - effect: The target takes a bane on their next strike.
        name: Effect
~~~