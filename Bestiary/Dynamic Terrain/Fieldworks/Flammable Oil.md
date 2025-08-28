---
file_basename: Flammable Oil
file_dpath: Dynamic Terrain/Fieldworks
item_id: flammable-oil-level-1-trap-ambusher
item_index: '07'
item_name: Flammable Oil (Level 1 Trap Ambusher)
scc:
- mcdm.monsters.v1:dynamic-terrain.fieldwork:flammable-oil-level-1-trap-ambusher
scdc:
- 1.1.1:4.3:07
source: mcdm.monsters.v1
type: dynamic-terrain/fieldwork
---

~~~ds-featureblock
name: Flammable Oil
type: Trap Ambusher
level: 1
ev: 2 per 10 x 10 patch
flavor: A patch of flammable oil or pitch on the ground is ready to be ignited.
stamina: "-"
size: One or more squares
stats: []
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a patch of flammable oil can make
          an **Agility test**.
        t1: The creature ignites the oil and is affected as if in its area.
        t2: The oil temporarily ignites before safely burning out, and the creature
          takes 3 fire damage and is burning (save ends).
        t3: The oil is rendered safe and can't be ignited.
  - name: Activate
    icon: ❕
    effects:
      - effect: A creature or object in a square of oil takes fire damage, or a creature
          or object enters a square of burning oil or starts their turn there.
      - effect: The triggering creature or object takes 3 fire damage and is burning
          (save ends). A burning creature takes 1d6 fire damage at the start of
          each of their turns. A burning object takes 1d6 fire damage at the end
          of each round.
        name: Effect
  - name: Upgrade
    icon: ⭐️
    effects:
      - effect: "**Concealed Oil (+1 EV)** The oil is hidden until it ignites."
  - name: Allied Awareness
    icon: ⭐️
    effects:
      - effect: Allies who have weapons are equipped with torches. Any ally can use a
          maneuver to throw a torch up to 5 squares and ignite the flammable
          oil.
~~~