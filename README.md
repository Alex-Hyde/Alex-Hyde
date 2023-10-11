### Hi there 👋
# Check out some of the things I've made.

- [🚀 Galacticolour](#-galacticolour---try-it-yourself)
- [♦️ Crazy beans](#%EF%B8%8F-crazy-beans---try-it-yourself)
- [🧠 Big brain time](#-big-brain-time)
- [🖥️ Real-time operating system](#%EF%B8%8F-real-time-operating-system)
- [♟️ Chess](#%EF%B8%8F-chess)
- [🚶 Walk-a-block](#-walk-a-block)
- [🚢 Battleship](#-battleship)
- [⛰️ Recusion graphics](#%EF%B8%8F-recusion-graphics)
- [😎 Raycasting](#-raycasting)
- [🎲 Dice game](#-dice-game)
- [🕵️ Wordsearch game](#%EF%B8%8F-wordsearch-game)
- [🏞️ Town of Aurora Parks and Trails](#%EF%B8%8F-town-of-aurora-parks-and-trails)

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
[Kevin Lee](https://github.com/li-kevin-987)<br>

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
# 🚶 Walk-a-block
# 🚢 Battleship
# ⛰️ Recusion graphics
# 😎 Raycasting
# 🎲 Dice game
# 🕵️ Wordsearch game
# 🏞️ Town of Aurora Parks and Trails

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
