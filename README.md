# Angry Birds - Split Mechanics Update 🚀

## Overview
A Box2D physics-based clone of Angry Birds built in Lua and LÖVE2D. Players use a slingshot mechanic to launch projectiles into destructible fortresses.

## Custom Features
* **Mid-Air Splitting:** Introduced a new dynamic split ability to the `AlienLaunchMarker`. While the alien is in flight, pressing `Space` splits the projectile into three separate aliens:
  * **Upper Alien:** Travels at a shallower arc.
  * **Middle Alien:** Maintains original trajectory.
  * **Lower Alien:** Travels at a steeper arc.
* **Updated Game Loop Check:** The level transition logic was updated to monitor the velocities of *all* split aliens, ensuring the turn doesn't end until every piece has stopped rolling.
