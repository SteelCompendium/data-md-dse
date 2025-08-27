---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '6'
file_basename: Gunge
file_dpath: Monsters/Demons/Statblocks
free_strike: 2
intuition: 2
item_id: gunge
item_index: '272'
item_name: Gunge
level: 4
might: 3
presence: -1
reason: 1
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:gunge
scdc:
- 1.1.1:2:272
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '25'
type: monster
---

```ds-statblock
name: Gunge
level: 4
roles:
  - Horde Controller
ancestry:
  - Abyssal
  - Demon
ev: "6"
stamina: "25"
weaknesses:
  - Holy 5
speed: 6
size: "3"
stability: 0
free_strike: 2
might: 3
agility: 2
reason: 1
intuition: 2
presence: -1
traits:
  - name: Lethe
    effects:
      - effect: While the gunge is winded, they gain an edge on strikes, and any strike
          made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the gunge can't be hidden from them.
abilities:
  - name: Bilious Expulsion
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Main action
    distance: 1 burst, or 3 cube within 5
    target: One creature or object in the area
    effects:
      - roll: Power Roll + 3
        t1: 5 acid damage; M < 1 slowed (save ends)
        t2: 7 acid damage; M < 2 slowed (save ends)
        t3: 9 acid damage; M < 3 restrained (save ends)
      - effect: The ground and any surfaces in the area pool with slime. The slime is
          difficult terrain for enemies, and any enemy is bleeding while in the
          area.
        name: Effect
  - name: Spew Slide
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    type: Free triggered action
    distance: Self
    target: Self
    trigger: The gunge takes damage from a melee strike.
    effects:
      - effect: The gunge vomits with great force, letting them shift up to their speed
          and ignore any additional effects from the strike. The space the gunge
          occupied before the shift is covered in slime that is difficult
          terrain for enemies. Additionally, any enemy is bleeding while in the
          slime.
        name: Effect
```