# Hager Smart Home

## Background

I am currently studying Software Development for Embedded Systems and IoT. With a prior background in fullstack web development, I wanted to create a project that would allow me to combine these two skill sets into a complete and functional IoT solution.

The idea behind this smart home system was to explore how hardware and software can work together to create meaningful, real-world services. I wanted to challenge myself with a project that involved both low-level programming on microcontrollers and high-level application development for the web. This project gave me the opportunity to build a system from the ground up—starting with soldering components and writing firmware, all the way to deploying a web interface accessible from anywhere in the world.

## Project Overview

This project is a smart home system that integrates multiple microcontroller (MCU) nodes to monitor and control various aspects of a home environment. At the core of the system, I use ESP32-based devices to handle tasks like motion detection, environmental monitoring, and communication between devices.

Currently, the system includes a **Mailbox Node** and a **Bridge Node**. The Mailbox Node detects when mail arrives and communicates this information via LoRa to the Bridge Node. The Bridge Node then sends the data via Wi-Fi to a Next.js application backend, which updates the frontend web interface, providing real-time notifications.

Future updates will include adding more MCU nodes to extend the system’s functionality, such as environmental sensors for monitoring temperature and humidity, as well as an improved web interface for better control and security.

## Tech Used

- **Hardware**:
    - ESP32 Wroom-32
    - Ra-02 SX1278 LoRa-chip
    - PIR Motion Sensor
    - SMA Antenna

- **Software**:
    - Next.js
    - Axios
    - TanStack React Query
    - Prisma
    - ESP-IDF

## What I've Learned

### Debugging  
After completing this project, I realized that debugging would become a major part of my development process. While debugging a web application is often just a matter of logging data to the console, debugging microcontrollers presents its own unique challenges. Solving bugs in this environment has been incredibly rewarding.

### Using Third-Party Code  
Since I used ESP-IDF for this project, which already includes a wide range of libraries tailored for nearly every ESP32 functionality, I encountered a challenge when there wasn’t an available library for LoRa communication. To overcome this, I cloned a repository containing code to control the Ra-02 chip for LoRa functionality. This experience taught me how to efficiently navigate and utilize third-party code.

### Programming and Project Structure  
My programming skills in C and TypeScript have significantly improved, and I now feel more confident in my overall development abilities. Given the size of this project and the plans to expand with more MCU nodes and features, I learned the importance of a clear and structured approach. I now have a solid understanding of how to organize a project for efficient workflow, scalability, and optimization.

## Future Features

This project is still in its early stages, and below are the features and functionality I plan to implement in future versions:

### For the Microcontrollers:
- Easy provisioning, enabling users to easily configure Wi-Fi for the devices.
- Encryption of data sent between the ESP32 devices via LoRa to enhance security.
- Implementation of FOTA for each ESP32.

### For the Web Application:
- User registration and login functionality.
- Customizable settings for the web interface to improve user experience.

And, of course, I plan to add more IoT nodes in the future to increase the system's capabilities.

## Extras

Throughout this project, I also gained valuable experience with Linux. I installed **Ubuntu Server LTS** on an old PC, which is now hosting the Next.js web application. Thanks to port forwarding, I can access my smart home system from anywhere in the world. This enables me to monitor my mailbox remotely and receive real-time notifications when I get mail. :)

For more information about what each submodule do, please read their README.md files!

Thanks for reading!!

---

### Contact

- **Email**: Johannbonde@hotmail.com  
- **LinkedIn**: [Johann Hagers's LinkedIn](https://www.linkedin.com/in/johann-bonde-hager-9424b531b/)
