# Smart Home System using Atmega32 AVR
This project demonstrates the implementation of a Smart Home System using the Atmega32 AVR microcontroller. The system includes an LCD display, keypad, LM35 temperature sensor, LDR (Light-Dependent Resistor), buzzer, and a DC motor controlled by PWM. It provides a user interface for access control, temperature monitoring, and automated light control, creating a basic but functional smart home system.

# Features
1. Access Control
Users must enter a PIN (default: 1234) to access the system.
After three incorrect attempts, the system blocks further access for 30 seconds.
2. Main Screen Options
Temp: Displays the current temperature as measured by the LM35 sensor.
Door: Toggles the door lock (simulated).
Light: Toggles the light (simulated).
More: Navigates to the second screen for additional options.
3. Second Screen Options
Auto Light: Enables automatic light control using the LDR to sense ambient light levels.
Log Out: Logs the user out of the system and returns to the PIN screen.
Back: Returns to the main screen.
4. Temperature-Controlled DC Motor (Fan)
30°C: The fan starts running.
35°C: The fan speed increases.
40°C: The fan reaches its maximum speed.
60°C: The system triggers the buzzer, acting as a fire alarm.

* Second screen with options:
  1. Auto Light: Set light automatically using LDR.
  2. Log Out: Log out of the system.
  3. Back: Go back to the main screen.
 
* DC motor (Fan) controlled by LM35 temperature sensor:
  * 30°C: Start working.
  * 35°C: Increase speed.
  * 40°C: Maximum speed level.
  * 60°C: Activate buzzer as a fire alarm.
# Components
Atmega32 AVR Microcontroller: Core of the system.
LM35 Temperature Sensor: Measures the temperature for fan control.
LDR (Light-Dependent Resistor): Used for automatic light control.
DC Motor: Represents the fan, controlled by the PWM signal based on temperature readings.
Keypad: Used for entering the PIN and interacting with the system.
LCD: Displays system status and options.
Buzzer: Sounds an alarm when the temperature exceeds 60°C.

# How It Works
Upon startup, users are prompted to enter a PIN for access. If the correct PIN is entered, the user can interact with the system through the main and secondary screens.
The LM35 temperature sensor continuously monitors the room temperature, controlling the fan's speed based on the thresholds defined above.
The LDR allows the light to be automatically toggled based on the room’s brightness when the "Auto Light" mode is activated.
If the temperature reaches 60°C, the system activates the buzzer, signaling a potential fire hazard.

# How to Run

Hardware Setup:

Connect the Atmega32 microcontroller to the components (LCD, keypad, LM35, LDR, buzzer, and DC motor) as per the circuit diagram.
Program the microcontroller with the provided code using an AVR programmer.
Interaction:

On powering up, the system will request a PIN for access.
After successful login, the user can interact with the system using the LCD and keypad interface.
The fan will automatically adjust its speed based on the room temperature.
The light will toggle based on user input or automatically via the LDR when the "Auto Light" mode is enabled.

 # Installation
 To install the project, follow these steps:

  1. Clone the repository
  2. Open the project in your preferred IDE
  3. Compile and upload the code to the Atmega32 AVR microcontroller

# Usage

After uploading the code, interact with the system using the keypad and LCD. The main screen will display the available options, and you can navigate through the system using the keypad. The second screen offers additional options, such as auto light control and logging out of the system.

# Contributing
Feel free to leave a suggestion or point out a problem in the issues.

# Screenshots
![image](https://github.com/HongYue1/Smart-Home-System/assets/87040288/d59cfba4-09f8-435b-b79e-cc4b2d2d6922)
![image](https://github.com/HongYue1/Smart-Home-System/assets/87040288/98fee4bc-997f-4cea-a74b-3ed8f8d3135f)
![image](https://github.com/HongYue1/Smart-Home-System/assets/87040288/5f701837-9751-47f3-afcf-6d236bb4ecfd)
![image](https://github.com/HongYue1/Smart-Home-System/assets/87040288/e0dad806-15b6-43ac-a1b7-dd976734f4a8)



