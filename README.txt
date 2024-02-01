ASSUMING RUNNING ON WINDOWS 10 & C++:

-----------------------------------------
OPEN PROPERTY PAGES OF PROJECT;
-   UNDER PROJECT / DEBUG  / VIEW 
  - SELECT "<YOUR_PROJECT> PROPERTIES"

C/C++ -> General -> Additional Include Directories
$(SolutionDir)\include
put SFML include folder in here aka "SFML". (already included in this GitHub.)


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
