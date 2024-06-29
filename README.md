# car_module
Surveillance Car using ESP32 Camera Module

he Surveillance Car using the ESP32 Cam module is a project that 
involves building a remote-controlled car equipped with a camera 
for surveillance purposes. The ESP32 Cam module, based on the 
ESP32 microcontroller, provides both the processing power and the 
capability to capture and stream video. The project allows users 
to remotely control the car over Wi-Fi, view live video footage, 
and potentially implement additional features for surveillance and 
exploration.

A surveillance car using ESP32-CAM is a system that utilizes the 
ESP32-CAM board and a car chassis to create a mobile surveillance 
device. The ESP32-CAM is a low-cost development board that 
integrates a small camera module and Wi-Fi connectivity. The car 
chassis allows the device to move around and capture video in 
different locations. The system can be controlled through a web 
interface hosted on the ESP32-CAM board. The web interface allows 
the user to control the car's movement, view live video streams, 
and take snapshots of the video feed. Additionally, the system can 
be programmed to detect motion using computer vision algorithms, 
such as object detection and tracking, and send alerts to the 
user. The surveillance car using ESP32-CAM has potential 
applications in home security, monitoring of remote locations, and 
industrial surveillance. With its low cost and easy-to-use 
interface, it provides a convenient solution for anyone who needs 
to monitor their surroundings remotely.

Initialization: 

The ESP32 Cam module is powered up, and the initialization routine 
begins. Wi-Fi Connection: The ESP32 Cam connects to a 
preconfigured Wi-Fi network, making it accessible on the local 
network. Web Server Hosting: The ESP32 Cam sets up a simple web 
server that hosts a web page. User Interaction: Users access the 
web page served by the ESP32 Cam using a web browser. The web page 
includes controls for moving the car. Motor Control: Based on user 
inputs from the web interface, the ESP32 Cam sends commands to the 
motor driver to control the movement of the car. 
Streaming: The ESP32 Cam captures video footage using its 
integrated camera. The live video stream is made available through 
the web server. Remote Surveillance: Users can remotely monitor 
the video feed in real-time, effectively using the car for 
surveillance purposes.
Web controlled surveillance cars can be built using the ESP32-CAM 
module. Apart from the ESP32-Camera module, we will need 4 DC 
motors with its Robo car chassis and L293D motor driver module to 
build this Robocar. ESP32 is one of the popular boards to build 
IoT-based projects.

Here HTTP communication protocol is used to receive video 
streaming from the camera over the web browser using an IP 
address. The web page will also have buttons to move the car in 
Left, Right, Forward, and reverse directions and can vary the 
speed with light control as well.
 
Uses and Applications:

This project is a practical application of IoT (Internet of 
Things) and robotics, providing an opportunity to learn about 
microcontroller programming, motor control, and wireless 
communication. It demonstrates the integration of hardware 
components and software logic to create a functional and remotely 
controlled surveillance car. A Surveillance Car using the ESP32 
Cam module has various practical applications due to its ability 
to capture and transmit video over Wi-Fi. Here are some potential 
uses: Home Security: Deploy the surveillance car to monitor your 
home when you're away. You can remotely access the live video feed 
to check for any unusual activities or intruders. Remote 
Monitoring: Use the surveillance car to monitor remote locations. 
This could be useful for checking on vacation homes, construction 
sites, or other areas where real-time visual inspection is 
necessary. Educational Tool: The project can serve as an 
educational tool for learning about robotics, IoT, and 
programming. Students and hobbyists can explore concepts such as 
motor control, wireless communication, and camera integration. Pet 
Monitoring: Keep an eye on your pets while you're not at home.
