# HandGesture-Project
Hand Gestures
This template allows you to trigger different effects based on recognized hand gestures. The template uses Hand Gestures to show a stylized picture of a recognized gesture, as well as triggering a sound effect. It provides an easy way to interact with the following gestures (each gesture is seen in the image below):

Template Walkthrough
Let’s take a high level overview of the project. It can be split into three major parts: 

Hand Tracking
Gesture Detection and Emitting Events
Responding to the Events and Triggering Effects
The Hand Tracking part is managed by the Object Tracking component, which is attached to the Orthographic Camera > Hand Tracking Region > Hand Tracking > Hand Center. In addition to tracking the hand, this component can also look for hand gestures.

NOTE

Emitting events is handled by the Hand Gesture Controller object. If you select this object, you can see, in the Inspector panel, that it takes an Object Tracking component and a list of Behavior triggers to emit for each of the recognizable gestures. So that every time the Object Tracking component detects a hand gesture, this script emits the given list of triggers.

T
We can use the Behavior script to respond to the hand gestures events. This template provides two examples of using the Behavior script to respond to detection of a hand gesture:

Instantiating prefabs
Playing sounds
