<h1>NTU Computer Systems Lab</h1>

<h2>Description</h2>
Computer Systems Lab was a seminar course at the National Taiwan University offered by the Department of Computer Science and Information Engineering during my student exchange in 2022. The course consisted of a weekly 1.5 hour lecture followed by a 1.5 hour tutorial, where we worked on the weekly assignment in groups of two to build a Computer System such as an FTIR touchpad, audio controller, motion controller, catapult etc. Programs and Tools used were Arduino, Unity, Fusion 360, 3D Printing and Laser cutting.
<br />


<h2>Week 1-3</h2>

- <b>Setting up Development Environments</b> 
- <b>Building an acrylic multi-touch pad based on the principles of FTIR</b>

<h3>FTIR Touchpad</h3>
Frustrated Total Internal Reflection (FTIR) touch technology relies on the principles of light reflection and refraction to detect touch input. For this, an acrylic board was bent into shape such that a platform was made where a webcam could be set up facing up as well as the actual touchpad above the webcam, where the input could be visually captured from. Red LED lights were stuck on the side of the contraption with electrical tape to internally reflect red light in the acrylic material. When the user's finger touches the board, the part of the finger glows red, which can be captured by the webcam.  

![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/d45f48d3-92c3-4e3f-8200-5ab32513caa9)
![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/43fd940c-2c72-4f7e-a873-8a582b5cf19d)
![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/bcd5187d-bdb7-4c0d-91c3-55e3ede666f3)
![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/587077be-7acb-43e0-abec-3a18503dbc1c)

Using the computer vision library of OpenCV, the video feed from the webcam is captured and transformed with a threshold set such that only the contour of the red hue on the finger can be seen. By finding the center of the contour, touchpoints can be recorded.

![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/2ca64d14-8964-409d-b642-404f5c5ee233)

<h2>Week 4</h2>

- <b>Introduction to Arduino Development Board</b> 

<h3>Physical interface for controlling audio volume and play/pause</h3>
Building this project involved a combination of hardware connections and Arduino programming. For volume control, a potentiometer was used, while for controlling play/pause, a simple button was connected to the Arduino board.

![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/eb7b0a15-3820-4ae2-b347-90bcd4858d11)


<h2>Week 5-7</h2>

- <b>Implementing a circuit using a Wifi-Capable Microcontroller that detects button press</b> 
- <b>Get the pose data from the IMU sensor on the Microcontroller</b>
- <b>Integrating the user input from the motion controller into Unity FPS game</b> 

<h3>Wireless Motion controller</h3>
The idea behind this project was to construct a controller for a  simple FPS game with a stationary player. The controller incorporates a trigger for shooting an enemy NPC and utilizes a microcontroller along with its sensor to gather data on the rate of rotation of the controller. This data is then used to determine whether the player is aiming left, right, or center.

Initially, the circuit was assembled on a breadboard. By establishing a connection with a local network, the script controlling the player in Unity could read the data from the wireless controller. This facilitated triggering the gun and adjusting the player's aim based on the rotation data received from the sensor. For the final part of the project, parts were sketched on Fusion 360, laser cut, and assembled into a case for the controller. A trigger mechanism was also made by bending a plastic part into shape and attaching it to the case.

![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/43d56ca6-23cc-450a-aa4c-99a25c2237c4)
![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/460329b2-f9f4-4db4-b3e2-6b81dd1bbb1f)
![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/abd6a78d-8a07-4141-9049-e38e5ee28776)
![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/45a55537-eff6-4ade-87eb-e3b2b7c23564)
![image](https://github.com/KIshiharaHCI/NTU-Computer-Systems-Lab/assets/122443065/007d561e-3c45-4d7f-8590-8785f122bea1)


