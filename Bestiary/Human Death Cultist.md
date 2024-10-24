```ds-statblock
name: [[Human]] Death Cultist
ancestry:
- [[Human]]
- Humanoid
roles:
- Support
level: 2
ev: 16
stamina: 40
immunities:
- Magic 2
- Psionic 2
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 4
might: 0
intuition: 0
agility: 1
reason: 0
presence: 1
traits: []
abilities:
- name: Death Scythe
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Melee
  - Ranged
  - Weapon
  distance: Reach 1 or Ranged 10
  target: One creature or object
  t1: 4 corruption damage
  t2: 7 corruption damage; [[Weakened|weakened]] (EoT)
  t3: 10 corruption damage; [[Weakened|weakened]] (INU ends)
- name: Rise, My Minions
  type: Maneuver
  cost: 1 VP per minion
  keywords:
  - Area
  distance: 5 burst
  target: One or more dead minions
  effects:
  - name: Special
    effect: Each target must have died during this encounter
  - name: Effect
    effect: Each target returns to life with their full Stamina, but they die at the
      end of the encounter or if the death cultist is killed. If the target dies a
      second time, they can be brought back to life by this ability again.

```
