---
agility: 2
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '32'
file_basename: Hobgoblin Bloodlord
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 7
intuition: 3
item_id: hobgoblin-bloodlord
item_index: '186'
item_name: Hobgoblin Bloodlord
level: 6
might: 4
presence: 3
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:hobgoblin-bloodlord
scdc:
- 1.1.1:2:186
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '180'
type: monster
---

```ds-statblock
name: Hobgoblin Bloodlord
level: 6
roles:
  - Leader
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "32"
stamina: "180"
immunities:
  - Fire 6
speed: 6
movement: Teleport
size: 1M
stability: 2
free_strike: 7
might: 4
agility: 2
reason: 2
intuition: 3
presence: 3
traits:
  - name: Infernal Ichor
    effects:
      - effect: When the bloodlord is reduced to 0 Stamina, they spray burning blood.
          Each creature adjacent to the bloodlord takes 3 fire damage.
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the bloodlord can take 10 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way
abilities:
  - name: Soul Sword
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 11 corruption damage; P < 2 bleeding (save ends)
        t2: 16 corruption damage; P < 3 bleeding (save ends)
        t3: 19 corruption damage; P < 4 bleeding (save ends)
      - effect: Each target is marked until the end of the encounter or until they die.
          The bloodlord's allies gain an edge on strikes against any target
          marked this way. The bloodlord can have up to three targets marked
          this way. If they mark a new target who would exceed the limit, the
          oldest mark ends.
        cost: 2 Malice
  - name: Take Point!
    icon: 🏹
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One ally
    effects:
      - effect: The target moves up to their speed and can use a signature ability.
        name: Effect
  - name: An Army From Blood
    icon: ❗️
    cost: 3 Malice
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A non-minion hobgoblin within distance takes damage.
    effects:
      - effect: Three hobgoblin recruits manifest from the target's blood into
          unoccupied spaces adjacent to the target.
        name: Effect
  - name: Advance!
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Self and each ally in the area
    effects:
      - effect: Each target gains 10 temporary Stamina and can move up to their speed.
          Then each non-minion target can make a free strike.
        name: Effect
  - name: Skulls Abound
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 3 aura
    target: Self
    effects:
      - effect: Until the end of the encounter, the bloodlord surrounds themself with a
          storm of flying skulls. Any enemy who enters the area for the first
          time in a round or starts their turn there takes 8 corruption damage
          and takes a bane on their next power roll until the start of their
          next turn.
        name: Effect
  - name: I Am Fire! I Am Death!
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 5 fire damage; P < 2 2 fire damage, push 2, prone
        t2: 5 fire damage; P < 3 7 fire damage, push 3, prone
        t3: 5 fire damage; P < 4 10 fire damage, push 5, prone
      - effect: Until the end of the encounter, the bloodlord is wreathed in black
          flames. Whenever any adjacent enemy grabs the bloodlord or uses a
          melee ability against them, that enemy takes 5 corruption damage.
        name: Effect
```