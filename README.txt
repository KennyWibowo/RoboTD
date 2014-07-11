Brief summary on what's been done so far.


LAYERS
-Remember that layer 0 is background layer. So new objects go on layer 1.
---

ENEMIES
(generic). they travel along the path until they reach the exit

Properties:
-Direction: direction of movement
-Health: health. If health <= 0, get destroyed.

---

ENEMY COLLISION
-At the moment, there are four tile blocks to shift the enemy's direction upon touch. If an enemy collides with a down-turn block, they will begin moving down immediately upon collision. Same for other directions.

---

TURRET
-Generic turret. Targets nearest enemy and shoots them with a bullet. Altering it to target strongest/weakest enemy in range is trivial. Attacking enemy nearest the exit is a little bit more difficult.

---

Properties:
-cooldown: cooldown between shots
-range: range
-local variable maxCD: constant that stores initial cooldown

---

SPAWNER
-Place that spawns generic enemies.

Properties:
-cooldown: cooldown between spawns
-NumberOfSpawns: number of spawns left

---

BULLET
-shoots enemies

Properties:
-life: time until it automatically gets destroyed
-damage: damage it deals to enemies

---

MENUTURRET
-turret that appears in the menu. Drag & Drop onto a non-road place that's not already occupied by a turret to place a new turret.

---

ROAD:
-path that enemies travel on. Can't place turrets here.

---

WALL:
-can place turrets here.




GOALS:
HIGH PRIORITY: figuring out how to zoom out the camera so you can actually see a larger portion of the screen