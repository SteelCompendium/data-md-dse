```ds-statblock
name: [[Human]] Knave
ancestry:
- [[Human]]
- Humanoid
roles:
- Defender
level: 2
ev: 18
stamina: 50
immunities:
- Magic 2
- Psionic 2
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 4
might: 1
intuition: 0
agility: 0
reason: 0
presence: 0
traits:
- name: Overwhelm
  effect: A creature who starts their turn adjacent to the knave can’t shift.
abilities:
- name: Morningstar & Javelin
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Reach 1 or Ranged 5
  target: One creature or object
  t1: 4 damage; [[Taunted|taunted]] (EoT)
  t2: 7 damage; [[Taunted|taunted]] (EoT)
  t3: 10 damage; [[Taunted|taunted]] (EoT)
  effects:
  - name: Effect
    effect: 'If an adjacent target [[Taunted|taunted]] by this ability harms a creature other
      than the knave, the knave can make a [[Free Strike|free strike]] against the [[Taunted|taunted]] creature
      as a free triggered action. '

```
