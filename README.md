# RF receiver
This project is an intermediate step between my drone automation project and the RF communication between it and remote.
This Arduino sketch uses Virtual Wire library to receive data through chanel 433MHz. Its goal is to decode received data in order to extract Yaw, Pitch, Roll and Throttle commands.
In a further step, these extracted commands will be used as flight instructions for the quadcopter.

Here what the whole looks like :
```
              |/_   ))))) RF 433MHz ))))    _\/
              /                               \
   +----------+                                +---------+
   | Arduino  |                                | Arduino |
   | receiver |                                | emitter |
   +----------+                                +---------+
```