---
agility: 1
ancestry:
- Human
- Humanoid
ev: '8'
file_basename: Human Death Cultist
file_dpath: Monsters/Humans/Statblocks
free_strike: 4
intuition: 0
item_id: human-death-cultist
item_index: '162'
item_name: Human Death Cultist
level: 2
might: 0
presence: 2
reason: 0
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster:human-death-cultist
scdc:
- 1.1.1:2:162
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '40'
type: monster
---

~~~ds-statblock
name: Human Death Cultist
level: 2
roles:
  - Platoon Support
ancestry:
  - Human
  - Humanoid
ev: "8"
stamina: "40"
immunities:
  - Corruption 2
  - psychic 2
speed: 5
size: 1M
stability: 0
free_strike: 4
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Supernatural Insight
    effects:
      - effect: The death cultist ignores concealment if it's granted by a supernatural
          effect.
abilities:
  - name: Death Scythe
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 6 corruption damage
        t2: 9 corruption damage
        t3: 12 corruption damage; I < 2 weakened (save ends)
      - effect: The death cultist regains Stamina equal to half the damage dealt.
        cost: 2 Malice
  - name: Rise, My Minions
    icon: ❇️
    cost: 1 Malice per minion
    keywords:
      - Area
    type: Maneuver
    distance: 5 burst
    target: Each dead minion in the area
    effects:
      - effect: Each target who died during this encounter revives with full Stamina.
          They immediately die at the end of the encounter or if the death
          cultist is killed. A target can be revived multiple times by this
          ability.
        name: Effect
~~~