# mexopencv
<font size=8>How to use opencv in matlab (Win)

<font size=6>

Note: Only the 3.4.1 release is supported by mexopencv.

<font size=6>**Prerequisite**

<font size=4> 
Matlab

Opencv3.4.1
<font size=6>

1. Opencv<font size=4> 

You can follow the [tutorial](https://github.com/kyamagu/mexopencv/tree/v3.4.1?tab=readme-ov-file#structure) to install opencv by yourself, or you can download the [compiled file](https://github.com/Zhang-CH0/mexopencv.git). (The Opencv3.4.1 with opencv_contrib-3.4.1 was built by cmake and compiled by visual studio 2015, so you do not compile anymore.)

If you use this compiled files, firstly，you need to (add your_path/mexopencv/x64/vc14/bin/ to the environment path).

<font size=6>

2. Mexopencv
<font size=4>


>> In matlab

>> mex - setup C++  % choose Microsoft Visual C++ 2015 compiler

>> addpath('.\mexopencv-3.4.1')

>> addpath('.\mexopencv-3.4.1\opencv_contrib')

>> mexopencv.make('opencv_path','.\mexopencv', 'opencv_contrib',true)


If all goes well, the compilation is successful

>> cv.getBuildInformation() %check opencv
