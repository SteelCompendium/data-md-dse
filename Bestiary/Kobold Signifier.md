```ds-statblock
name: Kobold Signifier
ancestry:
- Humanoid
- Kobold
roles:
- Support
level: 1
ev: 8
stamina: 15
immunities: []
weaknesses: []
speed: '5'
size: 1S
stability: 0
free_strike: 1
might: 0
intuition: 0
agility: 1
reason: 0
presence: 2
traits:
- name: Upholding High Standards
  effect: Allies within 5 of the signifier have an edge and resistance. If the signifier
    is killed, a minion from their squad can retrieve the signum and replace their
    stat block with the signifier stat block.
- name: Shield? Shield!
  effect: The signifier has increased Stability by 1 and can act as cover for allies
    when adjacent to an ally who also has this trait.
abilities:
- name: Signum
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  t1: 2 damage
  t2: 4 damage
  effects:
  - name: Effect
    effect: An ally within 10 can shift their speed, as long as they end their movement
      adjacent to an ally.
  - name: 2+ Malice
    effect: '1 additional ally can shift for every 2 malice spent. '
- name: Glory to the Legion
  type: Maneuver
  cost: 5 Malice
  keywords:
  - Area
  distance: 5 burst
  target: All allies in the burst
  effects:
  - name: Effect
    effect: 'Each target regains 5 Stamina. '

```
