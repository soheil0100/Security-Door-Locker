# Security Door Locker System

A GSM-based smart security door locking system built using Arduino.  
This system allows remote door control via SMS commands and integrates motion detection for enhanced security.

---

## Overview

The Security Door Locker is designed to provide remote and automated access control using GSM communication.  
Users can lock, unlock, and check door status via SMS commands.

The system integrates:

- GSM module (SMS control)
- PIR motion sensor (intrusion detection)
- Servo motor (door locking mechanism)
- Buzzer alarm system

---

## Features

- Remote door control via SMS (OPEN / CLOSE / CHECK)
- Motion detection using PIR sensor
- Alarm activation on intrusion
- Status verification through SMS
- Designed and simulated using Proteus

---

## Hardware Components

- Arduino Uno
- GSM Module (SIM800 / SIM900 compatible)
- PIR Motion Sensor
- Servo Motor
- Buzzer
- Power Supply

---

## Software

- Arduino IDE (.ino file included)
- Proteus simulation project included
- HEX file generated for deployment

---

## Project Structure

```
Security-Door-Locker/
/
/// firmware/
//// security_door_locker.ino
/
//// simulation/
///// proteus-project.pdsprj
/
/// images/
    /// simulation.png
```

---

## How It Works

1. The GSM module receives SMS commands.
2. The system verifies the sender number.
3. If the command is valid:
   - `OPEN`  Unlock door
   - `CLOSE`  Lock door
   - `CHECK`  Send door status
4. PIR sensor monitors movement and activates alarm if triggered.

---

## Security Note

The phone number for authorization is hardcoded in the source code.  
Modify it inside the firmware before deployment.

---

## Future Improvements

- Password-based SMS authentication
- Mobile application integration
- Cloud connectivity (IoT upgrade)
- Encrypted communication

---

## License

This project is licensed under the MIT License.
See the LICENSE file for details.

---

## Author

Developed by Soheil Ahmadi  
Open-source project for educational and development purposes.
