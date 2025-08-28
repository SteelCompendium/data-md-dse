---
agility: 2
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '28'
file_basename: Hobgoblin War Mage
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 6
intuition: 2
item_id: hobgoblin-war-mage
item_index: '184'
item_name: Hobgoblin War Mage
level: 5
might: 0
presence: 2
reason: 3
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:hobgoblin-war-mage
scdc:
- 1.1.1:2:184
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '120'
type: monster
---

```ds-statblock
name: Hobgoblin War Mage
level: 5
roles:
  - Elite Controller
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "28"
stamina: "120"
immunities:
  - Fire 5
speed: 5
movement: Hover, teleport
size: 1M
stability: 0
free_strike: 6
might: 0
agility: 2
reason: 3
intuition: 2
presence: 2
traits:
  - name: Infernal Ichor
    effects:
      - effect: When the war mage is reduced to 0 Stamina, they spray burning blood.
          Each creature adjacent to the war mage takes 3 fire damage.
  - name: Despair, You Who Face Death
    effects:
      - effect: Any enemy within 2 squares of the war mage has a −2 penalty to saving
          throws.
abilities:
  - name: Hellfire
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 5 fire damage; M < 1 weakened (save ends)
        t2: 9 fire damage; M < 2 weakened (save ends)
        t3: 11 fire damage; M < 3 weakened (save ends)
      - effect: Before using this ability, the war mage can teleport a creature within
          10 squares of them up to 2 squares.
        name: Effect
  - name: Enchantments of War
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    type: Main action
    distance: Ranged 10
    target: Two allies
    effects:
      - effect: Each target gains 10 temporary Stamina and has a double edge on their
          next power roll. The war mage can spend any amount of their current
          Stamina to increase the temporary Stamina each target gains by an
          equivalent amount.
        name: Effect
  - name: Unhallowed Ground
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 5 cube within 10
    target: Special
    effects:
      - effect: The war mage consecrates the area and causes it to smolder until the end
          of the encounter. The area is difficult terrain and an enemy in the
          area has fire weakness 10.
        name: Effect
  - name: Magic Siphon
    icon: ❗️
    keywords:
      - Magic
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A creature within distance uses a magic ability.
    effects:
      - effect: Any damage dealt or Stamina regained from the creature's ability is
          halved. The war mage regains Stamina equal to the remaining damage
          dealt or Stamina regained.
        name: Effect
```