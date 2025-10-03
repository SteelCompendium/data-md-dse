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
item_index: '293'
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
- 1.1.1:2:293
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '300'
type: monster
---

~~~ds-statblock
type: statblock
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
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the hag can take 5 damage to end one
          effect on them that can be ended by a saving throw. This damage can't
          be reduced in any way.
      - name: Solo Turns
        effect: The hag can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Supernatural Resistance
    icon: ⭐️
    effects:
      - effect: Magic and psionic abilities used against the hag take a bane.
  - type: feature
    feature_type: ability
    name: Corrosive Claws
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
      - roll: Power Roll + 3
        tier1: 9 corruption damage; A < 1 weakened (save ends)
        tier2: 13 corruption damage; A < 2 weakened (save ends)
        tier3: 16 corruption damage; A < 3 weakened (save ends)
  - type: feature
    feature_type: ability
    name: Soul Steal
    icon: 🔳
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 4 cube within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 corruption damage; P < 1 4 corruption damage
        tier2: 8 corruption damage; P < 2 5 corruption damage
        tier3: 10 corruption damage; P < 3 6 corruption damage
      - name: Effect
        effect: This ability gains an edge against a target who has a soul.
      - cost: 3 Malice
        effect: The hag regains Stamina equal to half the damage dealt.
  - type: feature
    feature_type: ability
    name: Shapeshifter
    icon: 👤
    keywords:
      - Magic
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The hag alters their body to become any size 1 creature, from a house
          cat to a humanoid. If the hag uses this ability while outside of any
          enemy's line of effect, they can choose to be automatically hidden.
          The hag can return to their original form as a free maneuver.
      - cost: 5 Malice
        effect: The hag becomes a size 2 creature instead, from a bear to an ogre. While
          in this form, the hag's melee abilities gain a +1 bonus to distance
          and deal an extra 4 damage.
  - type: feature
    feature_type: ability
    name: Turned Upside Down
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Area
      - Magic
    usage: Triggered action
    distance: 1 burst
    target: Each enemy in the area
    trigger: A creature targets the hag with a melee strike.
    effects:
      - roll: Power Roll + 3
        tier1: Slide 2; R < 1 the slide is vertical
        tier2: Slide 3; R < 2 the slide is vertical, and the target is restrained (EoT)
        tier3: Vertical slide 5; R < 3 restrained (EoT)
      - name: Effect
        effect: While restrained this way, a creature who is vertical force moved is
          suspended in midair. The creature falls when the condition ends.
  - type: feature
    feature_type: ability
    name: Snackies for Sweeties
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 5 burst
    target: Each creature in the area
    effects:
      - name: Effect
        effect: The hag attaches an ornate explosive pastry to each target who has A <
          2. At the end of the round, the hag makes one power roll against each
          creature with a pastry attached to them.
      - roll: Power Roll + 3
        tier1: 6 poison damage
        tier2: 10 poison damage
        tier3: 13 poison damage
      - name: Special
        effect: A creature wearing a pastry or adjacent to a creature wearing a pastry
          can attempt an **Agility test** to remove the pastry as a maneuver.
        tier1: The hag makes the power roll for all pastries.
        tier2: The pastry is not removed.
        tier3: The pastry is removed and can no longer explode.
  - type: feature
    feature_type: ability
    name: Predator's Alacrity
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
      - Weapon
    usage: "-"
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Before using this villain action, the hag shifts up to their speed. They
          then use Corrosive Claws against each target, push each target up to 2
          squares, and shift up to their speed again.
  - type: feature
    feature_type: ability
    name: Open the Oven
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Weapon
    usage: "-"
    distance: 5 cube within 1
    target: Each creature in the area
    effects:
      - roll: Power Roll + 3
        tier1: 6 fire damage; A < 1 weakened (save ends)
        tier2: 10 fire damage; A < 2 weakened (save ends)
        tier3: 13 fire damage; A < 3 weakened (save ends)
      - name: Effect
        effect: The hag turns the area into a roiling oven until the end of the
          encounter. Any creature in area takes an extra 5 damage from the hag's
          damage-dealing abilities.
~~~