---
agility: 2
ancestry:
- Angulotl
- Humanoid
ev: '12'
file_basename: Angulotl Daybringer
file_dpath: Monsters/Angulotls/Statblocks
free_strike: 4
intuition: 2
item_id: angulotl-daybringer
item_index: '243'
item_name: Angulotl Daybringer
level: 1
might: 3
presence: 0
reason: 0
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:angulotl-daybringer
scdc:
- 1.1.1:2:243
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '80'
type: monster
---

~~~ds-statblock
name: Angulotl Daybringer
level: 1
roles:
  - Leader
ancestry:
  - Angulotl
  - Humanoid
ev: "12"
stamina: "80"
immunities:
  - Poison 3
speed: 5
movement: Climb, swim
size: 1M
stability: 1
free_strike: 4
might: 3
agility: 2
reason: 0
intuition: 2
presence: 0
traits:
  - name: Moisturizing End Effect
    effects:
      - effect: At the end of each of the daybringer's turns, they can either take 5
          damage or end the wet effect on an adjacent creature in order to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - name: Toxiferous
    effects:
      - effect: Whenever an adjacent enemy grabs the daybringer or uses a me lee ability
          against them, that enemy takes 3 poison damage.
abilities:
  - name: Acid Grasp
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
      - roll: Power Roll + 3
        t1: 7 acid damage; A < 1 dazed (save ends)
        t2: 10 acid damage; A < 2 dazed (save ends)
        t3: 13 acid damage; A < 3 dazed (save ends)
      - effect: The next time the target makes a strike against the daybringer, the
          target takes 4 acid damage after the strike is resolved.
        name: Effect
      - effect: The daybringer jumps up to 3 squares before or after using this ability.
        cost: 1 Malice
  - name: Sun Lamp
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The daybringer expands their throat to make it resemble the sun until
          the start of their next turn. During that time, each angulotl who
          starts their turn within 10 squares of the daybringer regains 5
          Stamina and gains a +3 bonus to speed until the end of their turn.
        name: Effect
  - name: Tongue Slap
    icon: ❗️
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 5
    target: One creature
    trigger: The target makes a strike against the daybringer or an ally that isn't
      a critical hit.
    effects:
      - effect: The outcome of the strike's power roll is reduced by one tier.
        name: Effect
      - effect: The target is pulled up to 4 squares after the strike resolves.
        cost: 2 Malice
  - name: New Dawn
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Ranged
    type: "-"
    distance: Ranged 10
    target: Special
    effects:
      - effect: Four **angulotl pollywogs** erupt from the daybringer's back and waddle
          into unoccupied spaces within distance.
        name: Effect
  - name: Plague of Frogs
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
    type: "-"
    distance: 8 burst
    target: Self and each ally in the area
    effects:
      - effect: Each target can jump up to 4 squares. Each non-minion target can make a
          free strike at the end of the jump.
        name: Effect
  - name: It Is Day
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - "-"
    type: "-"
    distance: Special
    target: Special
    effects:
      - effect: The encounter map dries up and each enemy and object on it is
          illuminated until the end of the encounter. An illuminated creature or
          object can't hide or become invisible, and any strike made against an
          illuminated target gains an edge. Additionally, each enemy in the
          encounter who is wet has that effect end and takes 6 acid damage. Each
          angulotl in the encounter has a double edge on their next strike.
        name: Effect
~~~