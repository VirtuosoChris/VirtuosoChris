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
# Who Am I?
I am an independent game programmer, who specializes in 3D graphics, modern C++, and engine / API design.

I have worked on a lot of projects using a myriad of languages and engines, targeting everything from PC to mobile to VR.

A lot of my work isn't public (or public yet!), and my repositories are littered with various forks and experiments, so I figured this page could focus attention on the highlights.

### Professional highlights

A couple career highlights before I get into my current projects :

I was an OpenGL workstation driver engineer for almost a decade.  I redesigned the legacy driver's multithreading code, and was part of the team that developed an entirely new OpenGL driver, released in 2022, which had up to 72% performance gains in key applications.  I learned a lot and worked with a great team of people.

[<img src="https://github.com/user-attachments/assets/d4b6cc06-1359-4f34-9957-bc9c12525e6c" width="256"/>](https://www.tomshardware.com/news/amd-rearchitects-opengl-driver-for-a-72-performance-uplift)

Before that I worked in the Computer Graphics lab at UCF implementing [virtual texturing](https://silverspaceship.com/src/svt/) and [Blockmaps](https://diglib.eg.org/server/api/core/bitstreams/b64ac199-b739-4e5d-91f5-202caf811e89/content) for streaming visualization, work which concluded in 2013.

But I think my best, most exciting work is my current game and engine, which you'll read about below :)

More detailed career history, projects, and my up to date resume can be found on my [LinkedIn](https://www.linkedin.com/in/chris-pugh-70937975/)

Or here : [Christopher Pugh Resume July 2024.pdf](https://github.com/user-attachments/files/16486569/Christopher.Pugh.Resume.July.2024.pdf)

## Current Projects

### Killing Baby Hitler

I am currently making Killing Baby Hitler, a retro FPS "boomer shooter" inspired by classics like Wolfenstein.  The game is built on a custom engine ("Virtuoso Engine", discussed below).
A gameplay trailer can be seen here: 

https://github.com/user-attachments/assets/77d3f63f-70c5-4d7e-8026-a8b3d5da427a

Or on [YouTube](https://www.youtube.com/watch?v=QDfS3aJYwFk)

The game and engine code will eventually be publicly released under an MIT License, but not yet.  If you are considering me for employment and want an up to date code sample or playable build feel free to contact me and ask.

### Virtuoso Engine
<img src="https://github.com/user-attachments/assets/f954bf75-07e8-4741-9008-fc52df5a76c0" width="320"/>


#### Description and Philosophy
Virtuoso Engine is my personal game and app development framework that I've been working on for about a decade or so in various iterations, and have shipped multiple apps on.  The latest version is being used in the development of "Killing Baby Hitler."

The philosophy of the engine is to be a lightweight framework style engine, sort of like [RayLib](https://www.raylib.com/), but more focusing on C++20, 3D, and physics rather than C99/2D.  I wanted to make this because it's the language / paradigm under which I'm most productive as a very experienced C++ programmer with lots of graphics programming and graphics driver experience.

I also am a really strong booster of the ["STB"](https://github.com/nothings/stb) style of library - of making components or functionality that can be forked off without dependencies into a single header, permissive license "library."

#### Public Components
Several components of the engine can be seen publicly on my GitHub:

[YarnMachine](https://github.com/VirtuosoChris/YarnMachine) - A standalone C++ virtual machine for [YarnSpinner](https://www.yarnspinner.dev/), a narrative scripting language I use in KBH for dialogue and game scripting.

[Quake Style Console](https://github.com/VirtuosoChris/VirtuosoConsole) - Debug console and IMGUI widget.  The first version of this was written 11 years ago as an experiment but I've been maintaining and using this ever since.

[GLSugar](https://github.com/VirtuosoChris/GLSugar) - Graphics framework for modern / AZDO style OpenGL development with nicer syntax.  This has code for basic texture and shader handling, as well as struct annotation to easily make VAO's and [UBOs](https://github.com/VirtuosoChris/GL_UBO/) with correct memory alignments.  Built on GLHPP (discussed below), a library written by a colleague to which I am a contributor.

[uJNI](https://github.com/VirtuosoChris/uJNI) - Helper functions and classes to wrangle JNI / NDK things.  Not used in KBH, but was rapidly developed for the 2016/2017 iteration of the engine to ship a Fireworks Show VR app on the GearVR platform (Android).

[Spherical Harmonics](https://github.com/VirtuosoChris/SphericalHarmonics) - Utility code for environment map filtering.  Used for glossy HDR environment rendering in unreleased prototypes, and diffuse probe convolution in Fireworks Show VR.

[Noise](https://github.com/VirtuosoChris/Noise) - Perlin Noise Generation : Used in unreleased prototypes.

## Past Projects

A sampling of my motable past projects includes:

### Making Games By Year
A YouTube show talking about the history of a game for every year since the beginning of gaming, then making that game.  It got as far as 1969 (Lunar Lander) and 1971 (Star Trek) before I had to put the project aside due to the sheer amount of work between development, research, and video editing.  I do have ideas on how I want to revive this though :)

![Javascript Star Trek Game 2019](https://github.com/user-attachments/assets/9cfc1af6-9675-46b7-bdbc-dddefb20ae20)

[YouTube Episode Playlist](https://www.youtube.com/playlist?list=PLqb-u860i_E9UJC_YRI9igpuhXCXv3tqk)

[Star Trek Game JavaScript Source](https://github.com/MakingGamesByYear/TrekGame) from Episode 1

You can play the game [here](https://makinggamesbyyear.itch.io/star-trek-1971).

### Fireworks Show VR
2017 app released for free on the GearVR App Store via download code.  It was also available for Cardboard VR.  Built on Virtuoso Engine.  Source repo [TBD](https://github.com/VirtuosoChris/Fireworks-Show-VR/).  Preview gif below:

![fwgif](https://github.com/user-attachments/assets/8d931ee5-a879-4dd9-9510-eb06d53e7db1)

### Crayon Rendering Algorithm
2013, a heuristic approach made for low performance / mobile rendering at the time.  Source code and (unpublished) algorithm paper in repository [here](https://github.com/VirtuosoChris/CrayonRenderer).

![screenshot](https://github.com/user-attachments/assets/97751aa6-135b-49a4-9fa4-5c3c567d05ba)

### Music
I played trumpet in jazz, concert, and marching band in high school and middle school.  That's 7 years total, which is just shy of the time at my longest adult job.  This turned into being a self taught guitarist as an adult, and in the past year or two I started getting formal lessons.  It's been an enriching part of my life, but also turned into a skill I am using to make the soundtrack for KBH!

<img src="https://github.com/user-attachments/assets/12c11cf3-dabb-4408-9afc-5cc7e8936729" width="256"/>

## 3rd Party Libraries
A lot of the work on the engine is curating which third party libraries to use vs which things to write myself.  The engine puts together and builds on top of lots of third party open source libraries, including but not limited to:

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

## Older Projects
### Personal Projects
[1D Pong (2009)](https://github.com/VirtuosoChris/1DPong)

[Asteroids (2007) : My second game](https://github.com/VirtuosoChris/Asteroids)

[BONG (Breakout-Pong, 2006) : My first game](https://github.com/VirtuosoChris/BONG)


### Class Projects
[Paint Demo (2010)](https://github.com/VirtuosoChris/PaintDemo2010)

[Quake The Can (2009)](https://github.com/VirtuosoChris/quakethecan)

[Dr. Karnaugh's Lab (2008)](https://github.com/VirtuosoChris/drkarnaugh)


## Miscellaneous Screenshots Gallery
Various screenshots of various games / rendering effects / projects I've worked on (in no order).  These go back to when I first started to code in 2006 or so, up to around 2020.

![Post Processing FX DoG   Icosphere](https://github.com/user-attachments/assets/b3c71745-216d-455d-ae53-4c906db669dc)
![Mandelbrot OpenCL 2012](https://github.com/user-attachments/assets/ee74a7be-2475-4694-a5ba-23ee8cf39f33)
![HDR Mobile VR 2016](https://github.com/user-attachments/assets/eb760afc-2706-41dc-8555-2f7b8872b3f5)
![GLES Mobile Water Shader 2016](https://github.com/user-attachments/assets/4b38adad-a7de-492b-943d-b478295f9659)
![Bloom HDR Emissive 2012](https://github.com/user-attachments/assets/a61549a3-50e8-4731-a993-172cfa38cbd7)
![Spherical Harmonic Lighting Probe Convolutions](https://github.com/user-attachments/assets/5a50ba4c-e26d-4fc6-b661-91d796aae4ed)
![ShadowMaps Bloom LOD HDR](https://github.com/user-attachments/assets/6f88d5d3-3fcb-4c18-8575-c63203f1dd1e)
![Shadowmaps Bloom HDR](https://github.com/user-attachments/assets/e1755a54-dc48-44b5-b906-08e45a69b41a)
![38104_408871258299_5415115_n](https://github.com/user-attachments/assets/6bea0192-846c-4aac-8c00-623dce4b6ca0)
![1235364_10151693798478300_667182919_n](https://github.com/user-attachments/assets/94cffcd7-ad5c-4720-af3a-a973d60cbe6c)
![562340_10151693775423300_1418642382_n](https://github.com/user-attachments/assets/24ff2939-7294-4982-9a8b-a9234e7e66ef)
![462912_10150724418683300_1027386139_o](https://github.com/user-attachments/assets/e548e416-3e73-4223-bdde-76b629cc21e1)
![191696_10150121343723300_1099850_o](https://github.com/user-attachments/assets/b59efd1f-c5bc-4fc4-bc3c-b19be09d090d)
![191644_10150121343578300_4021780_o](https://github.com/user-attachments/assets/865b6b71-8cd6-4e16-b8c4-e024bc08c58b)
![34374_402948048299_5819395_n](https://github.com/user-attachments/assets/8ef66e0a-e341-4555-a054-1655d43fc3f3)
![27035_383537978299_5452579_n](https://github.com/user-attachments/assets/139d1f14-c9bd-4628-b844-bc4a193badaf)
![64147_10151693770768300_1219412655_n](https://github.com/user-attachments/assets/822b611b-e18f-4ce8-a503-1f9a955ae34e)
![1235908_10151693724063300_1248181310_n](https://github.com/user-attachments/assets/66b1c42e-696b-4d7d-9269-fbf935ee12d4)
![18157861_10154874392848300_6480177987938036393_n](https://github.com/user-attachments/assets/8802d612-7584-4d98-ae6b-f47f410a509c)

