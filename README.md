  
**GAS LEAKAGE DETECTION AND ALERT SYSTEM**

 **Introduction**

The Gas Leakage Detection and Alert System is an electronic safety system designed to detect the presence of combustible gas and provide an immediate warning.

The system uses a gas sensor to continuously monitor the surrounding environment. When the detected gas concentration exceeds the predefined threshold, the Arduino activates a single LED and buzzer to provide visual and audible alerts. The gas status is also displayed on an LCD.

 **Objective**

\- To detect the presence of gas leakage.  
\- To continuously monitor the surrounding gas level.  
\- To provide an immediate LED and buzzer alert during gas leakage.  
\- To display the gas status on an LCD.  
\- To develop a simple and low-cost gas safety monitoring system.

 **Components Required**

1\. Arduino UNO  
2\. MQ-series Gas Sensor  
3\. 16×2 LCD with I2C module  
4\. LED – 1  
5\. Buzzer – 1  
6\. Resistor for LED  
7\. Breadboard  
8\. Jumper wires  
9\. USB cable / suitable power supply  
10\. Servo motor – if included in the implemented setup

**Working Principle**

The gas sensor continuously senses the presence of combustible gases in the surrounding environment.

The sensor sends an electrical signal to the Arduino UNO. The Arduino processes the sensor reading and compares it with the predefined threshold value.

Under normal conditions, the system remains in the monitoring state.

**When the gas level exceeds the threshold**:

1\. Arduino detects the abnormal gas level.  
2\. The LCD displays the gas leakage status.  
3\. The LED turns ON.  
4\. The buzzer is activated to produce an audible warning.  
5\. The system continues monitoring the gas level.

When the gas level returns below the threshold, the alert outputs are deactivated and the system returns to monitoring.

 **LED and Buzzer Alert**

The project uses one LED and one buzzer for leakage indication.

**Normal Condition**

\- LED → OFF  
\- Buzzer → OFF  
\- LCD → Safe/Monitoring status

**Gas Leakage Detected**

\- LED → ON  
\- Buzzer → ON  
\- LCD → Gas Leakage Alert

The LED provides a visual indication, while the buzzer provides an audible warning so that the leakage can be noticed immediately.

 **LCD Display**

A 16×2 LCD with an I2C module is used to display the system status and gas-related information.

The LCD can display messages such as:

 \-SAFE  
 \- GAS LEVEL  
\- GAS LEAKAGE ALERT  
\- SYSTEM MONITORING

The I2C module reduces the number of Arduino pins required for LCD communication.

 **Arduino UNO**

Arduino UNO acts as the main controller of the system.

Its functions include:

\- Reading the gas sensor output.  
\- Processing the sensor value.  
\- Comparing the value with the threshold.  
\- Controlling the LED.  
\- Activating the buzzer during gas leakage.  
\- Updating the LCD display.

 **Flow of Operation**

START  
↓  
Initialize Arduino, Gas Sensor, LCD, LED and Buzzer  
↓  
Read Gas Sensor  
↓  
Check Gas Level  
↓  
Is Gas Level Above Threshold?  
↓  
YES  
↓  
LED ON \+ Buzzer ON  
↓  
Display GAS LEAKAGE ALERT  
↓  
NO  
↓  
LED OFF \+ Buzzer OFF  
↓  
Display SAFE / SYSTEM MONITORING  
↓  
Repeat Monitoring

 **Advantages**

\- Simple and low-cost design.  
\- Real-time gas monitoring.  
\- Immediate visual and audible warning.  
\- Easy to implement and demonstrate.  
\- LCD provides clear system status.  
\- Suitable for educational and prototype applications.

 **Applications**

\- Domestic gas leakage monitoring.  
\- Kitchens and cooking areas.  
\- Laboratories.  
\- Small-scale industries.  
\- Gas storage areas.  
\- Industrial safety prototypes.

 **Future Scope**

The system can be further enhanced by adding:

\- Automatic gas supply shut-off mechanism.  
\- Automatic exhaust fan activation.  
\- IoT-based remote monitoring.  
\- SMS or mobile notification.  
\- Cloud-based data monitoring.  
\- Multiple gas sensors for wider-area monitoring.

 **Conclusion**

The Gas Leakage Detection and Alert System demonstrates real-time gas leakage detection using a gas sensor and Arduino UNO.

When the detected gas level exceeds the predefined threshold, the system activates both a LED and buzzer to provide immediate visual and audible warnings. The LCD displays the corresponding system status.

The project provides a simple, economical and effective prototype for gas leakage detection and safety monitoring.  
