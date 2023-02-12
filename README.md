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


## Simple A* Pathfinding implementation
As a part of KR Combat demo, I was tasked to create a PvE game mode with a simple AI that would run around the level and/or chase the player and apply damage via pre-determined animated moves. I experimented with a lighter(for Quests) navigation system than what UE4/5's built in AI system. 

![Pathfinding1](Pathfinding1.gif)

I created a native implemention of A* grid-based pathfinding algorithm. The demo demonstrates dynamically-generated obstacles that can be created in editor or at runtime. The navigation manager finds the best path from point A(yellow) to point B(red) and outputs the path with locations of grid squares. The Green sphere than retraces the path for visualization. This algorithm successfully navigated the AI in KR Combat game and ran on Quest 2 to complement a fun VR demo.




## Custom Voxel Destruction System Experiment
![Destruction(Single)](Destruction(Single).gif)

The goal was to create a voxel-based destruction system that would run faster than UE4/5's built-in Chaos destruction, can be changed or created at runtime and be scalable for 60fps games, not just rendered movie pipelines. The demo creates a multi-story building, made out of instanced triangular chunks(33,000+). If the building recieves damage abve certain threshold, all chunks within a specified radius from the impact location will be destroye, creating a hole. The system is fully scalable and can support multiple buildings on the same level with up to 2 million chunks in each. The buildings can also be made out of irregular chunks like glass, have different materials, and have a completely abstract shape. In 90% of all possible cases, the entire algorithm runs under 5ms(asynchronyously) even with 30 million chunks in the level.

![Destruction(Total)](Destruction(Total).gif)

An island-searching algorithm will then determine if any part of the building is no longer connected to the sny neightbor components and, therefore, needs to be destroyed too. This is needed to avoid having large parts of a building just hovering in the air. I'm currently using this system, updated with cool VFX in another personal project on movable vehicles.


## Schuco Animation Kit
Tasked to initialize, develop, and deliver a complete software package for 3D model animation and for visualization and presentation. Allows people without prior experience in animation to create simple assembly/disassembly animated videos of their 3D models. Used by engineers and managers to visualize products and simplifiy the manufacturing and training processes. 

<img width="500" src="SAK1.png">      <img width="500" src="SAK2.png">
<img src="SAK3.png">


We utilized Unreal Engine’s real-time rendering backend and proprietary engineering solutions to create real-time animation rendering. Led development of UI/UX, frontend and backend systems. Shipped a complete desktop tool for use within and outside of Schuco International Engineering departments.


