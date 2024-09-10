# Sugar on Raspberry Pi

Hi! I am [Aayush Raj](github.com/44yu5h), studying in 1st year at BITS Pilani Goa, India. I was selected in the DMP 2024 program offered by C4GT. [Anurag Singh](https://github.com/drLite35) (selected in GSoC) and I were selected to work together on this project.

I will be talking only about my work here.

## Objectives achieved in this summer were:
 - Added a sensor library (having 10-15 sensor definitions)
 - Built a Camera (to use camera modules)
 - Built a Gallery Activity (shows media in ~/Pictures)
 - Built a Control Center to change RPi's settings via GUI
 - Added sensors to Turtle Art Activity
 - Made a setup video
 - Fixed Browser Activity

<br>

## Below are the objectives achieved by me:

# 1. [Sensors Library](SensorsLibrary.md)

The library lives [here](https://github.com/44yu5h/rpi_sensor_libs)

These libraries can be used globally from any activity.

### Features/Sensors implemented so far:

- Digital output
- Digital input
- PWM Output
- Delay
- Button
- HC-SR04 Ultrasonic distance sensor
- DHT11 Temperature and Humidity sensor
- OLED display
- Servo Motor
- DC Motor (not tested)

<br>

# 2. [Camera Activity](CameraActivity.md)

The library repo [here](https://github.com/44yu5h/rpi_camera_activity)

You can take pictures and videos with it as one would expect. It saves the media files in `~/Pictures/Camera`

### Features:
- Show/Hide the grid overlay.
- Flip the camera preview horizontally or vertically.
- Capture images by clicking the "Snap" button.
- Capture videos using "Video" button.
- Video timer indicator

<br>

# 3. [Gallery Activity](GalleryActivity.md)

This is a simple gallery that pulls up media files from `~/Pictures`.\
The latest modified files are displayed first.

On the toolbar, next, previous and delete buttons are for navigation and deletion respectively

### Keyboard Shortcuts:
- Previous Media: <kbd>Left</kbd> or <kbd>Back</kbd> key
- Next Media: <kbd>Right</kbd> or <kbd>Up</kbd> key
- Delete Media: <kbd>Delete</kbd> key 
- Play/Pause Video: <kbd>P</kbd> key

<br>

# 4. [Control Center Activity](ControlCenterActivity.md)

A control center application for Raspberry Pi, designed to manage and monitor various Raspberry Pi functionalities via a user-friendly interface.


### Features:
- **GPIO Control**: Control the GPIO pins on the Raspberry Pi.
- **I2C**: View and obtain addresses of connected I2C devices.
- **SPI**: View and obtain addresses of connected SPI devices.
- **Audio**: Check and manage connected speaker and microphone.
- **Camera**: View connected cameras.
- **Settings**: Control the state (on/off) of various settings such as I2C, SPI, VNC, Boot Splash, etc.

# 5. [TurtleArt RPi Plugin](TurtleArtRPiPlugin.md)

The repo lives [here]()

A plugin palette to add Blocks to TurtleArt to control sensors! It has a super simple installation process. Just run an "install requirements" block, wait for 2 minutes, and you are good to go!

### Added Blocks:
- GPIO input
- GPIO output
- Delay (ms)
- HIGH/LOW (1/0)
- HCSR04 sensor
- distance (for HCSR04)
- Oled display
- display text (for oled) 
