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
item_index: '241'
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
- 1.1.1:2:241
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
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
features:
  - type: feature
    feature_type: ability
    name: Acid Grasp
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
        tier1: 7 acid damage; A < 1 dazed (save ends)
        tier2: 10 acid damage; A < 2 dazed (save ends)
        tier3: 13 acid damage; A < 3 dazed (save ends)
      - name: Effect
        effect: The next time the target makes a strike against the daybringer, the
          target takes 4 acid damage after the strike is resolved.
      - cost: 1 Malice
        effect: The daybringer jumps up to 3 squares before or after using this ability.
  - type: feature
    feature_type: ability
    name: Sun Lamp
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The daybringer expands their throat to make it resemble the sun until
          the start of their next turn. During that time, each angulotl who
          starts their turn within 10 squares of the daybringer regains 5
          Stamina and gains a +3 bonus to speed until the end of their turn.
  - type: feature
    feature_type: ability
    name: Tongue Slap
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 5
    target: One creature
    trigger: The target makes a strike against the daybringer or an ally that isn't
      a critical hit.
    effects:
      - name: Effect
        effect: The outcome of the strike's power roll is reduced by one tier.
      - cost: 2 Malice
        effect: The target is pulled up to 4 squares after the strike resolves.
  - type: feature
    feature_type: trait
    name: Moisturizing End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of the daybringer's turns, they can either take 5
          damage or end the wet effect on an adjacent creature in order to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - type: feature
    feature_type: ability
    name: New Dawn
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Ranged
    usage: "-"
    distance: Ranged 10
    target: Special
    effects:
      - name: Effect
        effect: Four **angulotl pollywogs** erupt from the daybringer's back and waddle
          into unoccupied spaces within distance.
  - type: feature
    feature_type: ability
    name: Plague of Frogs
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
    usage: "-"
    distance: 8 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Each target can jump up to 4 squares. Each non-minion target can make a
          free strike at the end of the jump.
  - type: feature
    feature_type: ability
    name: It Is Day
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - "-"
    usage: "-"
    distance: Special
    target: Special
    effects:
      - name: Effect
        effect: The encounter map dries up and each enemy and object on it is
          illuminated until the end of the encounter. An illuminated creature or
          object can't hide or become invisible, and any strike made against an
          illuminated target gains an edge. Additionally, each enemy in the
          encounter who is wet has that effect end and takes 6 acid damage. Each
          angulotl in the encounter has a double edge on their next strike.
  - type: feature
    feature_type: trait
    name: Toxiferous
    icon: ⭐️
    effects:
      - effect: Whenever an adjacent enemy grabs the daybringer or uses a melee ability
          against them, that enemy takes 3 poison damage.
~~~