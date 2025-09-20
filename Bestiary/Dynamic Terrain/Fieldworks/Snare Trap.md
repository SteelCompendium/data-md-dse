---
file_basename: Snare Trap
file_dpath: Dynamic Terrain/Fieldworks
item_id: snare-trap-level-1-trap-ambusher
item_index: '01'
item_name: Snare Trap (Level 1 Trap Ambusher)
scc:
- mcdm.monsters.v1:dynamic-terrain.fieldwork:snare-trap-level-1-trap-ambusher
scdc:
- 1.1.1:4.3:01
source: mcdm.monsters.v1
type: dynamic-terrain/fieldwork
---

~~~ds-featureblock
type: featureblock
featureblock_type: Trap Ambusher
name: Snare Trap
level: 1
ev: "1"
flavor: A rope snare is set to grab a target, leaving them hanging upside down.
stamina: "1"
size: 1S
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a snare trap can make an **Agility
          test**.
        tier1: The creature triggers the trap and is affected as if in its space.
        tier2: The trap is deactivated but the creature is slowed (EoT).
        tier3: The trap is deactivated and doesn't trigger.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: The snare trap is calibrated to be triggered by creatures or objects of
          a particular size or larger. The trap triggers when a creature or
          object of the appropriate size enters its space.
      - name: Effect
        effect: A triggering creature or object ends their movement and is targeted by
          the **Snare** ability.
  - type: feature
    feature_type: ability
    name: Snare
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Free triggered action
    distance: Melee 0
    target: The triggering creature or object
    trigger: A creature or object of the appropriate size enters the trap's space.
    effects:
      - roll: Power Roll + 2
        tier1: The target shifts 1 square away from the snare.
        tier2: 1 damage; A < 1 restrained (save ends)
        tier3: 3 damage; A < 2 restrained (save ends)
      - name: Effect
        effect: A creature restrained this way is vertical pulled 2 squares and
          suspended in the air by the snare line. On a successful save, the
          snare is cut or breaks and the creature falls to the ground. The snare
          must be manually reset.
  - type: feature
    feature_type: trait
    name: Upgrade
    icon: ⭐️
    effects:
      - name: Net Trap
        cost: +1 EV
        effect: The snare becomes a net that can wrap up multiple targets. The net has 3
          Stamina and fills an area of 3 squares by 3 squares. The Snare ability
          loses its existing keywords, gains the Area keyword, and targets each
          creature or object in the area. The trap can be triggered by a target
          moving through one specific square, or by requiring multiple squares
          to be moved through. Any creature who makes their save to end the
          restrained effect ends that effect for all targets, who all fall to
          the ground.
  - type: feature
    feature_type: trait
    name: Hidden
    icon: ⭐️
    effects:
      - effect: The snare trap is hidden until triggered or detected.
~~~