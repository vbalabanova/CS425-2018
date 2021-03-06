# CS425 Programming Assignment 1: Movin’

## Due: September 16th (Sunday) 2018 at 11:59 pm

## Objective:

Understand the basics of animating a game character, including playing back animation clips and positioning and orienting the character. This framework will be used in future assignments. This assignment should be done in both OGRE and Unity. 

## Tasks:

Create a program so that the charactor follows a list of randomly generately waypoints. As the charactor walks or stops, the corresponding animation clips should be used. Please remember that this is an individual programming assignment. 

### OGRE Tasks (70 pts):
1. Read pa01.cpp/h. **There is a task and 10 pts in this file**
2. Read Agent.cpp/h. **There are 3 tasks and 60 pts in this file**
   - The Agent.cpp/h code provided includes the required variables and method declarations in the Agent class. Use it to setup your charactor. 
   - The Agent constructor includes a for loop that adds 10 waypoints onto the agent’s mWalkList.
   - The update method of the Agent class includes the necessary call to updateLocomote
3. You will need to fill in code for the **updateLocomotion method** of the Agent class.
4. While moving between the points, the character should display the run animation (top and base) and be properly oriented.
5. After the character reaches the last point, it should automatically switch to the idle animation (top and base) and continue displaying this idle behavior.
6. Your character should NOT keep looping between the points.

### Unity Tasks (30 pts):
1. Create a Unity project that demonstrates the same charactor and animations as your OGRE program. It is fine that the waypoints are different from OGRE's waypoints. This means you must have
    - A charactor following a list of 10 randomly created waypoints
    - The charactor must be displaying running and stopping animations.

### Notes:
- You are free to use your own mesh and animations, as long as it uses two animation clips, namely running and stopping, and both OGRE and Unity should use the same charactor.

## How to Submit:
1. For the OGRE part, remove "build" fold and submit everything else (including CMakeLists.txt) 
2. For the Unity part, video capture the screen showing the animation in mp4 format, and save it as your_gmu_id_PA1.mp4 (mp4, m4a, m4v, ...) 
3. Put everything in the corresponding folder and zip them into your_gmu_id_PA1.zip, e.g., jsmith_PA1.zip, and then submit the zip file on Blackboad.
