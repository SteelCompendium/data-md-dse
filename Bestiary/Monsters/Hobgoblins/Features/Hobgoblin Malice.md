---
file_basename: Hobgoblin Malice
file_dpath: Monsters/Hobgoblins/Features
item_id: hobgoblin-malice-malice-features
item_index: '20'
item_name: Hobgoblin Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:hobgoblin-malice-malice-features
scdc:
- 1.1.1:2.2:20
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Hobgoblin Malice
type: Malice Features
flavor: At the start of any hobgoblin's turn, you can spend Malice to activate
  one of the following features.
stats: []
features:
  - name: Goblin Malice Features
    icon: ⭐️
    cost: 3-7 Malice
    effects:
      - effect: The hobgoblin activates a Malice Feature available to goblins.
  - name: Operation Goblin Mode
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Each goblin in the encounter gains a +3 bonus to speed until the end of
          the round.
  - name: Operation Tactical Swarm
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: Each hobgoblin in the encounter shifts up to their speed and can take
          the Defend main action.
  - name: Operation Earth Sear
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Until the end of the round, the ground throughout the encounter map
          becomes blazing hot. Any enemy takes 1 fire damage for each square of
          the ground they enter. Any enemy who ends their turn on the ground has
          fire weakness 2 until the start of their next turn.
~~~