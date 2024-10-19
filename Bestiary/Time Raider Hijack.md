```ds-statblock
name: [[Time Raider]] Hijack
ancestry:
- Humanoid
- [[Time Raider]]
roles:
- Ambusher
level: 3
ev: 20
stamina: 50
immunities:
- Psychic 5
weaknesses: []
speed: '6'
size: 1M
stability: 0
free_strike: 5
might: 0
intuition: 2
agility: 2
reason: 2
presence: 1
traits:
- name: Foresight
  effect: The hijack doesn’t take a bane on attacks against concealed creatures.
abilities:
- name: Golden Sickles
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Psionic
  - Weapon
  distance: Reach 1
  target: One creature
  t1: 5 damage
  t2: 9 damage; [[Bleeding|bleeding]] (EoT)
  t3: 12 damage; [[Bleeding|bleeding]] (REA ends)
  effects:
  - name: Effect
    effect: 'If the target is [[Bleeding|bleeding]] from this ability, the hijack is hidden from
      the target until that [[Bleeding|bleeding]] ends. '
- name: Psi-Sickle
  type: Maneuver
  keywords:
  - Psionic
  - Ranged
  - Weapon
  distance: Ranged 5
  target: One creature or object
  effects:
  - name: Effect
    effect: 'The hijack psychically latches their sickle onto the target and closes
      the distance between them. If the target has a weight of 4 or higher, the hijack
      moves adjacent to the target. Otherwise, the target is pulled 4 squares toward
      the hijack. '

```
