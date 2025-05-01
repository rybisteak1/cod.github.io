# Project: Self-Balancing Robot

### Pictures!

| ![1746063767191](image/README/1746063767191.png) | ![1746063788230](image/README/1746063788230.png) |
| ---------------------------------------------- | ---------------------------------------------- |
| ![1746063810835](image/README/1746063810835.png) | ![1746063830784](image/README/1746063830784.png) |

### SRS Validation

|                 | Description                                                                                                                                                                                                                                                                                                                                                                   | Met? |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---- |
| **SRS 1** | SRS1 was met. The IMU successfully read the gyroscope and accelerometer data, and as a peripheral, and sent the information via I2C to the MCU. This functionality can be tested using the logic analyzer, as the IMU I2C data can be probed using a breadboard. We also verified that the MCU is able to read and use the data by writing to a serial monitor using the MCU. | Yes! |
| **SRS 2** | SRS2 was met. We used a PID control algorithm to control the motors in a way that would hypothetically keep our robot stable. As anticipated, due to the difficulty of testing the algorithm until the final robot was assembled, we completed some functionality testing to see how the feedback loop responded to changes in IMU angle.                                     | Yes! |
| **SRS 3** | SRS3 was met. We used a motor controller to control the movements of 2 DC motors through outputting PWM signals from the MCU. We were able to test this functionality using our motortest.c file by configuring it to write different speeds to the DC motor and seeing how it responds.                                                                                      | Yes! |
| **SRS 4** | SRS4 was met. We configured a PID control loop which required us to use timers and interrupts, in addition to other calculations. The success of this implementation was tested by seeing if our feedback loop was able to spin the wheels properly according to the IMU input, which we verified successfully.                                                               | Yes! |

#### SRS # Validation

#### SRS # Validation

### HRS Validation

|                 | Description | Met? |
| --------------- | ----------- | ---- |
| **HRS 1** |             | Yes! |
| **HRS 2** |             | Yes! |
| **HRS 3** |             | Yes! |
| **HRS 4** |             | Yes! |
| **HRS 5** |             | Yes! |

#### HRS # Validation

#### HRS # Validation

### Conclusion/Reflection
