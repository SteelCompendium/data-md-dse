---
agility: 1
ancestry:
- Giant
- Ogre
ev: 9 for four minions
file_basename: Ogre Blue Blood
file_dpath: Monsters/Ogres/Statblocks
free_strike: 4
intuition: 0
item_id: ogre-blue-blood
item_index: '04'
item_name: Ogre Blue Blood
level: 7
might: 4
presence: 2
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:ogre-blue-blood
scdc:
- 1.1.1:2:04
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '13'
type: monster
---

```ds-statblock
name: Ogre Blue Blood
level: 7
roles:
  - Minion Brute
ancestry:
  - Giant
  - Ogre
ev: 9 for four minions
stamina: "13"
speed: 5
size: "2"
stability: 4
free_strike: 4
with_captain: Gain an edge on strikes
might: 4
agility: 1
reason: -1
intuition: 0
presence: 2
traits:
  - name: In My Stead
    effects:
      - effect: Whenever the blue blood would make a free strike, an ally within 5
          squares can make a free strike instead.
  - name: Royal Anger
    effects:
      - effect: The blue blood has damage immunity 2 while their squad has three or
          fewer minions in it.
abilities:
  - name: Crush Underfoot
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        t1: 4 damage
        t2: 7 damage; M < 3 prone
        t3: 8 damage; prone
      - effect: A target who is already prone takes an extra 4 damage.
        name: Effect
```