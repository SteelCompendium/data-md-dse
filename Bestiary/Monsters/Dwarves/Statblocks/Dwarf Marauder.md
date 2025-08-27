---
agility: 0
ancestry:
- Dwarf
- Humanoid
ev: '20'
file_basename: Dwarf Marauder
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 5
intuition: 1
item_id: dwarf-marauder
item_index: '397'
item_name: Dwarf Marauder
level: 3
might: 3
presence: 0
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:dwarf-marauder
scdc:
- 1.1.1:2:397
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '132'
type: monster
---

```ds-statblock
name: Dwarf Marauder
level: 3
roles:
  - Leader
ancestry:
  - Dwarf
  - Humanoid
ev: "20"
stamina: "132"
speed: 5
size: 1M
stability: 4
free_strike: 5
might: 3
agility: 0
reason: 2
intuition: 1
presence: 0
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the marauder lord can take 5 damage
          to end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
abilities:
  - name: Levitating Axes
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 8 damage; slide 1
        t2: 12 damage; slide 3
        t3: 15 damage; slide 5
      - effect: A target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
        name: Effect
      - effect: A target force moved adjacent to an ally of the marauder lord is
          restrained until the end of their next turn.
        cost: 3 Malice
  - name: Magnetomancy
    icon: 🏹
    keywords:
      - Psionic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One creature or object
    effects:
      - effect: The target vertical slides up to 5 squares. A target restrained by a
          dwarf can be force moved by this ability. This forced movement doesn't
          end the restrained condition unless the Director determines otherwise.
        name: Effect
      - effect: This ability takes the Area keyword and loses the Ranged keyword, its
          distance becomes a 10 burst, and it targets each restrained creature
          in the area.
        cost: 5 Malice
  - name: Your Weapon Is Useless
    icon: ❗️
    keywords:
      - Psionic
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: Self or one ally
    trigger: A creature makes a melee strike against the target.
    effects:
      - effect: The target halves any damage from the strike and the triggering creature
          takes 4 damage.
        name: Effect
  - name: Ajax Will Pay Well for These Specimens
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
      - Psionic
      - Ranged
      - Weapon
    type: "-"
    distance: 5 cube within 10
    target: Each enemy in the area
    effects:
      - effect: The marauder lord uses Levitating Axes against each target, making one
          power roll against all targets.
        name: Effect
  - name: Don't Let Them Escape!
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
    type: "-"
    distance: 5 burst
    target: Each ally in the area
    effects:
      - effect: Each target shifts up to their speed. The marauder lord then uses
          Levitating Axes.
        name: Effect
  - name: Test Your Metal!
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Psionic
      - Ranged
    type: "-"
    distance: Ranged 10
    target: Special
    effects:
      - effect: The marauder lord creates three size 2 metal objects in unoccupied
          spaces within distance. Whenever the marauder lord uses Magnetomancy,
          they can additionally target one of these objects.
        name: Effect
```