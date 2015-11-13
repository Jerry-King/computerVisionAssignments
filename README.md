# computerVisionAssignments
Assignments Repo for Computer Vision course at Utrecht University, Maguell and Jerry

## Environment Setup

Please note that we are using Microsoft Visual Studio 2013 as our IDE since we are working on Windows.
OpenCV version for this repo is 2.4.11, Boost version: 1.59.0, and we also use OpenGL.

### Step 00:

Install Windows Visual Studio 2013, OpenCV 2.4.11, Boost 1.59.0 and OpenGL

### Step 01:

For Boost 1.59, do as follows after you unzip the zip file you got from Boost's website:

1. Run cmd, and cd to the dir where you unzip the boost_1_59_0 (e.g. C:/boost_1_59_0/)

2. Run bootstrap.bat from cmd;

3. Wait for a minute;

4. Run "bjam --toolset=msvc-12.0 --build-type=complete stage" in cmd;

5. Wait for less than a day, patiently;

6. After a long time, add the new generated lib folder to path, e.g."C:\boost_1_59_0\stage\lib\". Don't forget to include a ";" before the folder's actual path.

7. Setup input lib in Visual Studio later.

8. Cheers!

### Step 02:

For OpenCV, extract the file you got from OpenCV website (make sure it's 2.4.11 for Windows) to any directory you want. By default: C:/opencv/.

1. Add opencv and opencv/.../lib to your path, e.g. "C:\opencv\" and "C:\opencv\build\x86\vc12\lib".

2. Add opencv/.../bin to your path, e.g. "C:\opencv\build\x86\vc12\bin".

### Step 03:

For OpenGL, get the FIVE files ready: glut.h, glut.lib, glut.dll, glut32.lib, glut32.dll.

1. Copy the header file to your VS/VC/include/gl directory, e.g. "C:\Program Files (x86)\Microsoft Visual Studio 12.0\VC\include\gl". Notice that you will need to create a "gl" folder under "include" since it was not there by default.

2. Copy the .dll files to your system32 folder, i.e. "C:\Windows\System32".

3. Copy the .lib files to your VS/VC/lib directory, e.g. "C:\Program Files (x86)\Microsoft Visual Studio 12.0\VC\lib".

4. Cheers!

### Step 04:

Do as the setup pdf file says, the input libs are:


opencv_core2411d.lib

opencv_highgui2411d.lib

opencv_imgproc2411d.lib

opencv_calib3d2411d.lib

opencv_contrib2411d.lib

OpenGL32.lib

boost_filesystem-vc120-mt-1_59.lib

boost_regex-vc120-mt-gd-1_59.lib

boost_system-vc120-mt-gd-1_59.lib

### Step 05:

Cheers!
