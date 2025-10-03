---
agility: -1
ancestry:
- Abyssal
- Demon
ev: '32'
file_basename: Lumbering Egress
file_dpath: Monsters/Demons/Statblocks
free_strike: 7
intuition: 2
item_id: lumbering-egress
item_index: '264'
item_name: Lumbering Egress
level: 6
might: 4
presence: 2
reason: 1
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:lumbering-egress
scdc:
- 1.1.1:2:264
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 3
stamina: '180'
type: monster
---

~~~ds-statblock
type: statblock
name: Lumbering Egress
level: 6
roles:
  - Leader
ancestry:
  - Abyssal
  - Demon
ev: "32"
stamina: "180"
weaknesses:
  - Holy 5
speed: 6
size: "3"
stability: 3
free_strike: 7
might: 4
agility: -1
reason: 1
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Ensnarer Cannon
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 11 corruption damage; A < 2 restrained (save ends)
        tier2: 16 corruption damage; A < 3 restrained (save ends)
        tier3: 19 corruption damage; A < 4 restrained (save ends)
      - cost: 2 Malice
        effect: Two ensnarers appear in unoccupied spaces adjacent to each target. On a
          tier 3 outcome, four ensnarers appear.
  - type: feature
    feature_type: ability
    name: Demonic Egress
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 3 burst
    target: Special
    effects:
      - name: Effect
        effect: Four level 1 demon minions (most commonly ensnarers, frenzieds, and
          pitlings) burst forth from the egress and appear in unoccupied spaces
          in the area.
      - cost: 2 Malice
        effect: Four level 4 demon minions (most commonly orliq, grulqins, and wobalas)
          appear instead.
  - type: feature
    feature_type: ability
    name: Abyssal Protectors
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Area
      - Magic
    usage: Triggered action
    distance: 5 burst
    target: Special
    trigger: The last ally minion on the encounter map dies, or the egress is
      reduced below 25 Stamina.
    effects:
      - name: Effect
        effect: Eight ensnarers appear anywhere in the area.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of their turns, the egress can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - type: feature
    feature_type: ability
    name: Frenzied Deluge
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Ranged
    usage: "-"
    distance: Ranged 10
    target: Three enemies
    effects:
      - roll: Power Roll + 4
        tier1: 7 corruption damage
        tier2: 12 corruption damage
        tier3: 15 corruption damage; two frenzieds appear in unoccupied spaces adjacent
          to each target
  - type: feature
    feature_type: ability
    name: Fold Space
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Ranged
    usage: "-"
    distance: Ranged 20
    target: Self
    effects:
      - name: Effect
        effect: The egress folds into their own portal and teleports to an unoccupied
          space within distance. Four level 4 demon minions (most commonly
          orliq, grulqins, and wobalas) appear in squares in the egress's former
          space.
  - type: feature
    feature_type: ability
    name: Blood of the Abyss
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 10 x 3 line within 1
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 4
        tier1: 6 corruption damage; R < 2 weakened (save ends)
        tier2: 11 corruption damage; R < 3 weakened (save ends)
        tier3: 14 corruption damage; R < 4 weakened (save ends)
      - name: Effect
        effect: The egress recalls and instantly destroys any minion allies on the
          encounter map. A torrent of churned-up minion bodies, blood, and ichor
          erupts from the egress, dealing an extra 1 damage for each minion
          destroyed this way.
~~~