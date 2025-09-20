---
agility: 1
ancestry:
- Humanoid
- Rival
ev: '48'
file_basename: Rival Conduit
file_dpath: Monsters/Rivals/4th Echelon/Statblocks
free_strike: 10
intuition: 5
item_id: rival-conduit
item_index: '31'
item_name: Rival Conduit
level: 10
might: 4
presence: 3
reason: 1
roles:
- Elite Support
scc:
- mcdm.monsters.v1:monster:rival-conduit
scdc:
- 1.1.1:2:31
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '240'
type: monster
---

~~~ds-statblock
type: statblock
name: Rival Conduit
level: 10
roles:
  - Elite Support
ancestry:
  - Humanoid
  - Rival
ev: "48"
stamina: "240"
speed: 5
size: 1M
stability: 1
free_strike: 10
might: 4
agility: 1
reason: 1
intuition: 5
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Sunder the Very Skies
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    usage: Main action
    distance: Melee 1 or ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        tier1: 15 damage; vertical slide 3; M < 3 5 lightning damage
        tier2: 20 damage; vertical slide 4; M < 4 7 lightning damage
        tier3: 24 damage; vertical slide 5; M < 5 9 lightning damage
      - name: Effect
        effect: The conduit or one ally within distance regains Stamina equal to half
          the damage dealt.
      - cost: 2 Malice
        effect: Two additional allies within distance regain the same amount of Stamina.
  - type: feature
    feature_type: ability
    name: Empyrean Boon
    icon: 🏹
    cost: 5 Malice
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Self and five allie
    effects:
      - name: Effect
        effect: Each target has a double edge on their next strike, and that strike
          deals an extra 10 holy damage. Additionally, they can vertical slide
          each creature targeted by the strike up to 2 squares.
  - type: feature
    feature_type: trait
    name: Unwavering Defender
    icon: ⭐️
    effects:
      - effect: Damage dealt to any ally adjacent to the conduit is halved.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the conduit chooses one creature within
          their line of effect. Both the conduit and the creature can add a d3
          roll to power rolls they make against each other.
~~~