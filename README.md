# TP_Luigi_M1

## Controls

**Character Movement:**
- Move with **Left Stick**

**Torch/Aiming:**
- Aim flashlight using **Right Stick**
- Torch cannot rotate completely around Player

**Actions:**
- **Flash (B)** Indicate by an left bottom icon
- **Capture ():** Indicate by an left bottom progress bar
---

## Ghost AI Behavior

Ghosts in the game behave differently depending on their state:

**Patrol:**
- Patrolling between random points

**Stunned (after Flash):**
- Freeze in place for a short time
- Wait for the player to initiate capture

**Escape:**
- If the player fails to begin capture, the ghost escapes by running away the player at higher speed

**Capture:**
- When capture begins, the ghost moves around player in a circle
- The ghost tries to escape Player

---

## Capture Mechanic

Capturing a ghost is a challenge that requires the player to manage direction and timing:

- To successfully capture, Player must face the ghost while aiming the flashlight **in the opposite direction** of where the ghost is moving
- A hidden “tug-of-war” system calculates how well the player is aligned with the ghost
  - Good alignment charges the capture
  - Poor alignment slows / looses progress