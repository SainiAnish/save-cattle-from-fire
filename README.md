# save-cattle-from-fire


Objective : 
To design an IoT-based safety system that detects fire in cattle stables and automatically frees the cattle by releasing the ropes, while simultaneously triggering an alarm to alert farmers.

Problem Statement : 
In rural and farming areas, cattle are often tied to poles inside stables. In case of a fire outbreak (due to electrical faults, dry fodder ignition, or other accidents), the animals cannot escape as they are tied. This leads to injuries or death. There is often no immediate human presence to rescue them.

Proposed Solution : 
We implement an IoT-based system using fire sensors and a servo/solenoid rope release mechanism. The system detects fire, alerts the farmer via buzzer and IoT notification, and automatically unties the cattle by loosening the rope.

Components Used : 
Arduino/NodeMCU (ESP8266) – Microcontroller to process sensor data and control release mechanism.

Fire/Flame Sensor – Detects flames or sudden temperature rise.

Flex Sensor – Monitors tension on the rope to ensure cattle are tied.

Buzzer – Gives a loud local alarm when fire is detected.

Servo Motor / Solenoid Lock – Mechanism to automatically release or cut the rope.

IoT Module (Wi-Fi) – Sends alert notifications to farmer’s mobile.

Power Supply / Battery – To keep system running even during power cuts.


Working Principle : 

Normal Condition: Cattle are tied to a pole with the rope attached to a servo lock system. Sensors are active but idle.

Fire Detection: Flame sensor detects fire or high temperature.

Flex sensor ensures the cattle is tied before taking action.

Alert & Action: Buzzer starts to alert nearby people.

IoT module sends a notification to the farmer’s mobile app or SMS.

Servo motor rotates to open the rope lock, freeing the cattle.

Post-Release: Cattle can run to a safer place.

Manual Reset: Once danger is over, farmer can re-tie cattle and reset the system.



Implementation Steps : 

Install flame sensors at multiple points in the stable for full coverage.

Mount the flex sensor on the rope to detect tension (cattle tied).

Connect the servo motor to a rope-lock mechanism.

Interface all components with NodeMCU/Arduino.

Program the controller to:

Continuously monitor fire sensor values.

Activate buzzer and IoT alert when threshold is crossed.

Trigger servo to release rope.

Test in a controlled environment before deploying in actual stables.



Advantages : 

Saves cattle lives by giving them a way to escape.

Works even when no humans are present.

Sends real-time alerts to the farmer.

Low cost and easy to install.



Future Enhancements :

Add smoke sensor for early fire detection.

Integrate with CCTV for real-time monitoring.

Solar-powered system for remote areas.

GPS tracking of cattle after release.
