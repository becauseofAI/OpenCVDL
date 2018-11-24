![](./windows/python/Michael_Jordan_Pose_Python.jpg)  
# OpenCVDL
:smirk:Use OpenCV 4.0+ to play Deep Learning!
# Windows
## Easy Start
Prerequisites as follow:
+ OpenCV 4.0+
+ Python 2.7 or 3.5+ (Anaconda is recommended)
+ Visual Studio 2015+ (vc14 or vc15)
+ Visual Studio Code (optional but recommended)  

To download [opencv-4.0.0-vc14_vc15.exe](https://jaist.dl.sourceforge.net/project/opencvlibrary/4.0.0/opencv-4.0.0-vc14_vc15.exe)
and execute it to install. 

Add the opencv ```bin``` to your Path environment variable:
```
path\to\opencv\build\x64\vc14\bin
```
Copy the opencv ```pyd``` file which is  matched with your python version to the python ```site-packages``` directory:
```C++
path\to\opencv\build\python\cv2\python-3.6\cv2.cp36-win_amd64.pyd // python 3.6
```
```C++
your\python\path\Anaconda3\Lib\site-packages\ // Anaconda3 v5.2.0
```
Set the VS Project Properties as follow.  
VC++ Directories -> Include Directories:
```C++
path\to\opencv\build\include
path\to\opencv\build\include\opencv2
```
VC++ Directories -> Library Directories:
```C++
path\to\opencv\build\x64\vc14\lib
```
Linker -> Input -> Additional Dependencies:
```C++
opencv_world400d.lib // Debug x64
opencv_world400.lib // Release x64
```
## Now Enjoy
### OpenPose
```
git clone --recursive https://github.com/becauseofAI/OpenCVDL.git
```
To download the ```caffemodel``` from [here](https://github.com/becauseofAI/OpenCVDL/blob/master/windows/cpp/openpose/openpose.cpp#L5) and then put it in the directory of ```model/caffe/openpose/```.  
Now play as follow:
```python
python openpose.py
```
```C++
openpose.cpp //Build it in Visual Studio
```

## Others
:octocat:All you need is to **Star** and **Follow** me.



