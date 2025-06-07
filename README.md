# 🚗 Surveillance Car using ESP32-CAM | Wi-Fi Controlled Robotic Camera Car

![Car image](https://github.com/maanasaprathap/car_module/blob/main/Images/camera%20car%20eee%20project%20image.png)
![Surveillance Car](https://github.com/maanasaprathap/car_module/blob/main/Images/eee%20project.jpg) 

> Remotely control. Stream live video. Explore and secure your surroundings. All from a compact Wi-Fi powered car.

---

## 📝 Project Overview

This repository presents a **Wi-Fi Controlled Surveillance Car** built using the **ESP32-CAM module**, designed to offer **real-time remote monitoring and mobility**. Whether you want to secure your home, monitor your pets, or explore robotics and IoT, this project is a hands-on gateway to embedded systems and computer vision.

> **Built by:**
>  Maanasa Prathap Chander · Sahana S · Akshaya A · Neeraja A

---

## 🛠️ Features

* 📷 **Live Video Streaming** from the ESP32-CAM module via a browser-based interface.
* 🕹️ **Remote Car Control** using a simple and responsive web page.
* 🌐 **Wi-Fi Enabled** – connect and operate from any device on the same network.
* 🧠 **Expandable Architecture** for adding motion detection, object tracking, or sensors.

---

## 🔧 Components Used

| Component                        | Purpose                                            |
| -------------------------------- | -------------------------------------------------- |
| **ESP32-CAM**                    | Camera + microcontroller for streaming and control |
| **L298N Motor Driver Module**    | Controls motor direction and speed                 |
| **4WD Car Kit**                  | Base chassis with 4 DC motors                      |
| **7–12V DC Battery (LiPo 3S)**   | Power supply for motors and ESP32                  |
| **Arduino Uno**                  | Used to upload code to ESP32-CAM                   |
| **Breadboard & Jumper Wires**    | Wiring and prototyping                             |
| **Glue Gun & Double-sided Tape** | Mounting components securely                       |

---

## 🧩 How It Works

1. **Initialization**: ESP32-CAM powers on and connects to Wi-Fi.
2. **Web Interface Hosting**: A local web server is launched by the ESP32.
3. **Remote Control**: Users access a web page with control buttons (Left, Right, Forward, Reverse, Speed, and Light).
4. **Motor Control**: Commands are relayed to the L298N module to move the car.
5. **Live Streaming**: The camera feed is served in real-time through the same interface.
6. **Surveillance**: The car becomes your eyes on wheels, ready to monitor and explore.

---

## 🖼️ Circuit Diagram & Hardware Assembly

> *Refer to the detailed diagrams and images in the PDF of the project added as a file in this repository.*

**Assembly Steps:**

* Solder wires to gear motors and fix them to the chassis.
* Connect motor driver to the motors and power supply.
* Interface ESP32-CAM with the motor driver (refer to wiring chart).
* Mount all modules using glue and secure components.
* Attach wheels and ensure all circuits are stable and isolated.

---
Perfect! Thanks for confirming the contents of the `/scripts/` folder. Here's your fully **revised and accurate `💻 Code Structure`** section for your `README.md`, reflecting the actual files and purpose of each directory:

---

## 💻 Code Structure

This project supports both **Arduino IDE** and **PlatformIO**, and the codebase is organized for easy setup, compilation, and execution of the ESP32-CAM-based surveillance car.

---

### 📂 Root Directory

* **`camera_car.ino`**
  The main Arduino sketch that powers the ESP32-CAM-based surveillance car.
  Responsibilities include:

  * Initializing the camera
  * Connecting to Wi-Fi
  * Launching a web server
  * Handling directional commands via HTTP requests
  * Streaming live video to the browser

* **`esp32_board.json`**
  Custom board definition for ESP32-CAM, useful when configuring custom settings or using **PlatformIO** for uploading code.

---

### 📂 `/src/`

* **`AsyncTCP.cpp` & `AsyncTCP.h`**
  These files enable asynchronous TCP communication between the ESP32 module and the client browser.

  * Ensures smooth, non-blocking video streaming
  * Improves command responsiveness over the web interface

---

### 📂 `/scripts/`

Helper scripts to set up the development environment:

* **`install-arduino-ide.sh`**
  Installs the Arduino IDE and its required dependencies on supported systems.

* **`install-arduino-core-esp32.sh`**
  Installs the ESP32 board core (by Espressif) required to compile and upload code via Arduino IDE.

* **`install-platformio.sh`**
  Sets up PlatformIO — a cross-platform embedded development environment — typically used with Visual Studio Code for building and uploading the project.

---

## 🔄 Code Summary

This code integrates camera streaming, motor control, and web interface into a cohesive system as follows :-

1. **ESP32-CAM Setup**: Initializes camera and connects to Wi-Fi.
2. **Web Server Launch**: Hosts a browser-accessible interface with direction controls.
3. **Motor Commands**: Sends GPIO signals to the **L298N motor driver** to control movement.
4. **Live Feed**: Streams video to the user over MJPEG via an asynchronous TCP server.

With this structure, the code is modular, scalable, and beginner-friendly — whether you're uploading via Arduino or using advanced tools like PlatformIO.

### How to Upload:

* Use **Arduino Uno** as a bridge to program the ESP32-CAM.
* Baud rate: 115200 | Board: AI Thinker ESP32-CAM | Upload using FTDI or Uno.

---

## 🚀 Applications

| Use Case                       | Description                                                 |
| ------------------------------ | ----------------------------------------------------------- |
| 🏡 **Home Security**           | Monitor your home while away using a moving camera.         |
| 🧪 **Educational**             | Great for learning robotics, embedded programming, and IoT. |
| 🛠️ **Remote Site Monitoring** | View areas like construction zones or warehouses.           |
| 🐾 **Pet Watching**            | Keep track of pets and their activity indoors.              |

---

## 📸 Gallery

> Check `/images/` for real pictures of our **working prototype** in action!
> You’ll find assembly images, the ESP32-CAM feed UI, and the complete mounted setup.

---

## 🧠 Learnings and Takeaways

* Integration of hardware with software logic.
* Control over HTTP using embedded web servers.
* Real-time video streaming via IP.
* Basics of DC motor control and L298N configuration.
* Handling power and voltage challenges in embedded systems.

---

## 📎 Additional Resources

* ESP32-CAM Documentation: [Espressif Docs](https://docs.espressif.com/)
* Motor Driver Guide: [L298N H-Bridge Tutorial](https://lastminuteengineers.com/l298n-dc-motor-arduino-tutorial/)
* Web Controlled Car Reference: [Random Nerd Tutorials](https://randomnerdtutorials.com/)

---

## 🤝 Contributing

Feel free to fork this repo and extend functionality! Ideas include:

* Motion Detection with OpenCV
* Firebase Cloud Integration
* Autonomous Navigation
* Android App Interface

---

## 📜 License

This project is open-source under the **MIT License**.
Feel free to use, modify, and enhance it!

