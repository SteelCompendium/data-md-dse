```ds-statblock
name: Cradle Credenza
ancestry:
- Construct
- High Elf
roles:
- Support
level: 2
ev: 15
stamina: 35
immunities:
- weapon 3
weaknesses: []
speed: '4'
size: '2'
stability: 3
free_strike: 4
might: 2
intuition: 0
agility: 0
reason: 0
presence: 2
traits:
- name: [[Defend]] the Books
  effect: Each ally within 5 of a creature that attacks the cradle credenza can make
    a [[Free Strike|free strike]] against them.
abilities:
- name: Book Wall
  type: Action
  cost: Signature
  keywords:
  - Area
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The cradle credenza''s speed becomes 0, and they extend themselves into
      a 5-wall until the start of their next turn. Allies adjacent to the wall at
      the start of their turn regain 5 Stamina and can apply the Magic keyword to
      their weapon abilities until the end of their turn. '
- name: Elemental Chaos
  type: Action
  cost: 2d10 + 2
  keywords:
  - Area
  - Magic
  distance: 2 burst
  target: All enemies
  t1: 2 fire damage; 2 cold damage; 2 lightning damage
  t2: 3 fire damage; 3 cold damage; 3 lightning damage; push 3

```
