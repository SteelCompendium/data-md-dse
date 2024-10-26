```ds-statblock
name: [[Human]] Brawler
ancestry:
- [[Human]]
- Humanoid
roles:
- Brute
level: 1
ev: 16
stamina: 40
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
agility: 1
reason: 0
presence: 0
traits:
- name: Shoot the Hostage
  effect: The brawler takes half damage from attacks if they have a creature or object
    [[Grabbed|grabbed]]. The [[Grabbed|grabbed]] creature or object takes the other half of the damage.
- name: Supernatural Insight
  effect: The brawler can target supernatural creatures and objects within 5 squares,
    even if they don’t have line of effect.
abilities:
- name: Haymaker
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object
  t1: 4 damage; M1 [[Grabbed|grabbed]]
  t2: 7 damage; M2 [[Grabbed|grabbed]]
  t3: 10 damage; M3 [[Grabbed|grabbed]]
  effects:
  - name: Effect
    effect: 'The target has a bane on attempts to escape the [[Grab|grab]]. The brawler has
      edge on this attack if the target is already [[Grabbed|grabbed]]. '
- name: Throw
  type: Maneuver
  cost: 1 Malice
  keywords:
  - —
  distance: Melee 1
  target: One creature [[Grabbed|grabbed]] by the brawler
  effects:
  - name: Effect
    effect: 'Push 5. '

```
