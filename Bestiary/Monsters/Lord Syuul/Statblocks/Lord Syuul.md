---
agility: 3
ancestry:
- Horror
- Voiceless Talker
ev: '96'
file_basename: Lord Syuul
file_dpath: Monsters/Lord Syuul/Statblocks
free_strike: 7
intuition: 4
item_id: lord-syuul
item_index: '236'
item_name: Lord Syuul
level: 6
might: 1
presence: 3
reason: 4
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:lord-syuul
scdc:
- 1.1.1:2:236
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 3
stamina: '450'
type: monster
---

~~~ds-statblock
name: Lord Syuul
level: 6
roles:
  - Solo
ancestry:
  - Horror
  - Voiceless Talker
ev: "96"
stamina: "450"
immunities:
  - Psychic 10
speed: 7
movement: Hover, teleport
size: 1M
stability: 3
free_strike: 7
might: 1
agility: 3
reason: 4
intuition: 4
presence: 3
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of his turns, Lord Syuul can take 10 damage to end
          one effect on him that can be ended by a saving throw. This damage
          can't be reduced in any way.
        name: End Effect
      - effect: Lord Syuul can take two turns each round. He can't take turns
          consecutively.
        name: Solo Turns
  - name: Mind Over Manners
    effects:
      - effect: Whenever Lord Syuul uses a psionic ability, he can do so as if he were
          in the space of any creature within his line of effect who he has
          observed using a psionic ability.
abilities:
  - name: Tentacle Grab
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 11 damage; A < 2 grabbed
        t2: 17 damage; A < 3 grabbed
        t3: 20 damage; A < 4 grabbed
      - effect: The distance of this ability increases to melee 10. Each target grabbed
          by Lord Syuul is pulled up to 10 squares.
        cost: 2 Malice
  - name: Dampening Grenade
    icon: 🔳
    keywords:
      - Area
      - Psionic
      - Ranged
    type: Main action
    distance: 2 cube within 5
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 6 damage; the effect ends after 2 turns
        t2: 10 damage; the effect ends at the end of Lord Syuul's next turn
        t3: 13 damage; the effect lasts until the end of the encounter
      - effect: Any supernatural ability used by a creature in the area has a double
          bane. All reactive tests made against magic or psionic effects in the
          area have a double edge.
        name: Effect
  - name: Mind Blown
    icon: 🗡
    cost: 7 Malice
    keywords:
      - Melee
      - Psionic
      - Strike
    type: Main action
    distance: Melee 1
    target: One grabbed enemy
    effects:
      - roll: Power Roll + 4
        t1: 12 damage
        t2: 20 damage
        t3: 24 damage
      - effect: If this action reduces the target to 0 Stamina and they have a brain,
          their brain explodes, instantly killing them.
        name: Effect
  - name: You Come With Me
    icon: 👤
    keywords:
      - Psionic
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: Lord Syuul can teleport up to 5 squares along with each creature and
          object he has grabbed. He can release grabbed creatures and objects
          before or after teleporting
  - name: Adaptability
    icon: ❗️
    keywords:
      - Psionic
    type: Triggered action
    distance: Self
    target: Self
    trigger: Lord Syuul takes damage that has a damage type.
    effects:
      - effect: Until the start of his next turn, Lord Syuul gains immunity 5 to the
          triggering damage type.
        name: Effect
  - name: See Only Me
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
      - Psionic
    type: "-"
    distance: 10 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target makes an **Intuition test**.
        t1: 16 psychic damage; the target has no line of effect to any creture except
          Lord Syuul, and takes a bane on strikes targeting Lord Syuul (save
          ends)
        t2: 13 psychic damage; the target has no line of effect to any creature except
          Lord Syuul (save ends)
        t3: 7 psychic damage
  - name: Phantom Pain
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Psionic
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: Lord Syuul becomes invisible, can teleport up to 10 squares, and
          projects an illusory double within 10 squares. The double can't move
          or act, but Lord Syuul can use psionic abilities as if he were in its
          square. Whenever a creature touches or damages the double with a melee
          strike, they take 10 psychic damage. If Lord Syuul takes damage, his
          invisibility ends and the double disappears.
        name: Effect
  - name: Mindshatter
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Psionic
    type: "-"
    distance: 5 burst
    target: Each creature in the area
    effects:
      - roll: Power Roll + 4
        t1: 7 psychic damage
        t2: 13 psychic damage
        t3: 16 psychic damage
      - effect: Until the end of the encounter, each target has damage weakness 3.
        name: Effect
~~~