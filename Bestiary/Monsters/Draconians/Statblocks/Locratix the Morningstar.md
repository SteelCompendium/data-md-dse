---
agility: 3
ancestry:
- Draconian
- Dragon
- Humanoid
ev: '32'
file_basename: Locratix the Morningstar
file_dpath: Monsters/Draconians/Statblocks
free_strike: 7
intuition: 2
item_id: locratix-the-morningstar
item_index: '105'
item_name: Locratix the Morningstar
level: 6
might: 1
presence: 2
reason: 1
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:locratix-the-morningstar
scdc:
- 1.1.1:2:105
size: 1M
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '160'
type: monster
---

```ds-statblock
name: Locratix the Morningstar
level: 6
roles:
  - Elite Harrier
ancestry:
  - Draconian
  - Dragon
  - Humanoid
ev: "32"
stamina: "160"
immunities:
  - Acid 6
speed: 8
movement: Fly
size: 1M
stability: 2
free_strike: 7
might: 1
agility: 3
reason: 1
intuition: 2
presence: 2
traits:
  - name: Flighty
    effects:
      - effect: When Locratix deals rolled damage to an enemy, that enemy can't use
          Locratix as the trigger for any of their triggered actions until the
          start of Locratix's next turn.
  - name: Absorbing Scales
    effects:
      - effect: When Locratix takes damage of any type for which she has damage
          immunity, she has damage immunity 6 against the next strike made
          against her.
abilities:
  - name: Skewer
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 1 10 damage
        t2: 2 15 damage; M < 1 slowed (save ends)
        t3: 3 18 damage; M < 2 slowed (save ends)
      - effect: Locratix deals 6 damage to each creature or object in a 2 x 1 line
          behind the target.
        name: Effect
  - name: Acidic Stun
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 3 x 1 line within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 7 acid damage; M < 1 dazed (save ends)
        t2: 12 acid damage; M < 2 dazed (save ends)
        t3: 15 acid damage; M < 3 dazed (save ends)
      - effect: While dazed this way, a target takes an extra 6 damage from Locratix's
          abilities.
        name: Effect
  - name: Takeoff
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: Locratix flies up to her speed. Any creature adjacent to the space on
          the ground she took off from who has A < 2 is knocked prone.
        name: Effect
  - name: Stay Back!
    icon: ❗️
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 2
    target: The triggering creature
    trigger: A creature within distance moves or is forced moved.
    effects:
      - roll: Power Roll + 3
        t1: 7 acid damage; A < 1 the target's speed is 0 (EoT)
        t2: 12 acid damage; A < 2 the target's speed is 0 (EoT)
        t3: 15 acid damage; A < 3 the target's speed is 0 (EoT)
```