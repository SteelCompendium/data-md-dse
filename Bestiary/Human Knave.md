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
might: 2
intuition: 0
agility: 0
reason: 1
presence: 0
traits:
- name: I’m Your Enemy
  effect: The knave can make a [[Free Strike|free strike]] against an adjacent creature they have
    [[Taunted|taunted]] whenever the creature deals damage to a creature other than the knave.
- name: Overwhelm
  effect: An enemy who starts their turn adjacent to the knave can’t shift.
- name: Supernatural Insight
  effect: The knave can target supernatural creatures and objects within 5 squares,
    even if they don’t have line of effect.
abilities:
- name: Morningstar & Javelin
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 5
  target: One creature or object
  t1: 4 damage; M1 the target has a bane on their next attack
  t2: 7 damage; M2 the target has a bane on their next attack
  t3: 10 damage; M3 the target has a double bane on their next attack
  effects:
  - name: Effect
    effect: '[[Taunted]] (EoT). '

```
