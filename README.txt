ASSUMING RUNNING ON WINDOWS 10 & C++:

-----------------------------------------
OPEN PROPERTY PAGES OF PROJECT;
-   UNDER PROJECT / DEBUG  / VIEW 
  - SELECT "<YOUR_PROJECT> PROPERTIES"

C/C++ -> General -> Additional Include Directories
$(SolutionDir)\include
put SFML include folder in here aka "SFML". (already included in this GitHub.)

C/C++ -> Preprocessor
  * SMFL_STATIC
  * WIN32
  * _DEBUG
  * _WINDOWS

Linker -> General -> Additional Library Directories
$(SolutionDir)\lib

put SFML lib folder stuff in here. (already included in this GitHub.)

Linker -> Input -> Additional Dependencies :

openal32.lib
opengl32.lib
sfml-system-d.lib
sfml-graphics-d.lib
sfml-window-d.lib
flac.lib
freetype.lib
ogg.lib
sfml-audio.lib
sfml-graphics.lib
sfml-window.lib
sfml-system.lib
sfml-main.lib
sfml-network.lib
vorbis.lib
vorbisenc.lib
vorbisfile.lib


When done, build project by CTRL + B or right-clicking the <PROJECT_NAME> on the Solution Explorer tab and selecting "Build".

If you have errors executing program "unloaded /bin/-2.lib/.dll" file
AFTER BUILDING x64 folder will generate , hence in your folder copy the contents from "Debug" into the most outer x64 folder
then create a "Release" folder and copy contents from this github into there. 
