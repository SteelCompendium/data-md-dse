~~~ds-statblock
name: Goblin Assassin
ancestry:
- Goblin
- Humanoid
roles:
- Ambusher
level: 1
ev: 11
stamina: 20
immunities: []
weaknesses: []
speed: 6 (climb)
size: 1S
stability: 0
free_strike: 3
might: -2
intuition: 0
agility: 1
reason: 0
presence: -2
traits:
- name: Crafty
  effect: The assassin doesn’t provoke opportunity attacks by moving.
- name: Hide While Observed
  effect: The assassin can take the Hide maneuver even while observed, though they
    still must have cover or concealment.
abilities:
- name: Sword
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature or object
  t1: 3 damage
  t2: 5 damage
  t3: 7 damage
  effect: 'If the assassin has an edge or a double edge on the power roll for this
    ability, the ability deals an additional 2 damage. '
- name: Shadow Chains
  type: Action
  roll: AGL RR
  cost: 3 VP
  keywords:
  - Magic
  - Ranged
  - Resistance
  distance: Ranged 10
  target: Three creatures
  t3: 7 corruption damage; restrained (AGL ends)
  t2: 5 corruption damage; restrained (EoT)
  t1: '3 corruption damage '

~~~