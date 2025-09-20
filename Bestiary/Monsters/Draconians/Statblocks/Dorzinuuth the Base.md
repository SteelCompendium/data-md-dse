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

~~~ds-statblock
type: statblock
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
features:
  - type: feature
    feature_type: ability
    name: Punishing Flail
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 11 damage; M < 2 prone
        tier2: 16 damage; M < 3 prone
        tier3: 19 damage; M < 4 prone
      - cost: 2 Malice
        effect: If the target has M < 4, they are also bleeding (save ends).
  - type: feature
    feature_type: ability
    name: I'll Cut A Path
    icon: 🔳
    keywords:
      - Area
      - Weapon
    usage: Maneuver
    distance: 5 x 2 line within 1
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Before the power roll is made, Dorzinuuth shifts to an unoccupied space
          adjacent to the end of the line.
      - roll: Power Roll + 4
        tier1: 7 damage
        tier2: 13 damage; M < 3 prone
        tier3: 15 damage; M < 4 prone
  - type: feature
    feature_type: ability
    name: Watch Your Six!
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 1
    target: One ally
    trigger: An ally within distance takes damage while Dorzinuuth isn't flying.
    effects:
      - name: Effect
        effect: Dorzinuuth shields the triggering ally with his wings, halving the
          damage.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of his turns, Dorzinuuth can take 10 damage to end
          one effect on him that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - type: feature
    feature_type: trait
    name: Remember Your Oath
    icon: ⭐️
    effects:
      - effect: If Dorzinuuth hears a creature recite the Dragon Phalanx oath, he takes
          a bane on strikes made against that character until the end of the
          encounter.
  - type: feature
    feature_type: trait
    name: Sheltering Wings
    icon: ⭐️
    effects:
      - effect: While Dorzinuuth isn't flying, strikes made against him take a bane.
  - type: feature
    feature_type: ability
    name: Roaring Gambit
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Dorzinuuth lets loose a powerful roar. Each target makes a **Reason
          test**.
        tier1: Frightened (save ends)
        tier2: Frightened (EoT)
        tier3: No effect.
      - name: Effect
        effect: Each ally in the area gains an edge on their next strike.
  - type: feature
    feature_type: ability
    name: Wings of Second Wind
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Each target shifts or flies up to their speed and regains 10 Stamina.
  - type: feature
    feature_type: ability
    name: Snap, Crackle, Pop
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 5 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: Dorzinuuth covers the targets in an electrifying mesh. Whenever a target
          takes damage from a melee ability, the attacker takes 6 lightning
          damage.
~~~