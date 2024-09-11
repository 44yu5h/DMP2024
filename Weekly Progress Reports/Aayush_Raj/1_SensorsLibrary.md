# Sensors Library

The library lives [here](https://github.com/44yu5h/rpi_sensor_libs)

Most of the libraries for embedded development are written in C/C++, MicroPython, and CircuitPython (a variant of MicroPython). MicroPython and CircuitPython are different from the normal Python. You can say they are *mini* versions of the normal Python. To use these libraries on Raspbberry Pi we will use a software-layer: **adafruit_blinka** library. It translates the CircuitPython hardware API to whatever library the Linux board provides.



We have implemented several types of features/sensors

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

These libraries are embedded into `python3.xx/site-packages/` folder while the creation of the OS so that they can be used from any activity.

This was the most feasible and also the only solution I could see since the activities are containerized. So to make my libraries available to any activity (i.e. globally) I would have had to add them manually in the repo of each of them. Instead, we are adding them to site-packages which is used in each of the activities.



# Screenshots:

### Servo Motor:

<img src=https://raw.githubusercontent.com/44yu5h/rpi_sensor_libs/master/assets/servo.gif>

<br>

### PWM (Brightness Control):

<img src="https://raw.githubusercontent.com/44yu5h/rpi_sensor_libs/master/assets/PWM%20(brightness%20control).gif" height=300>

<br>

### Push Button:

<img src=https://raw.githubusercontent.com/44yu5h/rpi_sensor_libs/master/assets/btn.gif>

<br>

### Oled Display:

<img src=https://raw.githubusercontent.com/44yu5h/rpi_sensor_libs/master/assets/oled.jpg>
