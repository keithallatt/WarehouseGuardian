# Major Classes and Functions:

Since we're doing our project in Unity, the project isn't really divided into classes and functions. Instead we have Assets and Components.

We've made a few Prefabs for this project, including one for enemies, one for boxes, and one for the box endpoints. Each one has various components attached to them, but the most intricate is the Enemy prefab.

### Enemy Prefab

The Enemy prefab has a few different components that make it a good example of our work. First of all, since it is a prefab, we need a way of dictating the enemies movement. This was accomplished by using public fields in the custom movement script. Public fields in unity C# scripts translate to text boxes in the Unity Inspector window, allowing us to input each monsters path and speed. Each Enemy instance also has a box collider component which allows it to interact with the player and with the boxes. Finally, each Enemy instance uses 4 animation clips and an animation controller to control the direction the Enemy faces on screen. 

### Box Prefab

The Box prefab is a little more simple. It merely contains a box collider to be tangible to other entities and allows it to be pushed in any direction by the player. 

### Box Endpoint Prefab

The Box Endpoint prefab will contain a script to detect when a box is on top of them, and when all box endpoints detect a box, the player will be sent to the next level.
