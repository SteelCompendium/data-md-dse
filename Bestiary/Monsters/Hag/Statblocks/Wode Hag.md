---
agility: 1
ancestry:
- Fey
- Hag
ev: '60'
file_basename: Wode Hag
file_dpath: Monsters/Hag/Statblocks
free_strike: 6
intuition: 3
item_id: wode-hag
item_index: '295'
item_name: Wode Hag
level: 3
might: 2
presence: 3
reason: 1
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:wode-hag
scdc:
- 1.1.1:2:295
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '300'
type: monster
---

```ds-statblock
name: Wode Hag
level: 3
roles:
  - Solo
ancestry:
  - Fey
  - Hag
ev: "60"
stamina: "300"
speed: 5
movement: Fly, hover
size: 1L
stability: 1
free_strike: 6
might: 2
agility: 1
reason: 1
intuition: 3
presence: 3
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the hag can take 5 damage to end one
          effect on them that can be ended by a saving throw. This damage can't
          be reduced in any way.
        name: End Effect
      - effect: The hag can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Supernatural Resistance
    effects:
      - effect: Magic and psionic abilities used against the hag take a bane.
abilities:
  - name: Corrosive Claws
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
        t1: 9 corruption damage; A < 1 weakened (save ends)
        t2: 13 corruption damage; A < 2 weakened (save ends)
        t3: 16 corruption damage; A < 3 weakened (save ends)
  - name: Soul Steal
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 4 cube within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 5 corruption damage; P < 1 4 corruption damage
        t2: 8 corruption damage; P < 2 5 corruption damage
        t3: 10 corruption damage; P < 3 6 corruption damage
      - effect: This ability gains an edge against a target who has a soul.
        name: Effect
      - effect: The hag regains Stamina equal to half the damage dealt.
        cost: 3 Malice
  - name: Shapeshifter
    keywords:
      - Magic
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The hag alters their body to become any size 1 creature, from a house
          cat to a humanoid. If the hag uses this ability while outside of any
          enemy's line of effect, they can choose to be automatically hidden.
          The hag can return to their original form as a free maneuver.
        name: Effect
      - effect: The hag becomes a size 2 creature instead, from a bear to an ogre. While
          in this form, the hag's melee abilities gain a +1 bonus to distance
          and deal an extra 4 damage.
        cost: 5 Malice
  - name: Turned Upside Down
    cost: 2 Malice
    keywords:
      - Area
      - Magic
    type: Triggered action
    distance: 1 burst
    target: Each enemy in the area
    trigger: A creature targets the hag with a melee strike.
    effects:
      - roll: Power Roll + 3
        t1: Slide 2; R < 1 the slide is vertical
        t2: Slide 3; R < 2 the slide is vertical, and the target is restrained (EoT)
        t3: Vertical slide 5; R < 3 restrained (EoT)
      - effect: While restrained this way, a creature who is vertical force moved is
          suspended in midair. The creature falls when the condition ends.
        name: Effect
  - name: Snackies for Sweeties
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each creature in the area
    effects:
      - name: Effect
        effect: The hag attaches an ornate explosive pastry to each target who has A <
          2. At the end of the round, the hag makes one power roll against each
          creature with a pastry attached to them.
      - roll: Power Roll + 3
        t1: 6 poison damage
        t2: 10 poison damage
        t3: 13 poison damage
      - name: Special
        effect: A creature wearing a pastry or adjacent to a creature wearing a pastry
          can attempt an **Agility test** to remove the pastry as a maneuver.
        t1: The hag makes the power roll for all pastries.
        t2: The pastry is not removed.
        t3: The pastry is removed and can no longer explode.
  - name: Predator's Alacrity
    cost: Villain Action 2
    keywords:
      - Area
      - Weapon
    type: "-"
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - effect: Before using this villain action, the hag shifts up to their speed. They
          then use Corrosive Claws against each target, push each target up to 2
          squares, and shift up to their speed again
        name: Effect
  - name: Open the Oven
    cost: Villain Action 3
    keywords:
      - Area
      - Weapon
    type: "-"
    distance: 5 cube within 1
    target: Each creature in the area
    effects:
      - roll: Power Roll + 3
        t1: 6 fire damage; A < 1 weakened (save ends)
        t2: 10 fire damage; A < 2 weakened (save ends)
        t3: 13 fire damage; A < 3 weakened (save ends)
      - effect: The hag turns the area into a roiling oven until the end of the
          encounter. Any creature in area takes an extra 5 damage from the hag's
          damage-dealing abilities.
        name: Effect
```