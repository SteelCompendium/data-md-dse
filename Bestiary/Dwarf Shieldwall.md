```ds-statblock
name: [[Dwarf]] Shieldwall
ancestry:
- [[Dwarf]]
- Humanoid
roles:
- Defender
level: 3
ev: 16
stamina: 70
immunities:
- weapon 3
weaknesses: []
speed: '5'
size: 1M
stability: 4
free_strike: 5
might: 2
intuition: 0
agility: 0
reason: 0
presence: 1
traits:
- name: Call to the Wall
  effect: The shieldwall inflicts [[Taunted|taunted]] (EoT) on a creature whenever they deal damage
    to the shieldwall or take damage from the shieldwall.
abilities:
- name: Wide Axe
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  t1: 5 damage; slide 1
  t2: 8 damage; slide 1
  t3: 11 damage; slide 1
  effects:
  - name: Effect
    effect: The shieldwall can shift 1 to remain adjacent to the target. A target
      [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be slid by this attack.
  - name: 3 Malice
    effect: 'The shieldwall targets an additional creature or object. '
- name: Intercepting Shield
  type: Triggered Action
  cost: 1 Malice
  keywords:
  - '-'
  distance: Self
  target: Self
  trigger: A creature attacks an adjacent ally.
  effects:
  - name: Effect
    effect: 'The shieldwall becomes the attack''s target and has +3 defense against
      it. '

```
