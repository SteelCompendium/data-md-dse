---
agility: 2
ancestry:
- Accursed
- Humanoid
- Werebeast
ev: '36'
file_basename: Werewolf
file_dpath: Monsters/Werewolf/Statblocks
free_strike: 5
intuition: 1
item_id: werewolf
item_index: '335'
item_name: Werewolf
level: 1
might: 3
presence: 1
reason: -1
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:werewolf
scdc:
- 1.1.1:2:335
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '200'
type: monster
---

~~~ds-statblock
type: statblock
name: Werewolf
level: 1
roles:
  - Solo
ancestry:
  - Accursed
  - Humanoid
  - Werebeast
ev: "36"
stamina: "200"
speed: 7
size: 1M
stability: 0
free_strike: 5
might: 3
agility: 2
reason: -1
intuition: 1
presence: 1
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the werewolf can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
      - name: Solo Turns
        effect: The werewolf can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Accursed Rage
    icon: ⭐️
    effects:
      - effect: The werewolf's ferocity is expressed through rage, and their abilities
          can inflict rage points on any enemy except a stormwight fury. A
          creature who starts their turn with 10 or more rage expends their
          rage. Then before taking their turn, they must shift up to their speed
          toward the nearest creature and make a melee free strike against them.
          A creature who takes damage from this free strike gains 1 rage.
          Accumulated rage disappears after a character finishes a respite
  - type: feature
    feature_type: trait
    name: Shapeshifter
    icon: ⭐️
    effects:
      - effect: The werewolf enters combat in their hybrid humanoid form. Their shape
          can't be changed by any external effect
  - type: feature
    feature_type: trait
    name: Vukenstep
    icon: ⭐️
    effects:
      - effect: The werewolf ignores difficult terrain
  - type: feature
    feature_type: ability
    name: Accursed Bite
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 9 damage; the target gains 2 rage
        tier2: 13 damage; the target gains 4 rage
        tier3: 16 damage; the target gains 5 rage
      - cost: 2 Malice
        effect: "If the target has P < 0, they are afflicted with lycanthpy. Each time
          the target is unaffected by the potency effect, the potency increases
          by 1 the next time the werewolf uses the ability against the same
          target. A creature afflicted with lycanthrop gains 2 rage at the end
          of each of their turns whenever they're in combat. Their rage doesn't
          disappear after finishing a respite and they must complete the Find a
          Cure downtime project in \"Draw Steel: Heroes\" to end this effect"
  - type: feature
    feature_type: ability
    name: Ripping Claws
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 8 damage; M < 1 bleeding (save ends)
        tier2: 11 damage; the target gains 1 rage; M < 2 bleeding (save ends)
        tier3: 14 damage; the target gains 3 rage; M < 3 bleeding (save ends)
  - type: feature
    feature_type: ability
    name: Berserker Slash
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 1 burst
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 3
        tier1: 4 damage; push 2
        tier2: 6 damage; push 3; the target gains 1 rage
        tier3: 7 damage; slide 3; the target gains 3 rage
      - name: Effect
        effect: The werewolf shifts up to their speed before using this ability
  - type: feature
    feature_type: ability
    name: Wall Leap
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The werewolf jumps up to 4 squares. If they end this jump at a wall, the
          werewolf jumps off the wall up to 4 squares and can make a melee free
          strike. If the target of the free strike has M < 2, they are knocked
          prone.
  - type: feature
    feature_type: ability
    name: Facepalm and Head Slam
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 1
    target: The triggering creature
    trigger: A creature within distance targets the werewolf with a melee ability
      after charging or moving 2 or more squares in a straight line toward them.
    effects:
      - name: Effect
        effect: The target is knocked prone and takes 5 damage before the triggering
          ability is resolved.
  - type: feature
    feature_type: ability
    name: Howl
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target makes an Intuition test.
        tier1: The target must move their speed in a straight line away from the
          werewolf; frightened (save ends)
        tier2: Frightened (EoT)
        tier3: No effect
      - name: Effect
        effect: Any enemy in the encounter who has 1 or more rage gains 4 rage and howls
          along with the werewolf.
  - type: feature
    feature_type: ability
    name: Full Wolf
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The werewolf transforms into a massive wolf of size 3 until they die or
          until the end of the encounter. They move to a space that can
          accommodate their new size and push adjacent creatures out of their
          way. While in wolf form, they have speed 10 and stability 2, their
          strikes gain a +2 damage bonus and bestow an additional 1 rage, and
          the potency of Accursed Bite increases by 1.
  - type: feature
    feature_type: ability
    name: Rampage
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Weapon
    usage: "-"
    distance: 2 burst
    target: Each creature in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 damage; the target gains 2 rage; M < 1 bleeding (save ends)
        tier2: 8 damage; the target gains 4 rage; M < 2 bleeding (save ends)
        tier3: 11 damage; the target gains 8 rage; M < 3 bleeding (save ends)
      - name: Effect
        effect: The werewolf shifts up to their speed before and after using this
          ability.
~~~