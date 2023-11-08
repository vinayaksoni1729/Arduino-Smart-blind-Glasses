# Arduino Ultrasonic Distance Sensor

This is an Arduino project that utilizes an ultrasonic distance sensor to measure the distance to an object and display the results on the Serial Monitor. The code provided in this repository includes an Arduino sketch for interfacing with the ultrasonic sensor and reading distance measurements.

## Components

- Arduino board (e.g., Arduino Uno)
- Ultrasonic distance sensor (HC-SR04 or similar)
- Jumper wires


## Diagram
![1e3ea2ef-3a8e-48e1-882a-98640fbe6f27](https://github.com/vinayaksoni1729/Arduino-Smart-blind-Glasses/assets/113187290/5dc5fd41-edc6-470d-a1e3-bde66a0088bb)
## Wiring

Make the following connections between the Arduino and the ultrasonic sensor:

- Connect the trigger pin of the ultrasonic sensor to Arduino pin 2 (trig).
- Connect the echo pin of the ultrasonic sensor to Arduino pin 3 (echo).

## Arduino Sketch

The Arduino sketch provided in this repository is responsible for reading distance measurements from the ultrasonic sensor and displaying them on the Serial Monitor.

The key functions in the code include:

- `setup()`: Initializes the Serial communication and configures the trigger and echo pins.
- `calculate_distance(int trigger, int echo)`: Measures the distance by sending a trigger pulse and capturing the echo.
- `loop()`: Repeatedly calculates and displays the distance to the object in centimeters.

The distance is calculated based on the time it takes for the ultrasonic pulse to travel to the object and back.

## Usage

1. Upload the Arduino sketch to your Arduino board using the Arduino IDE.
2. Make sure the circuit connections are correctly set up as described in the wiring section.
3. Power up the Arduino board.
4. Open the Serial Monitor in the Arduino IDE (Ctrl + Shift + M) to view the distance measurements in centimeters.

You can adjust the delay in the `loop()` function to control how frequently distance measurements are displayed.

Feel free to modify and adapt this code for your specific distance sensing applications.

Happy measuring!
