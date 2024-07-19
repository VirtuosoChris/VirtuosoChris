# Chris Pugh's Homepage

<div display="flex">
  <img src="https://img.shields.io/badge/C++-gray?style=for-the-badge&logo=c%2B%2B&logoColor=%2361DAFB" alt="C++"/>
  <img src="https://img.shields.io/badge/OpenGL-gray.svg?style=for-the-badge&logo=opengl&logoColor=%#5586A4FB" alt="OpenGL"/>
  <img src="https://img.shields.io/badge/PhysX-gray.svg?style=for-the-badge&logo=nvidia&logoColor=%76B900FB" alt="PhysX"/>
</div>


<!--
**VirtuosoChris/VirtuosoChris** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

I am an independent game programmer, who specializes in 3D graphics, modern C++, and engine / API design.

I have worked on a lot of projects using a myriad of languages and engines, targeting everything from PC to mobile to VR.

A lot of my work isn't public (or public yet!), and my repositories are littered with various forks and experiments, so I figured this page could focus attention on the highlights.

## Current Projects

### Killing Baby Hitler

I am currently making "Killing Baby Hitler", a retro FPS "boomer shooter" inspired by classics like Wolfenstein.  The game is built on a custom engine ("Virtuoso Engine", discussed below).
A gameplay trailer can be seen here: 

[<img src="./preview.jpg" width="512"/>](https://www.youtube.com/watch?v=QDfS3aJYwFk)

The game and engine code will eventually be publicly released under an MIT License, but not yet.  If you are considering me for employment and want an up to date code sample or playable build feel free to contact me and ask.

### Virtuoso Engine
#### Description and Philosophy
Virtuoso Engine is my personal game and app development framework that I've been working on for about a decade or so in various iterations, and have shipped multiple apps on.  The latest version is being used in the development of "Killing Baby Hitler."

The philosophy of the engine is to be a lightweight framework style engine, sort of like [RayLib](https://www.raylib.com/), but more focusing on C++20, 3D, and physics rather than C99/2D.  I wanted to make this because it's the language / paradigm under which I'm most productive as a very experienced C++ programmer with lots of graphics programming and graphics driver experience.

I also am a really strong booster of the ["STB"](https://github.com/nothings/stb) style of library - of making components or functionality that can be forked off without dependencies into a single header, permissive license "library."

#### Public Components
Several components of the engine can be seen publicly on my GitHub:

[YarnMachine](https://github.com/VirtuosoChris/YarnMachine) - A standalone C++ virtual machine for [YarnSpinner](https://www.yarnspinner.dev/), a narrative scripting language I use in KBH

[Quake Style Console](https://github.com/VirtuosoChris/VirtuosoConsole) - Debug console and IMGUI widget

[GLSugar](https://github.com/VirtuosoChris/GLSugar) - Graphics framework for modern / AZDO style OpenGL development with nicer syntax.  This has code for basic texture and shader handling, as well as struct annotation to easily make VAO's and [UBOs](https://github.com/VirtuosoChris/GL_UBO/) with correct memory alignments.  Built on GLHPP (discussed below), a library written by a colleague to which I am a contributor.

[uJNI](https://github.com/VirtuosoChris/uJNI) - Not used in KBH, but was developed for the 2016/2017 iteration of the engine to ship a Fireworks Show VR app on the GearVR platform.

#### 3rd Party Components
A lot of the work on the engine is curating which third party libraries to use vs which things to write myself.  The engine puts together and builds on lots of third party open source technologies, including but not limited to:

[glhpp](https://github.com/Steve132/glhpp/) - Object oriented, DSA OpenGL header by a colleague, to which I am a contributor.

[PhysX](https://github.com/NVIDIA-Omniverse/PhysX/) - General purpose physics, collision, math, and simulation library

[Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page) - For matrix and linear algebra

[Dear ImGUI](https://github.com/ocornut/imgui) - For user interfaces and tools prototyping.  Also several other 3rd party repo's for adding gizmos, markdown, and file dialogs to IMGUI.

[MiniAudio](https://miniaud.io/) - For 3D sound playback and music streaming

[Yarn Spinner](https://github.com/YarnSpinnerTool/YarnSpinner) - For dialogue and narrative scripting.  I use their VSCode plugin and their compiler, but built my own C++ runtime discussed above.

[Debug Draw](https://github.com/glampert/debug-draw) - For wireframe primitive visualization

[GLFW](https://github.com/glfw/glfw) and [GLFWPP](https://github.com/Steve132/glfwpp) - for cross platform windowing system and input

[STB](https://github.com/nothings/stb) - Image loading and other miscellanea

[nlohmann's JSON](https://github.com/nlohmann/json) - For data serialization

[MiniZ](https://github.com/richgel999/miniz/) - for compression and bundling of map data


