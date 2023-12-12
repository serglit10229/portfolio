# Sergei Litovchenko

serglit10229@gmail.com  
(650) 471-4836  
Irvine, CA 92617  
[linkedin.com/in/SergeiL](https://linkedin.com/in/SergeiL)

### Summary:
Software developer specializing in game design and development. Expert in leveraging Unreal Engine 4/5, Unity, and custom OpenGL engines to achieve fun and stable gameplay experience with intricate mechanics. Experience as a Gameplay Engineer at Microsoft on Project AirSim, developing precise modeling of air and ground vehicles with real-world dynamics.

### Skills:
Programming Languages: C++ (5 years), C# (5 years), C (5 years), Java (2 years), MATLAB
APIs and Libraries: Unreal Engine 4/5, Unity, Oculus (OpenXR), SteamVR, Blender



## Microsoft Project AirSim
![Airsim](Airsim2.png)
* Developing a the new simulation platform. Ensuring the precise modeling of air and ground vehicles behaviors, guaranteeing an accurate simulation with real-world dynamics.
* Creating realistic virtual environments for testing and experimentation. Focusing on optimizing to ensure smooth and realistic interaction, aligning with accurate GIS data.
* Making custom tools for the simulation platform. Streamlining various aspects of simulation setup, data collection, and analysis, empowering the team to efficiently iterate on AI algorithms and autonomous systems.

[![Airsim](https://res.cloudinary.com/marcomontalbano/image/upload/v1702406595/video_to_markdown/images/youtube---WfTr1-OBGQ-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://www.youtube.com/watch?v=-WfTr1-OBGQ&ab_channel=ShitalShah "Airsim")


## Schuco Animation Kit
* Intended for use by people without prior experience in animation
* Designed for engineers and managers to visualize products and simplify manufacturing and training processes.
<img width="500" src="SAK1.png">      <img width="500" src="SAK2.png">

<img src="SAK3.png">

* Initialized, developed, and delivered a complete software package for 3D mesh(glTF, FBX, STEP) animation and visualization - Schuco Animation Kit
* Led frontend and backend development, Utilizing Unreal Engine’s real-time rendering backend. Supported UI/UX development
* Shipped a complete desktop tool for use within and outside of Schuco International Engineering departments


## Full-body Tracking UE4 SDK + Demo Games

![KR1](KR1.gif)

* Developed and maintained native C++ client SDK for wireless communication with custom KR motion-tracking hardware. Created a wrapper for UE4 Blueprint/C++ API with cross-platform capabilities
* Created a custom sockets plugin using UE4 `FSocket` API with cross-platform capabilities
* Optimized and maintained the plugin for use in Android-based builds for Meta Quest 1/2 wireless VR headsets

![KR2](KR2.gif)

* Delivered 2 full-body motion-tracking multiplayer games, made with UE5(C++), Oculus(OpenXR), SteamVR API, and KR development toolkit
* Worked on multiplayer netcode of first-ever MMORPG in VR. Focused on smooth gameplay and low latency to improve VR experience to reduce risk of motion sickness


## Custom Voxel Destruction System Experiment
Created a voxel-based destruction system designed for 60fps games, that can be changed or created at runtime, and is scalable. The system is designed to run faster than UE4/5's built-in Chaos destruction.

![Destruction(Single)](Destruction(Single).gif)

* Demonstrates a multi-story building made out of instanced triangular chunks, with over 33,000 chunks
* When the building receives damage above a certain threshold, all chunks within a specified radius from the impact location are destroyed, creating a hole
* The system is scalable, supporting multiple buildings on the same level with up to 2 million chunks each
* The system can be used for irregular chunks like glass, with different materials and abstract shapes
* In 90% of cases, the entire algorithm runs asynchronously in under 5ms, even with 30 million chunks in the level.

![Destruction(Total)](Destruction(Total).gif)

* Implemented an island-searching algorithm to determine if any part of a building is no longer connected to the neighbor components and needs to be destroyed
* Helps prevent large parts of a building from hovering in the air
* Updated with cool VFX and is being used in another personal project on movable vehicles.



## Simple A* Pathfinding implementation
As a part of KR Combat demo, I was tasked to create a PvE game mode with a simple AI that would run around the level and/or chase the player and apply damage via pre-determined animated moves. I experimented with a lighter(for Quests) navigation system than what UE4/5's built in AI system. 

![Pathfinding1](Pathfinding1.gif)

* Created a native implementation of the A* grid-based pathfinding algorithm
* Demonstrates dynamically generated obstacles that can be created in the editor or at runtime
* Navigation manager finds the best path from point A to point B and outputs the path with grid square locations. Then, retraces the path for visualization
* Successfully implemented the algorithm for AI navigation in KR Combat game and ran on Quest 2 for a fun VR demo.