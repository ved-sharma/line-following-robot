# Autonomous Line-following Robot
Other than writing code, I enjoy building things as a hobby. I made a line following robot using DIY components and open-source Arduino platform. The purpose of this robot was to transport stuff between two users back and forth. Robot moves from point A to point B along a line defined by the black sticky tape on the floor, while avoiding collision with a passing object (e.g. a person) in its way. When reaching the end, robot stops and waits for the user to pick up the stuff (a basket with things in it). Once user replaces the basket back on the robot, it turns back and moves towards the other end.

The whole project took around 5-6 months (few mins/hours here and there at night and weekends), where I taught myself various aspects of robot design - mechanical engineering, electronics and computer programming. I chose Arduino microcontroller for the brain of the robot, since it's an open-source platform with tons of resources available online and YouTube videos. The most challenging part in this project for me was the physical design of the robot itself, with the constrains on weight distribution, power management and its stability.

I utilized three sensors in the robot:

An array of 3 reflectance sensors on the underside of the robotic platform to detect and follow the line.
An ultrasonic sensor mounted on a servo motor at the front to detect and avoid collision with an object - a moving person.
Light-dependent resistor (LDR) embedded in the top platform to detect when the user lifts the basket off and puts it back, signaling that robot needs to turn back and move towards the other end.
Following are a series of videos describing the robot evolution while I implemented and optimized different features:

#### Version #1:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=7gEEXGK_PbU" target="_blank">
 <img src="https://res.cloudinary.com/marcomontalbano/image/upload/v1596294950/video_to_markdown/images/youtube--7gEEXGK_PbU-c05b58ac6eb4c4700831b2b3070cd403.jpg" alt="Line following Robot, version 01" width="240" height="180" border="10" />
</a>

#### Version #2: 
Moved wheels close to the center, which led to better weight distribution and improved robot's agility.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=8QIpKqybj4Y" target="_blank">
 <img src="https://res.cloudinary.com/marcomontalbano/image/upload/v1596335773/video_to_markdown/images/youtube--8QIpKqybj4Y-c05b58ac6eb4c4700831b2b3070cd403.jpg" alt="Line following Robot, version 02" width="240" height="180" border="10" />
</a>

#### Version #3:
Implemented a series of changes:
1. Better power management by having separate battery packs for the Arduino board and the motors.
2. Refined sensors and the code for the robot to follow a thinner line.
3. Added code for the robot to stop at the "T" intersection.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=9Ct8vHiWc-Q" target="_blank">
 <img src="https://res.cloudinary.com/marcomontalbano/image/upload/v1596336902/video_to_markdown/images/youtube--9Ct8vHiWc-Q-c05b58ac6eb4c4700831b2b3070cd403.jpg" alt="Line following Robot, version 03" width="240" height="180" border="10" />
</a>

#### Version #4 (Final design):
Added following features:
1. Added the four legs and top platform; embedded the LDR sensor into the top platform, which senses the basket movement.
2. Got all three sensors (LDR  sensor at the top, ultrasonic object avoidance sensor at the front and reflectance sensors at the bottom) to work together in the code.

Robot is working as expected. If a person comes in the way, robot stops and waits until the path is cleared. Robot stops at the end of the line (T intersection), waits for the user to pick up the basket. When user puts the basket back on the platform, robot turns back and starts moving towards the other end.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=npnqdeAV6AY" target="_blank">
 <img src="https://res.cloudinary.com/marcomontalbano/image/upload/v1596335773/video_to_markdown/images/youtube--npnqdeAV6AY-c05b58ac6eb4c4700831b2b3070cd403.jpg" alt="Line following Robot, version 04" width="240" height="180" border="10" />
</a>

