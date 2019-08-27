GLFW/GLEW/GLM/Freeglut/AntTweakBar and NanoGUI configuration

This is a windows version of GLFW/GLEW/GLM/FreeGLUT/AntTweakBar and nanogui binary file collection.

This version is ONLY used for Visual Studio 2019 Release(Debug)/x64 mode (Probabily it is also compatible for VS2015 and VS2017).

For other versions of binary file, you can compile it on your own using cmake-gui windows version

# Usage

<b> Do This In Order </b>

1: Add this folder into your system variables with:

Variable name: OPENGL

Variable value: This repo that you just downloaded
```
e.g.  
    Variable name: OPENGL
    Variable value: D:\Program Files\opengl
```

2: Add dll folder to your system's "Path":
```
e.g. 
    Variable name: Path
    Variable value: D:\Program Files\opengl\dll
```

2: Create your own empty project in Visual Studio 2019

3: Add each OPENGL.prop + NANOGUI.prop files into Visual Studio Property Manager（Release/Debug x64）:
(If you are using freeglut or antweakbar you can add it seperately, but do not put them all together with GLFW. It may cause some error when running the code)

3.a:  View->Other Windows->Property Manager

<img src="https://i.imgur.com/q4uePzR.png" />

3.b: Add Existing Property Sheet

<img src="https://i.imgur.com/UULN4Gd.png"/>

Make sure the project name itself is selected before adding the existing property sheet. Select OPENGL.props and NANOGUI.props here(Please add OPENGL.props first) and they should appear in the debug and release folder once added

4: Set build configurations to run on x64

4.a: Project -> Properties -> Platform (at top)

​		Value: Active(x64)

4.b: Project -> Properties -> Linker -> Advanced -> Target Machine

​		Value: MachineX64

4.c: Build -> Configuration

​		Configuration: Release

​		Platform: x64

5: Run code test:

GLFW/GLEW/GLM Test:

Add opengl_example/helloworld.cpp provided by LearnOpenGL into your project

NanoGui Test:

Add nanogui_example/example3.cpp provided by NanoGUI into your project

Done

# Reference Links

Xcode verison of NanoGUI configuration: [http://jody-lu-blog.logdown.com/posts/1533525](http://jody-lu-blog.logdown.com/posts/1533525).

Thanks for Jody Lu's help with Mac's configuration on Nanogui.

Thanks for Manevle16's help with some update for vs2019.

GLEW: [https://github.com/nigels-com/glew](https://github.com/nigels-com/glew)

GLFW: [https://github.com/glfw/glfw](https://github.com/glfw/glfw)

GLM: [https://github.com/g-truc/glm](https://github.com/g-truc/glm)

FreeGLUT: [http://freeglut.sourceforge.net](http://freeglut.sourceforge.net)

AntTweakBar: [http://anttweakbar.sourceforge.net/doc/](http://anttweakbar.sourceforge.net/doc)

NanoGui: [https://github.com/wjakob/nanogui](https://github.com/wjakob/nanogui)

Learn OpenGL: [https://github.com/JoeyDeVries/LearnOpenGL](https://github.com/JoeyDeVries/LearnOpenGL)

STB: [https://github.com/nothings/stb](https://github.com/nothings/stb)