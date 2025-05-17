# HIGHJUMP
Allows the player to jump higher than normal using different methods.

**Modes**

**Damage**
Uses damage knockback to launch the player upward.

**Vanilla**
Applies a simple jump boost similar to vanilla effects.

## ModeValues

**AutoDisable**
Disables the module automatically after the jump.

**Height**
Sets how high the jump should be.

Vanilla jump motion is 0.42. 


```mermaid
graph LR
  classDef motionY fill:#f9f,stroke:#333,stroke-width:2px,color:#000

  A0[MotionY: 0.0<br>Height: 0.00 blocks]:::motionY
  A1[MotionY: 0.2<br>Height: 0.25 blocks]:::motionY
  A2[MotionY: 0.4<br>Height: 1.00 blocks]:::motionY
  A3[MotionY: 0.6<br>Height: 2.25 blocks]:::motionY
  A4[MotionY: 0.8<br>Height: 4.00 blocks]:::motionY
  A5[MotionY: 1.0<br>Height: 6.25 blocks]:::motionY
  A6[MotionY: 1.2<br>Height: 9.00 blocks]:::motionY
  A7[MotionY: 1.5<br>Height: 14.06 blocks]:::motionY
  A8[MotionY: 2.0<br>Height: 25.00 blocks]:::motionY

  A0 --> A1 --> A2 --> A3 --> A4 --> A5 --> A6 --> A7 --> A8

