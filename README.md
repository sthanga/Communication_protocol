# Communication_protocol
Interview Preparation - I2C, SPI, UART, CAN, ETHERNET, LAN, UDP, IPMI, DBUS, IPC etc
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

