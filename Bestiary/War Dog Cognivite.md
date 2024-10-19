```ds-statblock
name: War Dog Cognivite
ancestry:
- Humanoid
- War Dog
roles:
- Defender
level: 1
ev: 11
stamina: 25
immunities: []
weaknesses: []
speed: 5 ([[Fly|fly]])
size: 1M
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 1
reason: 0
presence: 1
traits:
- name: Loyalty Collar
  effect: When the cognivite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Synlirii Grafts
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Area
  - Psionic
  distance: 1 burst
  target: Each enemy
  t1: 2 psychic damage; vertical slide 1
  t2: 4 psychic damage; vertical slide 2
  t3: '5 psychic damage; vertical slide 3 '
- name: Posthumous Promotion
  type: Maneuver
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One war dog with a loyalty collar
  effects:
  - name: Effect
    effect: 'The target’s loyalty collar detonates, killing them instantly. '
- name: The Voice (Maneuver) ◆ 1 VP
  keywords:
  - Psionic
  - Ranged
  distance: Ranged 10
  target: Each enemy
  effects:
  - name: Effect
    effect: 'The cognivite chooses an ally within 10 squares, then chooses whether
      each target is [[Taunted|taunted]] by the ally (EoT) or has a double bane on attacks against
      the ally (EoT). The same choice must be made for all targets. '

```
