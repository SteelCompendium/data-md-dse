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
name: Snare Trap
type: Trap Ambusher
level: 1
ev: "1"
flavor: A rope snare is set to grab a target, leaving them hanging upside down.
stamina: "1"
size: 1S
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a snare trap can make an **Agility
          test**.
        t1: The creature triggers the trap and is affected as if in its space.
        t2: The trap is deactivated but the creature is slowed (EoT).
        t3: The trap is deactivated and doesn't trigger.
  - name: Activate
    icon: ❕
    effects:
      - effect: The snare trap is calibrated to be triggered by creatures or objects of
          a particular size or larger. The trap triggers when a creature or
          object of the appropriate size enters its space.
      - effect: A triggering creature or object ends their movement and is targeted by
          the **Snare** ability.
        name: Effect
  - name: Snare
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Free triggered action
    distance: Melee 0
    target: The triggering creature or object
    trigger: A creature or object of the appropriate size enters the trap's space.
    effects:
      - roll: Power Roll + 2
        t1: The target shifts 1 square away from the snare.
        t2: 1 damage; A < 1 restrained (save ends)
        t3: 3 damage; A < 2 restrained (save ends)
      - effect: A creature restrained this way is vertical pulled 2 squares and
          suspended in the air by the snare line. On a successful save, the
          snare is cut or breaks and the creature falls to the ground. The snare
          must be manually reset.
        name: Effect
  - name: Upgrade
    icon: ⭐️
    effects:
      - effect: "**Net Trap (+1 EV)** The snare becomes a net that can wrap up multiple
          targets. The net has 3 Stamina and fills an area of 3 squares by 3
          squares. The Snare ability loses its existing keywords, gains the Area
          keyword, and targets each creature or object in the area. The trap can
          be triggered by a target moving through one specific square, or by
          requiring multiple squares to be moved through. Any creature who makes
          their save to end the restrained effect ends that effect for all
          targets, who all fall to the ground."
  - name: Hidden
    icon: ⭐️
    effects:
      - effect: The snare trap is hidden until triggered or detected.
~~~