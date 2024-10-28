```ds-statblock
name: High Elf Deathtouch
ancestry:
- Fey
- High Elf
- Humanoid
roles:
- Artillery
level: 2
ev: 14
stamina: 25
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 5
might: 2
intuition: 0
agility: 0
reason: 1
presence: 1
traits:
- name: Otherworldly Grace
  effect: At the start of their turn, the deathtouch can turn the duration of one
    save ends effect they suffer from into EoT.
abilities:
- name: Heartpiercer
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Ranged
  - Weapon
  distance: Ranged 10
  target: 1 creature
  t1: 5 damage; R1 deathtouched (save ends)
  t2: 8 damage; R2 deathtouched (save ends)
  t3: 11 damage; R3 deathtouched (save ends)
  effects:
  - name: Effect
    effect: A creature gains a new condition at the end of each turn while deathtouched,
      receiving [[Bleeding|bleeding]] at the end of their first turn, [[Slowed|slowed]] at the end of their
      second turn, and [[Restrained|restrained]] at the end of their third turn. When no longer deathtouched,
      all the conditions imposed by it end.
  - name: 5 Malice
    effect: 'The ability gains the Area keyword, the distance becomes 3 cube within
      10, and it targets all creatures in the cube. '
- name: Kiss of Death
  type: Maneuver
  keywords:
  - Magic
  distance: Melee 1
  target: 1 ally
  effects:
  - name: Effect
    effect: 'The target''s speed increases by 5 and they cannot get results lower
      than tier 3 on their power rolls. The target immediately dies at the end of
      their next turn. '

```
