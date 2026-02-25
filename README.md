# BlindMaster
Parent repository for BlindMaster, a cost-effective, efficient blinds controller.

## Structure
These three folders form the full stack for BlindMaster. 

### blinds_express
Provides the backend express.js code for the BlindMaster web server. It's equipped with job scheduling for setting blinds to a given position at a certain time, auto-emailing for password reset, account verification, and email/password changes.

### blinds_flutter
Provides Flutter app code for BlindMaster app. This communicates with the BlindMaster device over BLE during setup, as well as will the BlindMaster backend server for regular use. Setup, deletion, and control of devices are all handled through the app.

### Blinds_XIAO
Provides C++ code in a PlatformIO project structure for Seeed Studio ESP32C6. Uses an event-driven architecture (currently in development on taskdrivenpowersave branch), capitalizing on features of FreeRTOS on ESP32C6 like event queues, semaphores, and light sleep mode.

## Upcoming
- Once BMS system is developed on taskdrivenpowersave branch, this will replace main and the project may be released.
- Will release app on testflight and hardware designs will be open-sourced.