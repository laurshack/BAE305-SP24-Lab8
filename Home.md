# Lab 8 Report - App Development

Group members:
* Anastasia Myers
* Lauren Shackleford
* Rebecca Stacy

Date: 3/7/2024

## Summary
The purpose of this lab was to introduce us to the use of App Inventor. In this lab, we worked with our robot that we had previously built and used the App Inventor software to control it. The goal of this lab was to be able to operate our robot through the app. This was done by downloading our code from lab 6 onto our microcontroller (redboard) and using app inventor to connect loaded commands to buttons on our phone. The first part of the lab involved finishing the assembly of our robot, this had already been completed. The second part of the lab involved developing the app. App inventor utilizes block coding where each line is created as a block, this makes the process fairly simple. Part three of the lab was meant to involve the use of Bluetooth to control the robot, however, due to technical difficulties was dropped. The most challenging aspect of this lab was learning a new coding software.


## Equipment

- Computer to run Arduino IDE
- Access to App Inventor
- Android phone
- Adaptor
- Sparkfun Inventor's Kit
  - RedBoard
  - Ultrasonic sensor HC-SR04
  - Dual TB6612FNG, H-Bridge Motor Driver
  - Two gear motors
  - Wheel for each motor

## Testing, Design, and Methods

### Part 1 - Assemble and test robot

1. Attach the 2 wheels to the motors used in Lab 6.
2. Verify that the robot moves forward, backward, right, and left.
3. Attach the battery pack to the bottom of the robot. 

### Part 2 - Develop the app

1. Create an account or log in to the App Inventor 2 Web-based tool.
2. Create a new project.
3. Insert a button to initialize the serial communication (shown at Open_Serial in step 5). 
4. From the Connectivity section add a Serial component (shown at Serial1 in step 5). 
5. In the Blocks environment add the blocks shown below:

![image](https://github.com/Perc312/BAE305-SP24-Lab8/assets/156240511/21f9b9f8-94bd-4c2c-b6e4-191e4d5ae541)

6. Use the “call serialObject.WriteSerial” block and a “text” block to send the commands to the RedBoard. The text commands should be the same commands used in the Arduino IDE Serial Monitor. 
7. Use the QR code to install the app on your phone. Connect your phone to the RedBoard using a USB-C to USB-A cable. 




## Results
### Part 2 - Developing the app
![image](https://github.com/Perc312/BAE305-SP24-Lab8/assets/156240511/15fb0448-7c61-4061-9785-303ec838a527)

### Part 3 - Wireless remote

![image](https://github.com/Perc312/BAE305-SP24-Lab8/assets/156240511/b46a36ee-f392-4ee2-9d0a-778505a4206c)

## Discussion

### Part 1 - Assemble and Test Your Robot
In Lab 6 we found out what was the minimum speed that will move the motors. What is the minimum speed that will move the complete car?
> In lab when we investigated the minimum speed to operate, we determined that the number was "30". However, after assembling the complete car we determined that the minimum number to induce motion was "20". In lab 6 we attributed the value to being non-zero because of factors such as friction and electricity, but as we added wheels and movement the minimum speed to operate decreased, so we are confused as to what this could be attributed to.

## Conclusion

This lab introduced us to App Inventor software. Utilizing an app can make the user interface more simple to use especially for people unfamiliar with code. One way this is done is by linking commands to buttons which makes it so users can simply press a button to send a command. However, the app development software we used still requires that code be uploaded using Arduino IDE to the microcontroller. Another component we were meant to work with was Bluetooth, which allows commands from the app to be sent to the microcontroller through Bluetooth. This is important because this allows control of the machine without a physical connection.

The main takeaway of this lab is the ability to utilize our microcontroller, Arduino IDE code, and app inventor software. Using app inventor helped us become familiar with the use of their block coding format, as well as how to connect commands for our original codes to buttons. Working with app inventor gave us an important tool for our final project, this software could be used to create buttons to control the movement or drop of our claw. This lab was also a good jumping-off point for learning more about App inventor, for example, the use of the slider function to create variable motor speed on the claw. 

