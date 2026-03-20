# PinLab IoT Solutions Repository
This repository serves as a comprehensive collection of project ideas, firmware examples, and software solutions designed for the PinLab Internet of Things Laboratory. The contents are intended to be used as a reference for building IoT systems, focusing on the practical application of MicroPython to bridge the gap between hardware control and high-level logic using the ESP8266 microcontroller.

!​Technical Scope

​The primary objective of these projects is to provide a solid foundation for hardware-software interaction within the PinLab ecosystem. Each project is designed to be modular and serves as a conceptual starting point for custom builds, demonstrating reliable interrupt handling and interface management.

!​Core Technologies and Hardware

​System on Chip: ESP8266 (NodeMCU compatible)

​Development Environment: MicroPython

​Display Technologies: SSD1306 (OLED) and ST7735 (TFT)

​Interaction Modules: Passive buzzers, tactile buttons, and sensors

!​Hardware Configuration (PinLab GPIO Mapping)

​To ensure compatibility with the PinLab board layout and the provided code examples, use the following pin assignments:

!​!Displays and Indicators

​OLED SCL: GPIO 5 (D1)

​OLED SDA: GPIO 4 (D2)

​TFT CS: GPIO 15 (D8)

​TFT DC: GPIO 2 (D4)

​TFT RES: GPIO 0 (D3)

​RGB LED (WS2812B): GPIO 14 (D5)

!!​Input and Sensors
​Tactile Button (Left): GPIO 13 (D7)

​Tactile Button (Right): GPIO 16 (D0)

​Environmental Sensor (DHT): GPIO 12 (D6)

​Analog Input (Light/Potentiometer): ADC0 (A0)

​!!Sound and Actuators
​Passive Buzzer: GPIO 14 (D5) or GPIO 12 (D6) depending on board revision

​Servo Motor Signal: GPIO 2 (D4)

!​Project Ideas and Implementation

!!​Morse Code Telegraph System

​A digital-to-analog communication interface. It features manual input via tactile buttons and automated broadcasting for pre-defined signals, managing precise timing for signals through the buzzer and LEDs.

!!​Environmental Monitoring Station

​A data-driven application that polls atmospheric sensors to display metrics on the OLED screen. Includes error handling for sensor communication and data smoothing.

!!​Hierarchical UI Menu System

​A firmware component for the TFT display providing a structured navigation menu. This project demonstrates state-machine logic for switching between different IoT modes using physical buttons.

!!​Advanced RGB Signal Control

​Focuses on visual status indication using WS2812B chains. It enables complex lighting patterns, color gradients, and visual alerts for system notifications.

!​Deployment

1.​Flash the ESP8266 with the latest MicroPython firmware.

​2.Transfer the Python source files to the board using Thonny or a similar tool.

​3.Verify pin assignments in the configuration files against the mapping provided above.

4.​Execute main.py to initialize the laboratory logic.

!​Project Attribution

​Developed by Studio Amateur
