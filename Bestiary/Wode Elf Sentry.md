```ds-statblock
name: Wode Elf Sentry
ancestry:
- Fey
- Humanoid
- Wode Elf
roles:
- Support
level: 1
ev: 13
stamina: 30
immunities: []
weaknesses: []
speed: '7'
size: 1M
stability: 0
free_strike: 3
might: 0
intuition: 0
agility: 2
reason: 0
presence: 1
traits:
- name: Masking Glamor
  effect: The sentry immediately [[Hide|hides]] at the end of their turn while in cover or
    concealment, even if they are observed.
abilities:
- name: Tracer Longbow
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 10
  target: 1 creature or object
  effects:
  - roll: 2d10 + 2
    t1: 3 damage; A2 marked (save ends)
    t2: 5 damage; A3 marked (save ends)
    t3: 7 damage; marked (save ends)
  - name: Effect
    effect: Allies have **+1** on attacks and abilities against marked creatures and
      objects.
  - name: 3 Malice
    effect: 'The sentry targets two additional creatures or objects. '
- name: Death Blossom
  type: Maneuver
  cost: 2 Malice
  keywords:
  - Area
  - Weapon
  distance: 5 burst
  target: All marked enemies
  effects:
  - name: Effect
    effect: '3 damage. '

```
