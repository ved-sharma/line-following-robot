# Autonomous Line-following Robot
###Other than writing code, I enjoy building things as a hobby. I made a line following robot using DIY components and open-source Arduino platform. The purpose of this robot was to transport stuff between two users back and forth. Robot moves from point A to point B along a line defined by the black sticky tape on the floor, while avoiding collision with a passing object (e.g. a person) in its way. When reaching the end, robot stops and waits for the user to pick up the stuff (a basket with things in it). Once user replaces the basket back on the robot, it turns back and moves towards the other end.

###The whole project took around 5-6 months (few mins/hours here and there at night and weekends), where I taught myself various aspects of robot design - mechanical engineering, electronics and computer programming. I chose Arduino microcontroller for the brain of the robot, since it's an open-source platform with tons of resources available online and YouTube videos. The most challenging part in this project for me was the physical design of the robot itself, with the constrains on weight distribution, power management and its stability.

###I utilized three sensors in the robot:

###An array of 3 reflectance sensors on the underside of the robotic platform to detect and follow the line.
###An ultrasonic sensor mounted on a servo motor at the front to detect and avoid collision with an object - a moving person.
###Light-dependent resistor (LDR) embedded in the top platform to detect when the user lifts the basket off and puts it back, signaling that robot needs to turn back and move towards the other end.
###Following are a series of videos describing the robot evolution while I implemented and optimized different features:

##Version #1: first try...