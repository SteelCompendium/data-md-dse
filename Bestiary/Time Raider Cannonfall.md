```ds-statblock
name: [[Time Raider]] Cannonfall
ancestry:
- Humanoid
- [[Time Raider]]
roles:
- Artillery
level: 3
ev: 18
stamina: 40
immunities:
- Psychic 4
weaknesses: []
speed: '5'
size: 1L
stability: 3
free_strike: 5
might: 0
intuition: ''
agility: 2
reason: 2
presence: 0
traits:
- name: Foresight
  effect: The cannonfall doesn’t take a bane on attacks against concealed creatures.
abilities:
- name: Sunderbuss
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Area
  - Psionic
  - Ranged
  - Weapon
  distance: 3 cube within 10
  target: Each enemy
  t1: 4 sonic damage
  t2: 8 sonic damage; [[Slowed|slowed]] (EoT)
  t3: 10 sonic damage; [[Slowed|slowed]] (EoT); [[Prone|prone]]
  effects:
  - name: Effect
    effect: 'A layer of ground or floor beneath the area that is 1 square deep is
      destroyed. '
- name: Buss Buffer
  type: [[Triggered Action]]
  keywords:
  - Area
  - Psionic
  distance: 5 burst
  target: Each ally
  effects:
  - name: '**Trigger**'
    effect: A creature damages the cannonfall with a ranged ability.
  - name: Effect
    effect: 'The damage is reduced by half for the cannonfall and each target also
      affected by the triggering ability. '

```
