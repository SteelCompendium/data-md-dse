---
agility: 2
ancestry:
- Dwarf
- Humanoid
ev: '6'
file_basename: Dwarf Reel Winch
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 3
intuition: 1
item_id: dwarf-reel-winch
item_index: '406'
item_name: Dwarf Reel Winch
level: 1
might: 0
presence: 0
reason: 0
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster:dwarf-reel-winch
scdc:
- 1.1.1:2:406
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '36'
type: monster
---

```ds-statblock
name: Dwarf Reel Winch
level: 1
roles:
  - Platoon Support
ancestry:
  - Dwarf
  - Humanoid
ev: "6"
stamina: "36"
speed: 5
size: 1M
stability: 2
free_strike: 3
might: 0
agility: 2
reason: 0
intuition: 1
presence: 0
traits:
  - name: We Have a Quota!
    effects:
      - effect: If a target made slowed by the reel winch is already grabbed or slowed,
          the grabbed and slowed conditions end and the target is restrained
          (save ends).
abilities:
  - name: Snaring Crossbow
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage; M < 0 slowed (save ends)
        t2: 7 damage; M < 1 slowed (save ends)
        t3: 9 damage; M < 2 slowed (save ends)
      - effect: The target is pulled up to 5 squares. A target restrained by a dwarf can
          be force moved by this ability. This forced movement doesn't end the
          restrained condition unless the Director determines otherwise.
  - name: Reel Them In
    cost: 3 Malice
    keywords:
      - Ranged
      - Weapon
    type: Maneuver
    distance: Ranged 10
    target: Three creatures
    effects:
      - effect: The target is pulled up to 8 squares. A restrained or slowed target can
          be pulled an additional 2 squares. A target restrained by a dwarf can
          be force moved by this ability. This forced movement doesn't end the
          restrained condition unless the Director determines otherwise.
```