---
file_basename: Ashen Hoarder Malice
file_dpath: Monsters/Ashen Hoarder/Features
item_id: ashen-hoarder-malice-malice-features
item_index: '27'
item_name: Ashen Hoarder Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:ashen-hoarder-malice-malice-features
scdc:
- 1.1.1:2.2:27
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Ashen Hoarder Malice
type: Malice Features
flavor: At the start of an ashen hoarder's turn, you can spend Malice to
  activate one of the following features.
stats: []
features:
  - name: Relentless Strikes
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: The ashen hoarder moves up to their speed and can make a free strike
          against two targets.
  - name: Blade Wall
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: The ashen hoarder summons a 10 wall of bones and blades into unoccupied
          squares within 5 squares of them. Each square of the wall has 5
          Stamina. An enemy who comes adjacent to the wall for the first time in
          a round or starts their turn there takes 3 damage.
  - name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The ashen hoarder takes an additional main action on their turn. They
          can use this feature even if they are dazed.
  - name: Bone Storm
    icon: 🔳
    cost: 7 Malice
    effects:
      - effect: The ashen hoarder launches bone lances into the air, raining them down
          on enemies and impaling those unlucky enough to be on the receiving
          end. Each enemy within 20 squares of the ashen hoarder makes an
          **Agility test**.
        t1: 14 damage; restrained and bleeding (save ends)
        t2: 11 damage; bleeding (EoT)
        t3: 6 damage
~~~