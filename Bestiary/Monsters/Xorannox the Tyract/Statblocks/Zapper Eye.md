---
agility: 1
ancestry:
- Eyestalk
- Horror
- Overmind
ev: '-'
file_basename: Zapper Eye
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 3
intuition: 1
item_id: zapper-eye
item_index: '316'
item_name: Zapper Eye
level: 6
might: -1
presence: -1
reason: 4
roles:
- Artillery
scc:
- mcdm.monsters.v1:monster:zapper-eye
scdc:
- 1.1.1:2:316
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: Zapper Eye
level: 6
roles:
  - Artillery
ancestry:
  - Eyestalk
  - Horror
  - Overmind
ev: "-"
stamina: "30"
speed: 5
movement: Fly, hover
size: 1M
stability: 0
free_strike: 3
might: -1
agility: 1
reason: 4
intuition: 1
presence: -1
traits:
  - name: Psionic Barrier
    effects:
      - effect: The zapper eye has damage immunity 15. When they use a main action, they
          lose this immunity until the end of the round.
  - name: Gas Belch
    effects:
      - effect: Xorannox lets out a noxious belch. Each enemy within 2 squares of him
          who has M < 3 is weakened (save ends).
  - name: Slime Trail
    effects:
      - effect: Until the end of Xorannox's next turn, whenever he or any of his eyes
          leave their space, they secrete a viscous slime onto the ground in
          that area. Any enemy who enters an affected square has lightning
          weakness 5 and fire weakness 5 until the end of the encounter.
  - name: Solo Action
    effects:
      - effect: Xorannox takes an additional main action on his turn. He can use this
          feature even if he is dazed.
  - name: Mind Over Matter
    effects:
      - effect: Xorannox fills the encounter map with a powerful telekinetic field. The
          Director chooses a cardinal direction (north, south, east, or west).
          Whenever a creature in the encounter willingly moves or is force
          moved, they are pulled 2 squares in the chosen direction, ignoring
          stability. Each time this feature is used, its previous effect ends.
abilities:
  - name: Lightning Beam
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Psionic
    type: Main action
    distance: 10 x 1 line within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 6 lightning damage
        t2: 10 lightning damage
        t3: 13 lightning damage
      - effect: Each target loses all their surges.
        name: Effect
```