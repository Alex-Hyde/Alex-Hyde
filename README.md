### Hi there 👋
# Check out some of the things I've made.

- [🚀 Galacticolour](#-galacticolour---try-it-yourself)
- [♦️ Crazy beans](#%EF%B8%8F-crazy-beans---try-it-yourself)
- [🧠 Big brain time](#-big-brain-time)
- [🖥️ Real-time operating system](#%EF%B8%8F-real-time-operating-system)
- [♟️ Chess](#%EF%B8%8F-chess)
- [🚶 Walk-a-block](#-walk-a-block)
  * [🏆](#-received-the-commercialization-award-and-achieved-2nd-place-at-spark-hacks-2019-40-teams)
- [🚢 Battleship](#-battleship)
- [⛰️ Recusion graphics](#%EF%B8%8F-recusion-graphics)
- [😎 Raycasting](#-raycasting)
- [🎲 Dice game](#-dice-game)
- [🕵️ Wordsearch game](#%EF%B8%8F-wordsearch-game)
- [🏞️ Town of Aurora Parks and Trails](#%EF%B8%8F-town-of-aurora-parks-and-trails)
  * [🏆](#-won-first-place-at-the-aurora-hackathon-in-2019)

# 🚀 Galacticolour - [Try it Yourself!](https://alex-hyde.github.io/galacticolour/)

[READ MORE!](https://github.com/Alex-Hyde/galacticolour)

<p>Galacticolour is a web-based, two-dimensional space shooter which takes inspiration from classic
games such as Asteroids and Space Invaders, along with a touch of the beloved mobile game Color Switch.</p>

<p>The objective of Galacticolour is to complete a series of 14 levels, where the player traverses the galaxy from 
planet to planet fighting off waves of increasingly stronger enemies.</p>

<p>Change the appearance and functionality of your equipment including ship body types, projectiles and engines. </p>

<p>This project was developed in a team of 3 group members.</p>

[Alex Hyde](https://github.com/Alex-Hyde)<br>
[Sebastian Villate](https://github.com/Sebvillate)<br>
[Kevin Lee](https://github.com/keeinlev)<br>

| ![glowGif](https://github.com/Alex-Hyde/galacticolour/blob/master/screenshots/glow.gif/) | ![mobsManualGif](https://github.com/Alex-Hyde/galacticolour/blob/master/screenshots/mobsmanual.gif/) |
| --- | --- |
| ![openInvGif](https://github.com/Alex-Hyde/galacticolour/blob/master/screenshots/inventory.gif/) | ![moveShipLevelSelectGif](https://github.com/Alex-Hyde/galacticolour/blob/master/screenshots/levelselectmove.gif/) |
| ![levelGif](https://github.com/Alex-Hyde/galacticolour/blob/master/screenshots/level.gif/) | ![levelWarpGif](https://github.com/Alex-Hyde/galacticolour/blob/master/screenshots/warp.gif/) |

# ♦️ Crazy beans - [Try it Yourself!](https://alex-hyde.github.io/crazy-beans/)

[READ MORE!](https://github.com/Alex-Hyde/crazy-beans)

Crazy Beans is a chaotic multiplayer card game developed by

[Alex Hyde](https://github.com/Alex-Hyde)<br>
[Sebastian Villate](https://github.com/Sebvillate)<br>
[Kevin Li](https://github.com/li-kevin-987)<br>

This game was developed utilizing a ReactJS front end, paired with a Firebase backend to power online multiplayer functionality.
| ![](https://github.com/Alex-Hyde/crazy-beans/blob/master/Join.gif) | ![](https://github.com/Alex-Hyde/crazy-beans/blob/master/Gameplay.gif) |
| --- | --- |
| ![](https://github.com/Alex-Hyde/crazy-beans/blob/master/SpecialSuccess.gif) | ![](https://github.com/Alex-Hyde/crazy-beans/blob/master/SpecialFail.gif) |

# 🧠 Big brain time

[READ MORE!](https://github.com/Alex-Hyde/Big-Brain-Time)

Big Brain Time is a task management program made in Python with use of the Pygame module.
- All components are made entirely from scratch by drawing shapes, icons, and text.
- To make the program window resizable (Which is not a standard pygame feature), a <b>custom, dynamic, relative rendering module</b> was written for the project to allow all elements on screen to be rendered relative to other elements or relative to the window itself, rather than a fixed x,y position.
- All of the logic for propagating events such as mouse clicks and key presses is written from scratch.

The program includes analytics of task completion, a calendar, a file system with sorting options, different UI themes, and study sessions based on the Pomodoro Technique.

| ![menu](https://github.com/Alex-Hyde/Big-Brain-Time/blob/main/Menupreview.gif) | ![resizing](https://github.com/Alex-Hyde/Big-Brain-Time/raw/main/resize.gif) |
| --- | --- |
| ![selectingTheme](https://github.com/Alex-Hyde/Big-Brain-Time/blob/main/settings.gif) | ![colourOptions](https://github.com/Alex-Hyde/Alex-Hyde.github.io/blob/main/ProjectImages/Planner/5.png) |
| ![studySessions](https://github.com/Alex-Hyde/Big-Brain-Time/raw/main/study.gif) | ![calendar](https://github.com/Alex-Hyde/Big-Brain-Time/raw/main/calendar.gif) |

# 🖥️ Real-time operating system

This project involved designing a real-time executive (RTX) and implementing in on a `Keil MCB1700 board populated with an NXP LPC1768 microcontroller`.

The following are features and high-level implementation details of the RTX:
- A **memory management system** consisting mainly of a linked list that tracks all available memory blocks. The linked list itself (the memory block address and pointers to the next node) is built in a fixed amount of space in the kernel's memory.
- A **multi-level priority queue** to manage processes that is also built in fixed memory. This is possible since the number of processes has a hard limit. The queue is used to select processes for execution during scheduling and preemption.
- **Message-based inter-process communication** where messages are passed between processes by the kernel. Processes are blocked when trying to receive a message, until a message is available.
- A **timing service** that allows messaged to be delivered after a delay. An interrupt with a corresponding timer interrupt handler is used to deliver the message.
- **System console I/O and debugging support** which forwards characters from the keyboard to processes, and from processes to the display. This service is entirely interrupt based with no polling or busy waiting.

# ♟️ Chess
This project was an implementation of the classic game of chess. The game supports player vs. player and player vs. computer gameplay. The computer "player" can be chosen from multiple different difficulties. The most notable part of this project was the planning phase and the incorporation of multiple design patterns in the architecture diagram to create a very efficient, flexible, and easy to develop system.

Some of these design patterns included:
- **Observer Design Pattern**: Used by the different UI displays (text output & graphical display) to observe changes that occur on the game board and update the UI accordingly.
- **Decorator Design Pattern**: THe computer player class is implemented with the decorator pattern, where the basic level 1 computer player can be decorated with other difficulties. Each decorator level changes the values that are assigned to moves. Lower level decorators prioritize randomness and immediate captures. Higher level decorators look into the future and prioritize strategy. In the end, the move with the highest value is selected.
- **Resource Acquisition Is Initialization (RAII)**: The entire system incorporates this design pattern by using unique pointers for object creation, with no calls to `new` or `delete`. This significantly simplifies memory management, since all objects are destructed when they go out of scope.

# 🚶 Walk-a-block
An Android app that encourages walking to local businesses, rather than driving to or ordering from big chains, by rewarding users with coupons to get discounts on their purchases when they walk to the business.

Uses Google Maps location data to periodically calculate speed to ensure the user isn't driving.

### 🏆 Received the commercialization award and achieved 2nd place at Spark Hacks 2019 (40+ teams).
- Worked with the town of Brampton and the Brampton Entrepreneur Centre's incubator program to develop and market the idea.

| ![](https://github.com/Alex-Hyde/Alex-Hyde.github.io/raw/main/ProjectImages/Walkablock/1.1.PNG) | ![](https://github.com/Alex-Hyde/Alex-Hyde.github.io/raw/main/ProjectImages/Walkablock/1.2.PNG?raw=true) | ![](https://github.com/Alex-Hyde/Alex-Hyde.github.io/raw/main/ProjectImages/Walkablock/2.png) |
| --- | --- | --- |

# 🚢 Battleship

Implementation of the classic game Battleship using an Arduino. The game is displayed on a 32x16 LED display and includes PvP multiplayer and PvE with multiple AI difficulties. Developed in a 5 person team.

<img src="https://github.com/Alex-Hyde/Alex-Hyde.github.io/blob/main/ProjectImages/Battleship/1.png?raw=true" width="500"/>
<img src="https://github.com/Alex-Hyde/Alex-Hyde.github.io/blob/main/ProjectImages/Battleship/2.PNG?raw=true" width="500"/>
<img src="https://github.com/Alex-Hyde/Alex-Hyde.github.io/blob/main/ProjectImages/Battleship/3.PNG?raw=true" width="500"/>

# ⛰️ Recusion graphics

Program that generates and renders several fractal designs using recursion, including trees, mountains and bushes.

| <img alt="Screenshot 2023-10-14 at 12 35 45 AM" src="https://github.com/Alex-Hyde/Alex-Hyde/assets/56458804/e31a258f-0f3f-44d2-8dda-6a3df1e8fc95"> | ![Untitled2](https://github.com/Alex-Hyde/Alex-Hyde/assets/56458804/395cd3d0-045e-49e0-ac7c-09d5382f23ae) |
| --- | --- |
| ![Screen Recording 2023-10-14 at 1 04 33 AM](https://github.com/Alex-Hyde/Alex-Hyde/assets/56458804/96db97db-4c20-4cc2-8a06-4d1374b997b5) | <img alt="Screenshot 2023-10-14 at 12 46 46 AM" src="https://github.com/Alex-Hyde/Alex-Hyde/assets/56458804/217b8d8a-7f0c-4d6f-830e-14d83531c14b"> |


# 😎 Raycasting
Given any 2D tilemap, this program renders it in 3D, just like the original Doom game!

https://github.com/Alex-Hyde/Alex-Hyde/assets/56458804/ee4ea587-2e48-435b-9096-641ff1a6d5e8

https://github.com/Alex-Hyde/Alex-Hyde/assets/56458804/cb2dbd99-e283-4d26-907a-1d33d2d01aec

# 🎲 Dice game
A game where a player rolls 6 - 10 dice and has to calculate the points from the dice. If they guess right, the points are added to their score. If they guess wrong, they get nothing. The points are determined by the sum of the squared values in the longest consecutive sequence from a set of rolled die.

The UI employs 3D rendering techniques and a lot of trigonometry to simulate a die rolling and bouncing on the table before eventually settling and displaying a value.

| ![dicegame3 (1)](https://github.com/Alex-Hyde/Alex-Hyde/assets/56458804/572596be-2c73-49fe-85bf-ccb5cd46c6db) | ![dicegame2](https://github.com/Alex-Hyde/Alex-Hyde/assets/56458804/e19945fa-f01a-4b28-ba3e-79213ae6f0f5) |
| --- | --- |
# 🕵️ Wordsearch game
Just a classic game of wordsearch with smooth word highlighting.

https://github.com/Alex-Hyde/Alex-Hyde/assets/56458804/7ce7e552-cc3a-4d8f-bf0f-45e4ca8f27b9

# 🏞️ Town of Aurora Parks and Trails

An Android app that connects people to local parks, trails, and events using Google Maps API.

| ![alt text](https://github.com/Alex-Hyde/Alex-Hyde.github.io/blob/main/ProjectImages/AuroraParks/1.png?raw=true) | ![alt text](https://github.com/Alex-Hyde/Alex-Hyde.github.io/blob/main/ProjectImages/AuroraParks/2.png?raw=true)
| --- | --- |
| ![alt text](https://github.com/Alex-Hyde/Alex-Hyde.github.io/blob/main/ProjectImages/AuroraParks/4.png?raw=true) | ![alt text](https://github.com/Alex-Hyde/Alex-Hyde.github.io/blob/main/ProjectImages/AuroraParks/5.png?raw=true) |

### 🏆 Won first place at the Aurora Hackathon in 2019.
- Presented the idea to the Town of Aurora and worked with the town to determine the feasability of further developing and deploying the app.

<!--
**Alex-Hyde/Alex-Hyde** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

<Details open>   <Summary>🔭 I’m currently working on ...
<Details open>   <Summary>🌱 I’m currently learning ...
<Details open>   <Summary>👯 I’m looking to collaborate on ...
<Details open>   <Summary>🤔 I’m looking for help with ...
<Details open>   <Summary>💬 Ask me about ...
<Details open>   <Summary>📫 How to reach me: ...
<Details open>   <Summary>😄 Pronouns: ...
<Details open>   <Summary>⚡ Fun fact: ...
-->
