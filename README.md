# BubbleBall

BubbleBall consists of various prefabs and actions which allow you to e. g. fire a burst of bubbles towards a gameobject, have it wrapped around a bubble and fly away.

The bubble shader code is from Seyed Morteza Kamali and freely available, so many thanks and full credit to him for his great work!

## Quick Setup

* create a new Unity 2019.4.2f1 project

* download and import the project from https://bit.ly/BubbleBallSource

* load the demo scene Assets/BubbleBall/_Demo/BubbleBall

* hit play

## Demo

Open the BubbleBall demo scene and hit play. Use the left mousebutton to select the primitives which will make the cannon rotate towards them and fire at them when they are in range.

Here's a demo video of the project:

[![Bubble Ball](https://img.youtube.com/vi/VABkmazYbyA/0.jpg)](https://www.youtube.com/watch?v=VABkmazYbyA)

A gameplay showcase of the asset being used:

[![Bubble Bobble Type Showcase](https://img.youtube.com/vi/Nb_QU-pKRbg/0.jpg)](https://www.youtube.com/watch?v=Nb_QU-pKRbg)

## Package Info

#### Scripts

* BubbleHitAction.cs

  Check the collision of the bubble bullet with a gameobject and wrap that gameobject into a bubble.

  Important: Currently for demonstration purposes the bubble collider reacts to all gameobjects. You need to adapt the code to filter out gameobjects which shouldn't be affected, e. g. consider tags or a layers.

* BubbleTarget.cs

  There are situations where the pivot of the gameobject is on the outer bounds. This makes the wrapped gameobject spin offset, i. e. not in center.
  When this script is attached to the hit gameobject, then the data in there will be used, e. g. optionally that object's pivot instead of the gameobject's. Or you can specify a fixed diameter instead of having it calculated.


#### Prefabs

* BubbleBall

  The bubble that's wrapped around a gameobject.

* BubbleBullet

  A particle system with bubbles which is being used as a bullet. Upon hit detection with a gameobject a bubble is being instantiated and the gameobject is being wrapped into the bubble.

* BubbleBurst

  A particle system with bubbles


## Malbers Integration

If you use this with the Malbers Animals, check the region "Malbers specific" and uncomment the code. This will deactivate various scripts in order to keep the animals in the bubble.

## Planned Features

* consider wind

## Credits

* Seyed Morteza Kamali
  
  Bubble Shader https://github.com/smkplus/Iridescence

 