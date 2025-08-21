---
agility: 3
ancestry:
- Horror
- Voiceless Talker
ev: '32'
file_basename: Voiceless Talker Artillerist
file_dpath: Monsters/Voiceless Talkers/Statblocks
free_strike: 7
intuition: 2
item_id: voiceless-talker-artillerist
item_index: '342'
item_name: Voiceless Talker Artillerist
level: 6
might: 0
presence: 1
reason: 3
roles:
- Elite Artillery
scc:
- mcdm.monsters.v1:monster:voiceless-talker-artillerist
scdc:
- 1.1.1:2:342
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '140'
type: monster
---

```ds-statblock
name: Voiceless Talker Artillerist
level: 6
roles:
  - Elite Artillery
ancestry:
  - Horror
  - Voiceless Talker
ev: "32"
stamina: "140"
immunities:
  - Psychic 6
speed: 5
movement: Hover, teleport
size: 1M
stability: 2
free_strike: 7
might: 0
agility: 3
reason: 3
intuition: 2
presence: 1
traits:
  - name: Psionic Conductor
    effects:
      - effect: Whenever a non-minion voiceless talker within 5 squares of the
          artillerist uses a psionic ability, they can do so as if they were in
          the artillerist's space.
  - name: Locked On
    effects:
      - effect: The artillerist ignores invisibility, cover, and concealment. A creature
          can't hide from the artillerist while the artillerist has line of
          effect to the.
abilities:
  - name: Psionic Rifle Burst
    cost: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 11 damage
        t2: 19 damage; the strike spreads 1 square
        t3: 22 damage; the strike spreads 2 squares
      - effect: The strike's spread is the distance it expands from a target to nearby
          enemies. Each enemy within that distance takes 3 damage.
        name: Effect
      - effect: Each enemy within the strike spread takes an extra 3 damage.
        cost: 2 Malice
  - name: Mind Jolt
    keywords:
      - Area
      - Psionic
    type: Main action
    distance: 10 x 1 line within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 6 lightning damage
        t2: 10 lightning damage; I < 2 slowed (save ends)
        t3: 13 lightning damage; I < 3 slowed (save ends)
  - name: In Our Sights
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One creature
    effects:
      - effect: Until the start of the artillerist's next turn, the next psionic ability
          used against the target automatically treats its initial power roll as
          a 17. The creature using the ability can still roll to determine if
          they score a critical hit.
        name: Effect
  - name: Tactical Reposition
    cost: 1 Malice
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The artillerist takes damage.
    effects:
      - effect: The artillerist can teleport up to 5 squares and ignores any effects
          associated with the damage
        name: Effect
```