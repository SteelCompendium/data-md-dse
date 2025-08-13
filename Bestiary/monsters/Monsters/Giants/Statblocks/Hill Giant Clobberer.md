---
file_basename: Hill Giant Clobberer
file_dpath: Monsters/Giants/Statblocks
item_id: hill-giant-clobberer
item_index: '88'
item_name: Hill Giant Clobberer
scc:
  - mcdm.monsters.v1:monster:hill-giant-clobberer
scdc:
  - 1.1.1:2:88
source: mcdm.monsters.v1
type: monster
---

###### Hill Giant Clobberer

|     Giant, Hill Giant      |            -            |       Level 7        |       Elite Brute       |         EV 36          |
| :------------------------: | :---------------------: | :------------------: | :---------------------: | :--------------------: |
|      **4**<br/> Size       |    **6**<br/> Speed     | **200**<br/> Stamina |  **5**<br/> Stability   | **8**<br/> Free Strike |
| **Damage 3**<br/> Immunity | **Climb**<br/> Movement |          -           | **-**<br/> With Captain | **-**<br/> Weaknesses  |
|     **+4**<br/> Might      |   **-1**<br/> Agility   |  **-1**<br/> Reason  |  **-1**<br/> Intuition  |  **-1**<br/> Presence  |

<!-- -->
> 🗡 **Clobberin' Club (Signature Ability)**
>
> | **Charge, Melee, Strike, Weapon** |                 **Main action** |
> | --------------------------------- | ------------------------------: |
> | **📏 Melee 3**                    | **🎯 Two creatures or objects** |
>
> **Power Roll + 4:**
>
> - **≤11:** 12 damage
> - **12-16:** 17 damage; prone
> - **17+:** 21 damage; prone
>
> **Effect:** A target who is already prone takes an extra 12 damage.

<!-- -->
> 🗡 **Stomp (3 Malice)**
>
> | **Melee, Strike, Weapon** |               **Main action** |
> | ------------------------- | ----------------------------: |
> | **📏 Melee 1**            | **🎯 One creature or object** |
>
> **Power Roll + 4:**
>
> - **≤11:** 14 damage; prone
> - **12-16:** 20 damage; prone; M < 3 can't stand (save ends)
> - **17+:** 25 damage; prone; M < 4 can't stand (save ends)
>
> **Effect:** In suitably soft ground, the target is entrenched in a 2-square deep hole.

<!-- -->
> ❇️ **Hill Quake**
>
> | **Area**       |                  **Maneuver** |
> | -------------- | ----------------------------: |
> | **📏 3 burst** | **🎯 Each enemy in the area** |
>
> **Effect:** Each target must make either a **Might test** or an **Agility test**.
>
> - **≤11:** 6 damage; vertical push 3
> - **12-16:** 2 damage; vertical push 2
> - **17+:** Push 2
>
> **Effect:** The clobberer can choose to fall prone in order to double the forced movement distance.

<!-- -->
> ❗️ **You Ain't Getting Away**
>
> | **Melee**      |           **Triggered action** |
> | -------------- | -----------------------------: |
> | **📏 Melee 3** | **🎯 The triggering creature** |
>
> **Trigger:** A creature within distance moves or shifts away from the clobberer.
>
> **Effect:** The target makes an Agility test.
>
> - **≤11:** Grabbed, and the target takes a bane on the Escape Grab maneuver
> - **12-16:** Grabbed
> - **17+:** No effect
>
> **2 Malice:** A target who would be grabbed by this ability is instead either vertical pushed up to 5 squares; or they take 5 damage, are knocked prone, and can't stand until the end of their next turn.

<!-- -->
> ⭐️ **Destructive Path**
>
> The clobberer automatically destroys any mundane size 1 objects in their path when they move or are forced moved. They can break through any mundane wall made of wood, stone, or a similarly sturdy material this way as long as the wall is 2 squares thick or less.

<!-- -->
> ⭐️ **Distracted**
>
> Whenever the clobberer targets a creature or object with an ability, any enemy within distance of the ability can use a free triggered action to distract the clobberer. The clobberer targets that enemy instead
