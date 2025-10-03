---
agility: 3
ancestry:
- Dragon
- Elemental
ev: '48'
file_basename: Thorn Dragon
file_dpath: Monsters/Dragons/Statblocks
free_strike: 5
intuition: 1
item_id: thorn-dragon
item_index: '345'
item_name: Thorn Dragon
level: 2
might: 2
presence: 2
reason: -1
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:thorn-dragon
scdc:
- 1.1.1:2:345
size: '3'
source: mcdm.monsters.v1
speed: 8
stability: 6
stamina: '250'
type: monster
---

~~~ds-statblock
type: statblock
name: Thorn Dragon
level: 2
roles:
  - Solo
ancestry:
  - Dragon
  - Elemental
ev: "48"
stamina: "250"
immunities:
  - Poison 5
speed: 8
movement: Fly
size: "3"
stability: 6
free_strike: 5
might: 2
agility: 3
reason: -1
intuition: 1
presence: 2
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the dragon can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
      - name: Solo Turns
        effect: The dragon can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Withering Wyrmscale Aura
    icon: ❇️
    effects:
      - effect: The dragon's scales create a 2 aura of withering green magic around
          them. Any creature other than the dragon who regains Stamina in the
          area regains only half the expected amount. Any winded creature who
          enters the area for the first time in a round or starts their turn
          there takes 1d3 corruption damage.
  - type: feature
    feature_type: ability
    name: Virulent Breath
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 10 x 1 line within 1
    target: Each enemy and object in the area
    effects:
      - name: Effect
        effect: Each target makes a **Might test**.
        tier1: 12 poison damage; the target is dragonsealed (save ends)
        tier2: 9 poison damage; the target is dragonsealed (save ends)
        tier3: 5 poison damage
      - effect: A dragonsealed creature has their wounds bound by nettles and thorns,
          causing them to take an extra 1d3 damage whenever they take damage
          rolled as a d6 or a d3.
  - type: feature
    feature_type: ability
    name: Spinous Tail Swing
    icon: 🗡
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two enemies or objects
    effects:
      - roll: Power Roll + 3
        tier1: 8 damage; push 2
        tier2: 12 damage; push 4
        tier3: 15 damage; push 8
      - cost: 2 Malice
        effect: Each target takes an extra 1d3 damage, and if they have A < 2, they are
          bleeding (save ends).
  - type: feature
    feature_type: trait
    name: Provoking Nettles
    icon: ⭐️
    effects:
      - effect: Once per turn, the dragon shifts up to 5 squares and can move through
          enemies' spaces at their usual speed. The first time the dragon moves
          through an enemy's space during this movement, the enemy takes 3
          damage.
  - type: feature
    feature_type: ability
    name: Investiture of Verdure
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 10 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target must be dragonsealed. Each target is pulled up to 5 squares
          toward the dragon, who gains 5 temporary Stamina for each target
          pulled.
  - type: feature
    feature_type: ability
    name: Prickly Situation
    icon: ❗️
    keywords:
      - Magic
      - Ranged
    usage: Free triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A dragonsealed creature within distance ends the dragonsealed effect.
    effects:
      - name: Effect
        effect: The target is pulled up to 5 squares toward the dragon, and if they have
          A < 2, they are restrained until the end of their next turn.
  - type: feature
    feature_type: ability
    name: Thorny Scales
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Melee
    usage: Free triggered action
    distance: Melee 1
    target: The triggering creature
    trigger: A creature within distance deals damage to the dragon with a melee strike.
    effects:
      - name: Effect
        effect: The dragon makes a free strike against the target, and if the target has
          M < 2, they are bleeding until the end of their next turn.
  - type: feature
    feature_type: ability
    name: Briar Bindings
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 4 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 damage; A < 1 restrained (save ends)
        tier2: 9 damage; A < 2 restrained (save ends)
        tier3: 12 damage; A < 3 restrained (save ends)
  - type: feature
    feature_type: ability
    name: Thorned Armor
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The thorns upon the dragon's scales grow longer and sharper. Until the
          end of the encounter, any adjacent creature who targets the dragon
          with a melee strike takes 3 damage. The dragon then uses their
          Provoking Nettles ability.
  - type: feature
    feature_type: ability
    name: Malign Thicket
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - "-"
    usage: "-"
    distance: Special
    target: Special
    effects:
      - name: Effect
        effect: Poisonous overgrowth and seeking vines cover all surfaces on the
          encounter map. The dragon uses their Bramble Barricade Malice feature
          twice at no cost. Until the end of the encounter, any creature force
          moved by the dragon takes 1d3 poison damage, and if they have M < 2,
          they are weakened (save ends).
      - name: Special
        effect: If the Thorn Dragon's Domain trait is in effect, any creature other than
          the dragon who starts their turn on the encounter map takes 1d3 poison
          damage.
  - type: feature
    feature_type: trait
    name: Cage of Thorns
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: A cage of thorns grows around one dragonsealed enemy on the encounter
          map, making that enemy restrained until the end of their next turn.
  - type: feature
    feature_type: trait
    name: Bramble Barricade
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: The dragon grows a 10 wall of briars in unoccupied spaces on the
          encounter map. The wall blocks line of effect for all creatures except
          the dragon. Each square of the wall has 5 Stamina and fire weakness 5.
          The area can be moved through but is difficult terrain. Any creature
          who is force moved into or within the area takes 1 damage for each
          square of the area entered and is bleeding until the end of their next
          turn.
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The dragon takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - type: feature
    feature_type: trait
    name: Afflictive Overgrowth
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: The dragon summons poisonous, biting thorns around their foes. Each
          enemy on the encounter map makes an **Agility test**.
        tier1: 12 poison damage; restrained (save ends)
        tier2: 9 poison damage; bleeding (save ends)
        tier3: 5 poison damage; bleeding (EoT)
~~~