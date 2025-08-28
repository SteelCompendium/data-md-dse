---
agility: 2
ancestry:
- Humanoid
- Kobold
ev: '3'
file_basename: Kobold Venator
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 2
intuition: 0
item_id: kobold-venator
item_index: '93'
item_name: Kobold Venator
level: 1
might: 0
presence: 1
reason: 0
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster:kobold-venator
scdc:
- 1.1.1:2:93
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '15'
type: monster
---

```ds-statblock
name: Kobold Venator
level: 1
roles:
  - Horde Ambusher
ancestry:
  - Humanoid
  - Kobold
ev: "3"
stamina: "15"
speed: 5
size: 1S
stability: 0
free_strike: 2
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Lost in the Crowd
    effects:
      - effect: While the venator is adjacent to any ally who is not hiding, the venator
          can attempt to hide as if they had concealment, even if observed.
  - name: Not What I Seem
    effects:
      - effect: The venator starts the encounter disguised as a minion. They have a
          double edge on their first main action of the encounter, after which
          they reveal themself.
  - name: Shield? Shield!
    effects:
      - effect: While adjacent to an ally who also has this trait, the venator has
          stability 1, has cover, and grants cover to allies.
abilities:
  - name: Dolabra and Net
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
        t1: 4 damage
        t2: 6 damage; M < 1 restrained (save ends)
        t3: 7 damage; M < 2 restrained (save ends)
      - effect: The venator lights their net on fire, and a target restrained this way
          takes 2 fire damage at the start of each of their turns.
        cost: 3 Malice
```