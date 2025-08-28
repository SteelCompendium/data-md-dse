---
agility: 1
ancestry:
- Draconian
- Dragon
- Humanoid
ev: '32'
file_basename: Dorzinuuth the Base
file_dpath: Monsters/Draconians/Statblocks
free_strike: 7
intuition: 2
item_id: dorzinuuth-the-base
item_index: '101'
item_name: Dorzinuuth the Base
level: 6
might: 4
presence: 3
reason: 1
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:dorzinuuth-the-base
scdc:
- 1.1.1:2:101
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '180'
type: monster
---

```ds-statblock
name: Dorzinuuth the Base
level: 6
roles:
  - Leader
ancestry:
  - Draconian
  - Dragon
  - Humanoid
ev: "32"
stamina: "180"
immunities:
  - Lightning 6
speed: 5
movement: Fly, hover
size: "2"
stability: 3
free_strike: 7
might: 4
agility: 1
reason: 1
intuition: 2
presence: 3
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of his turns, Dorzinuuth can take 10 damage to end
          one effect on him that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - name: Remember Your Oath
    effects:
      - effect: If Dorzinuuth hears a creature recite the Dragon Phalanx oath, he takes
          a bane on strikes made against that character until the end of the
          encounter.
  - name: Sheltering Wings
    effects:
      - effect: While Dorzinuuth isn't flying, strikes made against him take a bane.
abilities:
  - name: Punishing Flail
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
      - roll: Power Roll + 4
        t1: 11 damage; M < 2 prone
        t2: 16 damage; M < 3 prone
        t3: 19 damage; M < 4 prone
      - effect: If the target has M < 4, they are also bleeding (save ends).
        cost: 2 Malice
  - name: I'll Cut A Path
    icon: 🔳
    keywords:
      - Area
      - Weapon
    type: Maneuver
    distance: 5 x 2 line within 1
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Before the power roll is made, Dorzinuuth shifts to an unoccupied space
          adjacent to the end of the line.
      - roll: Power Roll + 4
        t1: 7 damage
        t2: 13 damage; M < 3 prone
        t3: 15 damage; M < 4 prone
  - name: Watch Your Six!
    icon: ❗️
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 1
    target: One ally
    trigger: An ally within distance takes damage while Dorzinuuth isn't flying.
    effects:
      - effect: Dorzinuuth shields the triggering ally with his wings, halving the
          damage.
        name: Effect
  - name: Roaring Gambit
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Dorzinuuth lets loose a powerful roar. Each target makes a **Reason
          test**.
        t1: Frightened (save ends)
        t2: Frightened (EoT)
        t3: No effect.
      - effect: Each ally in the area gains an edge on their next strike.
        name: Effect
  - name: Wings of Second Wind
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Self and each ally in the area
    effects:
      - effect: Each target shifts or flies up to their speed and regains 10 Stamina.
        name: Effect
  - name: Snap, Crackle, Pop
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each ally in the area
    effects:
      - effect: Dorzinuuth covers the targets in an electrifying mesh. Whenever a target
          takes damage from a melee ability, the attacker takes 6 lightning
          damage.
        name: Effect
```