---
agility: 2
ancestry:
- Draconian
- Dragon
- Humanoid
ev: '32'
file_basename: Phrrygalax the Subduer
file_dpath: Monsters/Draconians/Statblocks
free_strike: 7
intuition: 0
item_id: phrrygalax-the-subduer
item_index: '103'
item_name: Phrrygalax the Subduer
level: 6
might: 3
presence: 3
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:phrrygalax-the-subduer
scdc:
- 1.1.1:2:103
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '180'
type: monster
---

~~~ds-statblock
type: statblock
name: Phrrygalax the Subduer
level: 6
roles:
  - Elite Brute
ancestry:
  - Draconian
  - Dragon
  - Humanoid
ev: "32"
stamina: "180"
immunities:
  - Fire 6
speed: 5
movement: Fly
size: 1L
stability: 3
free_strike: 7
might: 3
agility: 2
reason: 0
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Baneful Blade
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
        tier1: 10 damage
        tier2: 16 damage; M < 1 bleeding (save ends)
        tier3: 19 damage; M < 2 3 damage, bleeding (save ends)
  - type: feature
    feature_type: ability
    name: Spinning Spit
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 7 fire damage
        tier2: 13 fire damage
        tier3: 16 fire damage
  - type: feature
    feature_type: ability
    name: Heavy Landing
    icon: 👤
    keywords:
      - Area
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: Phrrygalax flies up to his speed and lands in an unoccupied space on the
          ground. Each creature adjacent to where he lands who has A < 2 is
          knocked prone.
  - type: feature
    feature_type: ability
    name: Armor of the Ancients
    icon: ❗️
    cost: 2 Malice
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: Phrrygalax takes acid, cold, corruption, fire, lightning, or poison damage.
    effects:
      - name: Effect
        effect: Phrrygalax takes no damage and instead regains the same amount of
          Stamina. He then swaps his current damage immunity with the triggering
          damage type.
  - type: feature
    feature_type: ability
    name: Still Your Tongue!
    icon: ❗️
    keywords:
      - "-"
    usage: Free triggered action
    distance: Self
    target: Self
    trigger: Phrrygalax hears a creature within 5 squares reciting the oath of Good
      King Omund's Dragon Phalanx.
    effects:
      - name: Effect
        effect: Phrrygalax shifts up to his speed and uses Baneful Blade against the
          triggering creature. That ability deals an extra 7 damage.
  - type: feature
    feature_type: trait
    name: Oathbreaker's Vengeance
    icon: ⭐️
    effects:
      - effect: Whenever Phrrygalax fails a saving throw, he deals an additional 7
          damage on his next strike.
~~~