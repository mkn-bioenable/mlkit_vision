# BioEnable ML Kit Vision Quickstart Sample App

## Introduction

This BioEnable ML Kit Quickstart app demonstrates how to use and integrate various vision based ML Kit features into your app.

## Feature List

Features that are included in this Quickstart app:
* [Object Detection]  Detect, track, and classify objects in real time and static images
* [Face Detection] Detect faces in real time and static images
* [Text Recognition] Recognize text in real time and static images
* [Barcode Scanning] can barcodes in real time and static images
* [Image Labeling] Label images in real time and static images
* [Custom Image Labeling - Birds] Label images of birds with a custom TensorFlow Lite model.
* [Pose Detection]  Detect the position of the human body in real time.

 
 
## How to use the app

This app supports three usage scenarios: Live Camera, Static Image, and CameraX enabled live camera.

### Live Camera scenario
It uses the camera preview as input and contains these API workflows: Object detection & tracking, Face Detection, Text Recognition, Barcode Scanning, and Image Labeling. There's also a settings page that allows you to configure several options:
* Camera
    * Preview Size - Specify the preview size of rear camera manually (Default size is chose appropriately based on screen size)
    * Enable live viewport - Prevent the live camera preview from being blocked by API rendering speed
* Object detection / Custom Object Detection
    * Enable Multiple Objects -- Enable multiple objects to be detected at once.
    * Enable classification -- Enable coarse classification
* Face Detection
    * Landmark Mode -- Toggle between showing no or all facial landmarks
    * Contour Mode -- Toggle between showing no or all contours
    * Classification Mode -- Toggle between showing no or all classifications (smiling, eyes open/closed)
    * Performance Mode -- Toggle between two operating modes (Fast or Accurate)
    * Face Tracking -- Enable or disable face tracking
    * Minimum Face Size -- Choose the proportion of the head width to the image width
* AutoML Image Labeling
    * AutoML Remote Model Name -- Allows you to specify an AutoML VisionEdge model to remotely download from the Firebase Console
    * AutoML Model Choices -- Toggle between using the remote or local AutoML model.
* Pose Detection
    * Performance Mode -- Allows you to switch between "Fast" and "Accurate" operation mode
    * Show In-Frame Likelihood -- Displays InFrameLikelihood confidence within the app

### Static Image scenario
The static image scenario is identical to the live camera scenario, but instead relies on images fed into the app through the gallery.

### CameraX Live Preview scenario
The CameraX live preview scenario is very similar to the native live camera scenario, but instead relies on CameraX live preview instead of the Camera2 live preview. Note: CameraX is only supported on API level 21+.

 
 
