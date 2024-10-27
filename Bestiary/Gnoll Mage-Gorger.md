```ds-statblock
name: Gnoll Mage-Gorger
ancestry:
- Fiend
- Gnoll
roles:
- Hexer
- Minion
level: 2
ev: 4
stamina: 8
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 1
free_strike: 2
might: 2
intuition: 0
agility: 1
reason: -1
presence: 0
traits:
- name: Death Frenzy
  effect: Whenever an ally within 5 is reduced to 0 Stamina, the mage-gorger moves
    up to their speed and makes a [[Free Strike|free strike]].
abilities:
- name: Wizard Ripper
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Melee
  distance: Melee 1
  target: 1 creature or object per minion
  t1: 2 acid damage
  t2: 3 cold damage
  effects:
  - name: Effect
    effect: 'The target has a bane on their next resistance roll until the start of
      the mage-gorger''s next turn. '

```
