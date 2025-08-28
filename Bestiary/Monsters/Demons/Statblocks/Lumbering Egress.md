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
item_index: '266'
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
- 1.1.1:2:266
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 3
stamina: '180'
type: monster
---

~~~ds-statblock
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
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the egress can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
abilities:
  - name: Ensnarer Cannon
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 11 corruption damage; A < 2 restrained (save ends)
        t2: 16 corruption damage; A < 3 restrained (save ends)
        t3: 19 corruption damage; A < 4 restrained (save ends)
      - effect: Two ensnarers appear in unoccupied spaces adjacent to each target. On a
          tier 3 outcome, four ensnarers appear.
        cost: 2 Malice
  - name: Demonic Egress
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 3 burst
    target: Special
    effects:
      - effect: Four level 1 demon minions (most commonly ensnarers, frenzieds, and
          pitlings) burst forth from the egress and appear in unoccupied spaces
          in the area.
        name: Effect
      - effect: Four level 4 demon minions (most commonly orliq, grulqins, and wobalas)
          appear instead.
        cost: 2 Malice
  - name: Abyssal Protectors
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Area
      - Magic
    type: Triggered action
    distance: 5 burst
    target: Special
    trigger: The last ally minion on the encounter map dies, or the egress is
      reduced below 25 Stamina.
    effects:
      - effect: Eight ensnarers appear anywhere in the area.
        name: Effect
  - name: Frenzied Deluge
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Ranged
    type: "-"
    distance: Ranged 10
    target: Three enemies
    effects:
      - roll: Power Roll + 4
        t1: 7 corruption damage
        t2: 2 12 corruption damage
        t3: 3 15 corruption damage; two frenzieds appear in unoccupied spaces adjacent
          to each target
  - name: Fold Space
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Ranged
    type: "-"
    distance: Ranged 20
    target: Self
    effects:
      - effect: The egress folds into their own portal and teleports to an un occupied
          space within distance. Four level 4 demon minions (most commonly
          orliq, grulqins, and wobalas) appear in squares in the egress's former
          space.
        name: Effect
  - name: Blood of the Abyss
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 10 x 3 line within 1
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 4
        t1: 6 corruption damage; R < 2 weakened (save ends)
        t2: 2 11 corruption damage; R < 3 weakened (save ends)
        t3: 3 14 corruption damage; R < 4 weakened (save ends)
      - effect: The egress recalls and instantly destroys any minion allies on the
          encounter map. A torrent of churned-up minion bodies, blood, and ichor
          erupts from the egress, dealing an extra 1 damage for each minion
          destroyed this way.
        name: Effect
~~~