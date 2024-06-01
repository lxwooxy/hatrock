# hatrock

## Generating data for scientific research

### The quick spiel
Generating visual data to be used for training machine learning models in intuitive physics.

### Details
When we think of human perception and cognition, many aspects of our perception can be chalked up to "intuition". For machines and computer vision, we attempt to recreate this intuition with advanced computational methods in our attempt to teach machines to see the world around us as we do.

In particular, I want to focus on contact information – a key aspect of our perceived physics. Objects in contact with each other will behave differently when force is applied to one of them, compared to when the objects are not in contact. This seems simple enough, but for machines, this vision task is nontrivial, as occlusion and proximity might confuse a vision model attempting to classify objects. In addition, humans can predict contact information. Consider object A moving toward a stationary object B at a fixed rate. If you were viewing this as a video feed, even if the video were cut short (before contact), we can mentally simulate the trajectory of object A, and conclude if contact will happen or not. This task is again, nontrivial for computer vision, as simple feed-forward predictions with pattern recognition (eg. seeing the same event happen before) cannot generalize to the real world with infinite possibilities of scenarios. 

As such, my goal is to generate such scenes computationally, using rendering software like Blender to create a range of common (and some uncommon) objects, Unity3D to animate the scenes, and C# scripting to automate the process of changing the objects (texture, shape, size, color) used in the scenarios, while keeping the rest of the data consistent (video angles, lighting, speed).

My motivation for this task is to explore how computational methods can be used to aid scientific research. With complex tasks like training a vision model to learn intuitive physics, it is time-consuming to create these scenes in real life to train the model. Even though some aspects of manually creating data would help teach a machine to generalize (camera shake, different variations of speed and trajectory), in this project I aim to discover if current deep learning methods have sufficient architecture to capture features from this data to perform comparably with humans. With my proposed method of computationally generating data, it would not be an unthinkable task to create 10,000 videos, each of which can be fed to a machine learning model to train or test it. My hope is to contribute this data to the field of computer science and the cognitive sciences.

### Task Breakdown
In 10 weeks:
[ ] Create 3D models in Blender
[ ] Set up a Unity3D environment for automating rendering
[ ] Writing C# scripts to animate the physics of the scenes
[ ] Writing C# scripts to record the scenes from a set number of viewpoints
[ ] Writing C# scripts to automate swapping out individual variables of the scene (eg. instead of having to manually select Object A and B)
[ ] Hosting the resulting work on Github Pages

Future work:
[ ] Testing data on deep neural networks that claim to understand intuitive physics
[ ] Finetuning model architecture to generalize to the new data
