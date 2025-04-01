# Communication_protocol
Interview Preparation - I2C, SPI, UART, CAN, ETHERNET, LAN, UDP, IPMI,REDFISH, DBUS, IPC etc

# I2C
![image](https://github.com/user-attachments/assets/489ce3cd-cb04-4020-8ec8-0ccc26874612)
``` bash

Start Condition:
          The SDA line undergoes a transition from a high to a low voltage level
          before the SCL line shifts from high to low.
Stop Condition:
          The SDA line switches from a low to a high voltage level
          after the SCL line transitions from low to high.
Address Frame:
          A distinctive 7 or 10-bit sequence unique to each slave,
          enabling communication with the master.
Read/Write Bit:
          A solitary bit specifying whether the master sends data to the slave
          (low voltage level) or requests data from it (high voltage level).
ACK/NACK Bit:
          Following each frame in a message is an acknowledgment or non-acknowledgment bit.
          An ACK bit is transmitted back to the sender if an address or data frame was
          received successfully by the receiving device.

```
``` questions
Clock Stretching:
          It can introduce delays in the clock signal, impacting timing in certain devices.
Limited Speed:
          The limited clock frequency of I2C might make it unsuitable for high-speed applications.
What is the maximum speed of I2C?
          Standard mode operates at 100 kbit/s, while fast mode reaches speeds up to 400 kbit/s.
          High-speed mode can reach up to 3.4 Mbit/s.
Applications:
          Including sensors, displays, EEPROMs, and other peripheral devices. It is also used in
          system management applications such as power management and temperature monitoring.
```
```
How many devices can be connected to an I2C bus?
Ans : The number of devices that can be connected to an I2C bus depends on the available address space.
In standard mode, there are 128 possible 7-bit addresses, while in fast mode, there are 2048 possible 10-bit addresses.

```
```
What is the difference between I2C standard mode and fast mode?
Ans : I2C standard mode operates at a maximum frequency of 100 kHz, while fast mode operates at a maximum
frequency of 400 kHz. Fast mode allows for faster data transfer rates but requires stronger pull-up resistors
due to the higher data rate.
```
# SPI protocol

![image](https://github.com/user-attachments/assets/c18d1b23-5fba-45dc-91e4-bef4a029a0d4)


# UART protocol
![image](https://github.com/user-attachments/assets/3fd66942-2905-487d-b0b4-435b64438c9d)

![image](https://github.com/user-attachments/assets/46243c57-c4db-4571-bbaf-fc7fe70a337f)

