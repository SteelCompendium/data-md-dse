---
agility: 1
ancestry:
- Giant
- Troll
ev: 11 for four minions
file_basename: Troll Crack Trooper
file_dpath: Monsters/Trolls/Statblocks
free_strike: 5
intuition: 0
item_id: troll-crack-trooper
item_index: '410'
item_name: Troll Crack Trooper
level: 9
might: 4
presence: 2
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:troll-crack-trooper
scdc:
- 1.1.1:2:410
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 4
stamina: '15'
type: monster
---

```ds-statblock
name: Troll Crack Trooper
level: 9
roles:
  - Minion Brute
ancestry:
  - Giant
  - Troll
ev: 11 for four minions
stamina: "15"
weaknesses:
  - Acid 5
  - fire
speed: 6
size: "2"
stability: 4
free_strike: 5
with_captain: +3 bonus to Stamina
might: 4
agility: 1
reason: -1
intuition: 0
presence: 2
traits:
  - name: Group Appetite
    effects:
      - effect: The crack trooper dies only if their squad's Stamina pool is reduced to
          0 Stamina by acid or fire damage, if they end their turn with 0
          Stamina in their squad's Stamina pool, or if they take acid or fire
          damage while their squad's Stamina pool is at 0 Stamina.
abilities:
  - name: Charging Chomp
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        t1: 5 damage; push 2
        t2: 7 damage; push 3; A < 3 3 damage
        t3: 9 damage; push 4; A < 4 5 damage
      - effect: The crack trooper's squad's Stamina pool regains Stamina equal to half
          the damage dealt.
```