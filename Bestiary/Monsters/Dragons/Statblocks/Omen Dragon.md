---
agility: 4
ancestry:
- Dragon
- Elemental
ev: '120'
file_basename: Omen Dragon
file_dpath: Monsters/Dragons/Statblocks
free_strike: 9
intuition: 3
item_id: omen-dragon
item_index: '343'
item_name: Omen Dragon
level: 8
might: 3
presence: 5
reason: 2
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:omen-dragon
scdc:
- 1.1.1:2:343
size: '5'
source: mcdm.monsters.v1
speed: 10
stability: 6
stamina: '550'
type: monster
---

```ds-statblock
name: Omen Dragon
level: 8
roles:
  - Solo
ancestry:
  - Dragon
  - Elemental
ev: "120"
stamina: "550"
immunities:
  - Corruption 6
speed: 10
movement: Fly
size: "5"
stability: 6
free_strike: 9
might: 3
agility: 4
reason: 2
intuition: 3
presence: 5
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the dragon can take 15 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
        name: End Effect
      - effect: The dragon can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Deathcount
    effects:
      - effect: Several of the dragon's abilities impose a Deathcount on a target. At
          the end of every turn, a creature with a Deathcount who is within the
          area of the dragon's Stagnant Wyrmscale Aura has that Deathcount
          reduced by 1. When a creature's Deathcount hits 0, they die. If
          multiple Deathcounts are imposed on a creature, they don't stack. Only
          the lowest Deathcount takes effect. All Deathcounts are lost when the
          dragon is reduced to 0 Stamina.
  - name: Stagnant Wyrmscale Aura
    effects:
      - effect: The dragon's scales create a 4 aura of supernatural stagnancy around
          them. The area is difficult terrain for enemies, and no creature
          except the omen dragon can regain Stamina while in the area. Any
          creature dragonsealed by the omen dragon who starts their turn in the
          dragon's aura and doesn't have a Deathcount gains a Deathcount of 12.
  - name: Death or Victory
    effects:
      - effect: Once per turn, the dragon chooses one creature with a Deathcount within
          line of effect. That creature can choose to take 1d6 damage and lose a
          recovery to increase their Deathcount by 5.
  - name: Black Skies
    effects:
      - effect: The dragon expands their wings to create a shroud of shadow. Until the
          start of the dragon's next turn, any strike made against them takes a
          bane.
  - name: Rise and Fall
    effects:
      - effect: >-
          The dragon flies up to 10 squares and carries fated souls with them.
          Each creature in the area of the dragon's Stagnant Wyrmscale Aura
          trait makes a **Presence test**.

          - **≤11:** Vertical pull 10

          - **12-16:** Vertical pull 6

          - **17+:** Vertical pull 4
  - name: Solo Action
    effects:
      - effect: The dragon takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - name: Burn It Right Down
    effects:
      - effect: Each edge of the encounter map burns with intangible purple flames until
          the end of the encounter. The flames expand by 1 square at the end of
          every turn. Any enemy takes 5 corruption damage for each square of
          flames they enter.
abilities:
  - name: Corroding Breath
    cost: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 5 cube within 10
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: Each target makes an **Agility test**.
        t1: 18 corruption damage; the target is dragonsealed (save ends)
        t2: 14 corruption damage; the target is dragonsealed (save ends)
        t3: 9 corruption damage
      - effect: Only creatures with souls can be dragonsealed by the omen dragon. A
          dragonsealed creature appears ghastly and pale, their Presence score
          is treated as 1 lower for the purpose of resisting potencies, and they
          can't treat other creatures as allies.
  - name: Barbed Tail Swing
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 4
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 14 damage; M < 3 bleeding (save ends)
        t2: 19 damage; M < 4 bleeding (save ends)
        t3: 23 damage; M < 5 bleeding (save ends)
      - effect: The potency increases by 2, and each target is also pulled up to 5
          squares.
        cost: 3 Malice
  - name: Detonation
    cost: 5 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 10 burst
    target: Each enemy in the area
    effects:
      - effect: Each target must be dragonsealed. Each target takes 9 corruption damage,
          and the omen dragon regains Stamina equal to half the total damage
          dealt. The target then loses their dragonseal.
        name: Effect
  - name: Don't Turn Away
    cost: 1 Malice
    keywords:
      - "-"
    type: Free triggered action
    distance: Self
    target: Self
    trigger: A creature leaves the area of the dragon's Stagnant Wyrmscale Aura trait.
    effects:
      - effect: The dragon shifts up to their speed, and the Deathcount of each
          dragonsealed creature who comes adjacent to the dragon during this
          shift is reduced by 1.
        name: Effect
  - name: Repent!
    cost: 2 Malice
    keywords:
      - Ranged
    type: Free triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A dragonsealed creature within distance deals damage to the dragon.
    effects:
      - effect: The target must choose between making a free strike against themself or
          gaining a Deathcount of 5.
        name: Effect
  - name: What You Deserve
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        t1: Pull 1; the target has a Deathcount of 10
        t2: Pull 2; the target has a Deathcount of 8
        t3: Pull 3; the target has a Deathcount of 6
      - effect: Each target receives a premonition of their imminent death.
        name: Effect
  - name: Souls of the Broken
    cost: Villain Action 2
    keywords:
      - Magic
      - Ranged
      - Strike
    type: "-"
    distance: Ranged 10
    target: Five creatures
    effects:
      - name: Effect
        effect: The dragon spits fragments of souls to attempt to possess the targets,
          making a separate power roll for each target.
      - roll: Power Roll + 5
        t1: P < 5 frightened (save ends)
        t2: P < 5 the target moves up to their speed toward the dragon
        t3: P < 5 the target makes a free strike against the nearest ally
  - name: So Long and Goodnight
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 6 burst
    target: Each creature in the area
    effects:
      - effect: Each target must be dragonsealed. The dragon's eyes glow with unequalled
          malevolence, and any target who has a Deathcount has that Deathcount
          reduced to 1.
        name: Effect
```