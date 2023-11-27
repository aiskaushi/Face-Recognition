# Face-Recognition
Face Recognition With Raspberry Pi and OpenCV
Basic and Initial Requirements
How to Flash the Old 'Buster' Raspberry Pi OS to a Micro-SD
Download this OS raspios_armhf

Enable camera and SSH
$ sudo reboot
Try to run 
$ Raspistill -o test.jpg
      $ Sudo apt-get  update
$ Sudo apt-get  upgrade
$ Raspistill -o test.jpg
Install picamera
$ sudo apt-get update
$ sudo apt-get install python-picamera python3-picamera

Open a Python 3 editor, such as Thonny Python IDE:
Open a new file and save it as camera.py.
Note: it’s important that you never save the file as picamera.py.
    **Setting Up Open-CV and Facial Recognition From Scratch**
1.$ pip install picamera[array]
2.$ Sudo apt-get update
3.$ Sudo apt-get upgrade
4.$ sudo apt install cmake build-essential pkg-config git
5.$ sudo apt install libjpeg-dev libtiff-dev libjasper-dev libpng-dev libwebp-dev libopenexr-dev
6.$ sudo apt install libavcodec-dev libavformat-dev libswscale-dev libv4l-dev libxvidcore-dev libx264-dev libdc1394-22-dev libgstreamer-plugins-base1.0-dev libgstreamer1.0-dev
7.$ sudo apt install libgtk-3-dev libqtgui4 libqtwebkit4 libqt4-test python3-pyqt5
8.$ sudo apt install libatlas-base-dev liblapacke-dev gfortran
9.$ sudo apt install libhdf5-dev libhdf5-103
$ sudo apt install python3-dev python3-pip python3-numpy
We must now expand the swapfile before running the next set of commands. To do this type and enter into the Terminal the following line.

10.$ sudo nano /etc/dphys-swapfile
       The change the number on CONF_SWAPSIZE = 100 to CONF_SWAPSIZE=2048. 
       
11.$ sudo systemctl restart dphys-swapfile
12.$ git clone https://github.com/opencv/opencv.git
13.$ git clone https://github.com/opencv/opencv_contrib.git
14.$ mkdir ~/opencv/build
15.$ cd ~/opencv/build
16.$ cmake -D CMAKE_BUILD_TYPE=RELEASE \
17.$ -D CMAKE_INSTALL_PREFIX=/usr/local \
18.$ -D OPENCV_EXTRA_MODULES_PATH=~/opencv_contrib/modules \
19.$ -D ENABLE_NEON=ON \
20.$ -D ENABLE_VFPV3=ON \
21.$ -D BUILD_TESTS=OFF \
22.$ -D INSTALL_PYTHON_EXAMPLES=OFF \
23.$ -D OPENCV_ENABLE_NONFREE=ON \
24.$ -D CMAKE_SHARED_LINKER_FLAGS=-latomic \
25.$ -D BUILD_EXAMPLES=OFF ..
 
26. $ cmake ..
27.$ make -j$(nproc)


This | make | Command will take over an hour to install and there will be no indication of how much longer it will take. It may also freeze the monitor display. Be ultra patient and it will work. Once complete you are most of the way done. Then we will resume terminal commands.
28.$ sudo make install
29.$ sudo ldconfig
30.$ pip3 install face-recognition --no-cache-dir
This | pip install face-recognition| Command will take over 40 mins to install and there will be no indication of how much longer it will take. Be ultra patient and it will work. Once complete you are most of the way done. Then we will resume terminal commands.
31.$ pip3 install imutils


We must now return the swapfile before running the next set of commands. To do this type into Terminal this line.
32.$ sudo nano /etc/dphys-swapfile


The change the number on CONF_SWAPSIZE = 2048 to CONF_SWAPSIZE=100. Having done this press Ctrl-X, Y, and then Enter Key to save these changes. This returns the Swapfile to normal. To have these changes affect anything we must restart the swapfile by entering the following command to the terminal. Then we will resume terminal Commands as normal.

33.$ sudo systemctl restart dphys-swapfile
34.$ git clone https://github.com/carolinedunn/facial_recognition
