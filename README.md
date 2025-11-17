# Solar Tracker Using Arduino Uno R3

## Project Purpose

The main goal of this project is to maximize solar panel efficiency by automatically tilting or rotating the panel toward the direction of maximum sunlight. This is achieved by using sensor feedback to follow sun rays throughout the day, ensuring more solar energy is captured continuously.

## What the Project Does

The solar tracker system uses four LDR (Light Dependent Resistor) sensors fitted to the corners of a solar panel and two servo motors controlled by an Arduino Uno R3. The microcontroller reads sunlight intensity from the sensors and adjusts the position of the panel to always face the brightest spot in the sky (the sun).

## Project Workflow

1. **Component Procurement:**  
   Identified and acquired the necessary components—Arduino Uno R3, servo motors, LDR sensors, resistors, etc.

2. **Firmware Development:**  
   Wrote and uploaded the embedded code onto the microcontroller to read LDR values and control servo positions accordingly.

3. **Hardware Design & Assembly:**  
   Completed interfacing all sensors and actuators on a breadboard and mounted them on the solar panel structure.

4. **Debugging & Testing:**  
   Faced and resolved several interfacing and logic bugs during integration. Calibrated the sensors for accurate sunlight tracking.

5. **Final Assembly & Artwork:**  
   Enhanced the visual and physical presentation for demonstration, including proper cable management and housing.

## Components Used

- Arduino Uno R3 microcontroller
- 2 × Servo Motors for dual-axis movement
- 4 × LDR (Light Dependent Resistor) sensors
- 4 × 10kΩ resistors (for voltage dividers with LDRs)
- Small solar panel (for demo or practical use)
- Breadboard & jumper wires
- Mounting structure for the panel and sensors

![Circuit Diagram](images/solar-tracker-circuit-diagram.png)

## How It Works

1. Four LDRs are positioned at the panel’s corners.
2. Arduino continuously samples analog values from each LDR.
3. It compares these values to determine which direction receives the most sunlight.
4. Based on the difference, Arduino moves the servo motors to tilt/rotate the solar panel toward the brightest position.
5. This process enables real-time tracking of the sun for optimal exposure.

## Steps to Reproduce

- Assemble the hardware as per the circuit diagram.
- Make all connections: LDRs (with resistors) to Arduino analog pins, servos to PWM pins, and panel to servo mount.
- Upload the firmware (to be added in the `/code` directory when available) to the Arduino Uno R3.
- Power up the system and verify that the panel follows movements of a light source or sunlight during the day.


![Assembly Photo](images/solar-tracker-assembly.jpg)
![Demo Photo](images/solar-tracker-demo.jpg)

## Challenges and Learnings

- My first hands-on experience in embedded systems and firmware development.
- Learned sensor interfacing techniques, including working with analog sensors and voltage dividers.
- Gained foundational skills in hardware design and system integration.
- Understood debugging principles, including pinpointing electrical and code-level mistakes during integration.

## Future Scope & Improvements

- Integrate data logging or wireless monitoring (ESP32).
- Make system weatherproof for prolonged outdoor use.
- Use larger servos and a bigger solar panel for real applications.
- Add an LCD or IoT dashboard for real-time tracking data.
