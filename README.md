# Vehicle Number Plate Detection System using ESP32

This project entails developing a system for vehicle number plate detection, utilizing an ESP32 microcontroller and a camera module. The hardware components include an ESP32 board, an ESP32 CAM Module, and a 16x2 LCD Display, while the software stack comprises Python OpenCV and the Arduino IDE.

## Procedure

1. **Hardware Setup**: Connect the camera module to the ESP32 board to capture images of passing vehicles.
2. **Image Preprocessing**: Enhance image clarity and reduce noise through preprocessing techniques.
3. **Plate Localization**: Utilize image processing techniques like edge detection and contour analysis to locate the number plate region within the image.
4. **Optical Character Recognition (OCR)**: Apply OCR algorithms to extract text from the localized number plate region.
5. **Character Segmentation and Cleanup**: Segment individual characters for better accuracy and clean up extracted text if necessary.
6. **Display or Transmission**: Display the detected number plate on a connected LCD display or transmit the information to a remote server for further processing.
7. **Integration**: Extend the system's functionality by integrating it with other components or systems.

## Hardware Setup

![Block Diagram](block_diagram.png)

The block diagram visually illustrates the hardware setup, encompassing the ESP32 module, ESP32 CAM module, and the LCD display.

### Hardware Components Description

- **ESP32 Module**: A versatile microcontroller suitable for various applications, including IoT.
- **ESP32 CAM Module**: A development board with an onboard camera, ideal for IoT applications and DIY projects.
- **16x2 LCD Display**: Used to display alphanumeric information in electronic devices.

## Software Description

- **Python OpenCV**: A library for solving computer vision problems.

### Code Overview

#### Arduino Code

Initializes the ESP32 CAM module, establishes WiFi connection, and handles image capture requests.

#### Python Code

Connects to the ESP32 CAM module's IP address to retrieve images and display the live stream from the camera.

#### Number Plate Detection Code

Utilizes OpenCV for plate detection and Tesseract OCR for text extraction.

## Summary

This project integrates hardware and software components to create a robust system capable of real-time vehicle number plate detection. It offers potential applications in various fields such as security, traffic management, and automated toll collection.

