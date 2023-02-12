# Sergei Litovchenko

serglit10229@gmail.com  
(650) 471-4836  
San Jose, CA 95116  
[linkedin.com/in/SergeiL](https://linkedin.com/in/SergeiL)

### Summary:
Results-driven software developer with a strong background in game development using Unreal Engine 4/5, Unity, and custom OpenGL game engines. Proven experience in creating VR, mobile, and desktop games with intricate mechanics and optimized performance. Skilled in delivering high-quality, efficient, and reliable code. Committed to staying current with industry trends and advancements in technology.

### Skills:
Programming Languages: C++ (4 years), C# (4 years), C (2 years), Java (2 years), MATLAB
API and Libraries: Unreal Engine 4/5, Unity 2021.2, Oculus (OpenXR), SteamVR, GLFW 3.3, OpenGL 4.6, Direct3D 11/12, Win32 API



## Full-body Tracking UE4 SDK + Demo Games
![KR1](KR1.gif)  
Tasked to create a communication protocol between Unreal Engine 4 game/application and Kinetic Reality Proprietary full-body motion tracking hardware on local WIFI network. 
Developed a UDP packet writing/reading SDK in native C++ for extemely low latency comunication with KR sensors on LAN. 
Helped with development and debugging of hardware-side UDP communication code.
Developed a custom sockets plugin using UE4 FSocket API to employ cross-platform abilities. 
Optimized and maintained the plugin for use in Android-based builds to support Meta Quest 1/2 wireless VR headsets.
Implemented simple Blueprint and C++ components for fast and scalable development of games/apps that want to use full-body tracking on Skeletal Mesh and Static Mesh systems with physics adjusted to simulate a character standing on their feet and inverse-kinematics calculation methods.
![KR2](KR2.gif)

Developed two standalone VR games using UE4 and the KR SDK for internal testing and tech demonstations.
KR Tennis features realistic tennis ball and racquet physics, simulated in real-time on one or multiple Quest VR Headsets. Demonstrates the ability of KR hardware to support low-latency applications and tollerance to fast-accelerating movements. Allows for useful biomechanics analysis to be completed on the recorded(or in realtime) player movements. Demonstrates KR hardware's support for muitple simuoultaniuons users in the same sensor-area network, allowing multiplayer tennis matches.
KR Combat features an arcade PvE and PvP martial arts fighting simulator. Fun demo game made for intended for shows and conferences like GDC 2023. The main obstacle with the initial idea was force feedback and visualization of damage on players. Since this is a game in "virtual" reality, players dont actually hit each other physically as they can be playing together on different continents. But to make the experiecen feel somewhat realistic and fun, I designed and implemented a simple vfx feedback emulation that separated the physical model of the character from the skeletal mesh binded to the KR sensors.  
![KR3](KR3.png)  
