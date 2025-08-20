---
agility: 3
ancestry:
- Devil
- Infernal
ev: '32'
file_basename: Devil High Judge
file_dpath: Monsters/Devils/Statblocks
free_strike: 6
intuition: 1
item_id: devil-high-judge
item_index: '298'
item_name: Devil High Judge
level: 6
might: 1
presence: 2
reason: 0
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:devil-high-judge
scdc:
- 1.1.1:2:298
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 2
stamina: '181'
type: monster
---

```ds-statblock
name: Devil High Judge
level: 6
roles:
  - Leader
ancestry:
  - Devil
  - Infernal
ev: "32"
stamina: "181"
immunities:
  - Fire 5
speed: 7
movement: Fly
size: 1M
stability: 2
free_strike: 6
might: 1
agility: 3
reason: 0
intuition: 1
presence: 2
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the high judge can take 10 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - name: True Name
    effects:
      - effect: If a creature within 10 squares speaks the high judge's true name, the
          high judge loses their damage immunities, any nondamaging effects of
          their signature ability, and their Devilish Suggestion triggered
          action until the end of the encounter.
abilities:
  - name: Infernal Decree
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 12
    target: Three creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 10 damage; P < 2 the target can't hide (save ends)
        t2: 15 damage; P < 3 the target can't hide (save ends)
        t3: 19 damage; P < 4 the target can't hide (save ends)
      - effect: While a target is unable to hide this way, any strike against them made
          by a devil gains an edge.
        cost: 2 Malice
  - name: Compel the Jury
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Maneuver
    distance: Ranged 12
    target: Two creatures
    effects:
      - effect: |-
          **Power Roll + 4**
          - **≤11:** I < 2 the target is charmed (save ends)
          - **12-16:** I < 3 the target is charmed (save ends)
          - **17+:** I < 4 the target is charmed (save ends)
      - effect: While charmed this way, a creature treats the high judge as an ally, and
          the high judge can spend 1 Malice on their turn to make that creature
          move up to 3 squares.
  - name: Devilish Suggestion
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    type: Triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature targets the high judge with a strike.
    effects:
      - effect: >-
          The target makes a **Presence test**.

          - **≤11:** The target is charmed (save ends).

          - **12-16:** The high judge chooses a new target for the strike.

          - **17+:** The target takes a bane on the strike.

          While charmed this way, a creature treats the high judge as an ally,
          and the high judge can spend 1 Malice on their turn to make that
          creature move up to 3 squares.
  - name: All Rise
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - effect: >-
          The target makes a **Presence test**.

          - **≤11:** 15 psychic damage; the target is charmed (save ends)

          - **12-16:** 12 psychic damage; the target is charmed (save ends)

          - **17+:** 7 psychic damage

          While charmed this way, a creature treats the high judge as an ally,
          and the high judge can spend 1 Malice on their turn to make that
          creature move up to 3 squares.
  - name: Heed My Decree
    cost: Villain Action 2
    keywords:
      - Area
    type: "-"
    distance: 5 burst
    target: Self and each ally in the area
    effects:
      - effect: Each target shifts up to their speed. The high judge can make each
          creature charmed by All Rise, Compel the Jury, or Devilish Suggestion
          move up to half that creature's speed.
  - name: Deceptive Stratagem
    cost: Villain Action 3
    keywords:
      - Magic
      - Ranged
    type: "-"
    distance: Ranged 12
    target: One creature
    effects:
      - effect: If the target is an ally or a creature charmed by All Rise, Compel the
          Jury, or Devilish Suggestion, the high judge and the target teleport
          to swap places. Each ally within 12 squares of the high judge can then
          make a free strike against a target of the high judge's choice. Each
          creature charmed by All Rise, Compel the Jury, or Devilish Suggestion
          makes a free strike against a target of the high judge's choice.
```