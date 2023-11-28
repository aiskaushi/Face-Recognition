# Face Recognition with Raspberry Pi and OpenCV

## Table of Contents
- [Introduction](#introduction)
- [Basic and Initial Requirements](#basic-and-initial-requirements)
  - [Flashing the OS](#flashing-the-os)
  - [Enabling Camera and SSH](#enabling-camera-and-ssh)
  - [Installing PiCamera](#installing-picamera)
  - [Setting Up Python Environment](#setting-up-python-environment)
- [Setting Up OpenCV and Facial Recognition](#setting-up-opencv-and-facial-recognition)
  - [Installing OpenCV Dependencies](#installing-opencv-dependencies)
  - [Building and Installing OpenCV](#building-and-installing-opencv)
  - [Installing face_recognition and imutils](#installing-face_recognition-and-imutils)
- [Running the Facial Recognition Program](#running-the-facial-recognition-program)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project guides you through setting up face recognition on a Raspberry Pi 4 using OpenCV and the face_recognition library.

## Basic and Initial Requirements

### Flashing the OS
1. Download the OS: [raspios_armhf](#)
2. Enable camera and SSH:
    ```bash
    $ sudo reboot
    $ raspistill -o test.jpg
    $ sudo apt-get update
    $ sudo apt-get upgrade
    $ raspistill -o test.jpg
    ```

### Enabling Camera and SSH
- Follow the instructions for enabling the camera and SSH.

### Installing PiCamera
```bash
$ sudo apt-get update
$ sudo apt-get install python-picamera python3-picamera





