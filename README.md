# Pico Rubber Ducky – Payload-Focused Cybersecurity Toolkit

This project is a **custom USB Rubber Ducky built using a Raspberry Pi Pico and Adafruit CircuitPython**, with a **primary focus on developing and testing keystroke-injection payloads for cybersecurity research and penetration testing**.

It is based on the original **dbisu/pico-ducky** project and extends it with **custom hardware controls** and a **payload-centric workflow**.

---

## Project Overview

This repository documents the development of a **payload-oriented USB HID attack platform**.  
The primary goal of this project is **payload development**, not just device creation.

Key objectives include:

- Designing and testing custom **DuckyScript payloads**
- Rapid payload switching during testing
- Safe experimentation using hardware-controlled modes
- Stealth testing via USB visibility control
- A low-cost, portable platform for cybersecurity labs and demonstrations

The **Raspberry Pi Pico acts as the execution platform**, while the **payloads themselves are the core output** of this project.

---

## Project Focus

Unlike a standard pico-ducky setup, this project emphasizes **payload engineering and cybersecurity testing**, including:

- Custom keystroke-injection payloads
- Payloads for authorized penetration testing
- Demonstrations of common attack vectors
- Repeatable and controlled payload execution

---

## Hardware Modifications

To support efficient payload testing, the Raspberry Pi Pico has been physically modified with **soldered hardware controls**.

### Toggle Switches
- **Payload Selection Switches**  
  Switch between **three payloads**
- **Stealth / Invisible Mode Switch**  
  Disables USB mass-storage visibility

### Push Button
- **Safe / Setup Mode Button**  
  Prevents automatic payload execution and allows safe editing

These modifications allow **on-the-go control** without reflashing firmware or reconnecting jumpers.

---

## Payload System

Payloads are written in **DuckyScript** and executed via **USB HID keyboard emulation**.

### Using Payloads

1. Create or edit a DuckyScript payload
2. Copy the payload file to the **root of the CIRCUITPY drive**
3. Rename it to one of the following:

payload0.dd
payload1.dd
payload2.dd
payload3.dd

4. Use the hardware switches to select the desired payload
5. Plug the device into the target system

> ⚠️ If safe/setup mode is disabled, the selected payload will execute immediately after boot.

---

## Payloads in This Repository

*(This section will be populated as payloads are developed)*

- **Payload 0 – TBD**  
  Description coming soon

- **Payload 1 – TBD**  
  Description coming soon

- **Payload 2 – TBD**  
  Description coming soon

- **Payload 3 – TBD**  
  Description coming soon

Each payload is developed with a **specific security objective**, such as automation, attack simulation, or training.

---

## Software & Platform

- **Hardware:** Raspberry Pi Pico  
- **Firmware:** Adafruit CircuitPython  
- **Execution Method:** USB HID keyboard emulation  
- **Payload Format:** DuckyScript (`.dd`)  

---

## Credits & License

This project is a **fork and derivative work** of:

- **dbisu/pico-ducky**  
  https://github.com/dbisu/pico-ducky  

Licensed under the **GNU General Public License v2.0 (GPL-2.0)**.

All modifications, payloads, and documentation in this repository are released under **GPL-2.0**, in compliance with the original license.

---

## Ethical Use Disclaimer

This project is intended **strictly for educational purposes, cybersecurity research, and authorized penetration testing**.

⚠️ **Do not use this device or its payloads on systems you do not own or do not have explicit permission to test.**
