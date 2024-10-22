```ds-statblock
name: [[Time Raider]] Armiger
ancestry:
- Humanoid
- [[Time Raider]]
roles:
- Defender
level: 3
ev: 21
stamina: 60
immunities:
- Psychic 5
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 5
might: 0
intuition: ''
agility: 2
reason: 2
presence: 0
traits:
- name: Foresight
  effect: The armiger doesn’t take a bane on attacks against concealed creatures.
- name: Kuran’zoi Heraldry
  effect: While any [[Time Raider|time raider]] starts their turn with line of effect to the armiger,
    that [[Time Raider|time raider]] can end one condition affecting them.
abilities:
- name: Serrated Saber
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Psionic
  - Weapon
  distance: Reach 1
  target: One creature or object
  t1: 5 damage
  t2: 8 damage; [[Weakened|weakened]] (EoT)
  t3: 11 damage; [[Weakened|weakened]] (REA ends)
  effects:
  - name: Effect
    effect: 'The target takes a bane on the next attack they make before the start
      of the armiger’s next turn. '
- name: Shared Sickness
  type: [[Triggered Action]]
  cost: REA RR
  keywords:
  - Psionic
  - Ranged
  - Resistance
  distance: Ranged 20
  target: Triggering creature
  t1: 11 poison damage
  t2: 8 poison damage
  t3: '5 poison damage '
  effects:
  - name: '**Trigger**'
    effect: 'A creature deals damage to any ally of the armiger to whom the armiger
      has line of effect. '

```
