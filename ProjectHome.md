# Demo Project #
## A sample setup for Android games ##

This project is intended as an introduction to graphics and physics-animation, particularly on Android.

This is a basic setup that illustrates how a physics engine can be integrated with OpenGL to achieve high performance graphics with real-world physics animation.

Some knowledge of physics, JNI and OpenGL is recommended.

The setup features an Android application demonstrating two dynamic shapes that bounce around the screen affected by the phone's accelerometer.


## 2D Physics ##

Using a physics engine, virtual shapes can be animated and interacted with each other, to simulate real-world movement.

All physics is based on either of two Box2D versions:
  * The original Box2D was written in C++ by Erin Catto. See http://box2d.org/.
  * JBox2D, Box2D's Java-port. See http://jbox2d.org/.


This project includes the code to glue together Box2D with Android through Java's JNI interface.

The game-core of the project interacts with a Box2D interface which either be an instance of JBox2D or JNIBox2D. This physics-engine configuration can be chosen at run-time.


## Graphics ##

Graphics is drawn using OpenGL | ES. The one primitive shape used is a rectangle. Attempts have been made to make it easy to extend to other types of shapes.
