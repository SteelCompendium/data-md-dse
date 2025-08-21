---
agility: 3
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '32'
file_basename: Shadow Elf Eclipse
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 7
intuition: 1
item_id: shadow-elf-eclipse
item_index: '219'
item_name: Shadow Elf Eclipse
level: 6
might: 4
presence: 2
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:shadow-elf-eclipse
scdc:
- 1.1.1:2:219
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 1
stamina: '180'
type: monster
---

```ds-statblock
name: Shadow Elf Eclipse
level: 6
roles:
  - Leader
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: "32"
stamina: "180"
speed: 6
movement: Climb
size: 1M
stability: 1
free_strike: 7
might: 4
agility: 3
reason: 2
intuition: 1
presence: 2
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the eclipse can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - name: Of the Umbra
    effects:
      - effect: The eclipse ignores concealment created by darkness. While the eclipse
          is in direct sunlight, they have damage weakness 3. While the eclipse
          has concealment, they have damage immunity 3.
abilities:
  - name: Manifold Blade
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
        t1: 11 damage; I < 2 bleeding (save ends)
        t2: 16 damage; I < 3 bleeding (save ends)
        t3: 19 damage; I < 4 bleeding (save ends)
      - effect: The potency increases by 1.
        cost: 2 Malice
  - name: Grasping Shadow
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: Three creatures or objects casting a shadow
    effects:
      - roll: Power Roll + 4
        t1: Pull 5; I < 2 slowed (save ends)
        t2: Pull 7; I < 3 slowed (save ends)
        t3: Pull 10; I < 4 slowed (save ends)
  - name: Put It Out!
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering enemy
    trigger: An enemy within distance uses an ability that emits light, including
      abilities that deal fire or lightning damage.
    effects:
      - effect: The target has a double bane on the ability.
        name: Effect
  - name: From the Shadows
    cost: Villain Action 1
    keywords:
      - Ranged
    type: "-"
    distance: Ranged 5
    target: Special
    effects:
      - effect: The eclipse calls forth one brush stalker into an unoccupied space
          within distance. Each ally within distance can then shift up to their
          speed and make a free strike.
        name: Effect
  - name: Cast Away All Hope
    cost: Villain Action 2
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - effect: Each target loses all their surges. Additionally, until the end of the
          round, allies ignore edges and double edges on any targets' abilities,
          and ignore any nondamaging effects of any target's damage-dealing
          abilities.
        name: Effect
  - name: Umbral Hunger
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 3 cube within 5
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 7 corruption damage; R < 2 the target has speed 0 (save ends)
        t2: 12 corruption damage; R < 3 the target has speed 0 (save ends)
        t3: 15 corruption damage; R < 4 the target has speed 0 (save ends)
      - effect: The area is shrouded in darkness that creates concealment until the end
          of the encounter. Any enemy who starts their turn in the area takes 5
          corruption damage.
        name: Effect
```