---
file_basename: Devil Malice
file_dpath: Monsters/Devils/Features
item_id: devil-malice-malice-features
item_index: '36'
item_name: Devil Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:devil-malice-malice-features
scdc:
- 1.1.1:2.2:36
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Devil Malice
type: Malice Features
flavor: At the start of any devil's turn, you can spend Malice to activate one
  of the following features.
stats: []
features:
  - name: Bureaucratic Tape
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: One devil acting this turn uses a signature ability against an adjacent
          creature. On a tier 3 outcome, the target of the ability has a double
          bane on strikes (save ends).
  - name: Underhanded Tactics
    icon: ⭐️
    cost: 5+ Malice
    effects:
      - effect: One or two devils can teleport to a space adjacent to one or more
          creatures who aren't hidden and make a free strike. For each 2
          additional Malice spent on this feature, one additional devil can
          teleport.
  - name: Read the Small Print
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Each enemy in the encounter is subject to a bad deal proposed by the
          devils. An enemy must choose between having damage weakness 5 or
          taking a bane on power rolls. The bad deal lasts until the end of the
          encounter.
  - name: Devil Temptations
    effects:
      - effect: >-
          Although some devils enjoy comfort and opulence for their own sake,
          they primarily use treasure as bargaining chips in fiendish compacts:
          bait on the devils' infernal barbs.


          Even more sinister than a prize won in a devil's hard bargain is a
          gift freely given by a devil. The advantages of such a gift are
          conditional, lasting only until the devil revokes it at some
          inconvenient time.

          The following are samples of the wonders that a devil can offer-to
          only the most discriminating customers, of course. A devil might only
          have two or three of these items available for trade, but others (such
          as an archdevil's wing) can be won by force. See *Draw Steel: Heroes*
          for more information about how these items can be used by heroes.
      - effect: An archdevil's wing, archdevil's blood, soul chalk, a wide selection of
          true names
        name: Components
      - effect: Notes in Anjali for the Devil's Bargain armor enhancement or a
          Hellcharger Helm, notes in Hyrallic for a Mediator's Charm
        name: Project Sources
      - effect: Diabolist, Maestro
        name: Titles
      - effect: G'Allios Visiting Card, Thief of Joy
        name: Treasures
      - effect: Each hero can earn 1 wealth in exchange for a small favor
        name: Wealth
~~~