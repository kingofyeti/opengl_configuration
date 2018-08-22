# GLFW/GLEW/GLM/Freeglut/AntTweakBar and NanoGUI configuration

This is a windows version of GLFW/GLEW/GLM/FreeGLUT/AntTweakBar and nanogui binary file collection.

This version is used for Visual Studio 2015 Release(Debug)/x64 mode.

For other versions of binary file, you can compile it on your own using cmake-gui windows version

# Usage

1: Add this folder into your system variables with:

Variable name: OPENGL

Variable value: YOUR_CURRENT_FOLDER
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

2: Create your own empty project in Visual Studio 2015

3: Add each OPENGL.prop + NANOGUI.prop files into Visual Studio Property Manager:
(If you are using freeglut or antweakbar you can add it seperately, but do not put them all together with GLFW. It may cause some error when running the code)

```
    View->Other Windows->Property Manager
    Add Existing Property Sheet
```

4: Run code test:

GLFW/GLEW/GLM Test:

Add opengl_example/helloworld.cpp provided by LearnOpenGL into your project

NanoGui Test:

Add nanogui_example/example3.cpp provided by NanoGUI into your project

Done

# Reference Links

Xcode verison of NanoGUI configuration: [http://jody-lu-blog.logdown.com/posts/1533525](http://jody-lu-blog.logdown.com/posts/1533525).

Thanks for Jody Lu's help with Mac's configuration on Nanogui.

GLEW: [https://github.com/nigels-com/glew](https://github.com/nigels-com/glew)

GLFW: [https://github.com/glfw/glfw](https://github.com/glfw/glfw)

GLM: [https://github.com/g-truc/glm](https://github.com/g-truc/glm)

FreeGLUT: [http://freeglut.sourceforge.net](http://freeglut.sourceforge.net)

AntTweakBar: [http://anttweakbar.sourceforge.net/doc/](http://anttweakbar.sourceforge.net/doc)

NanoGui: [https://github.com/wjakob/nanogui](https://github.com/wjakob/nanogui)

Learn OpenGL: [https://github.com/JoeyDeVries/LearnOpenGL](https://github.com/JoeyDeVries/LearnOpenGL)

STB: [https://github.com/nothings/stb](https://github.com/nothings/stb)
