# Interface-a-PIR-sensor-with-an-STM32-Disco-boardrd

                                            /***** A basic example functionning a Passive Infrared Sensor "PIR"  *******/ 
                                             ***************************************************************************

                                               -*- This project was build using STM32CubeIDE with HAL librairies -*-

           
The PIR sensor is a passive Infrared sensor that detects the Infrared radiations ( as its name indicates). When a motion is detected the sensor sends a high signal (1)
from its OUT pin, the high state will persist around 5 seconds and then turn to the low state.

The STM32 will detect these High level with its IN Pin and turns the blue LED (PB15) ON for seconds.

The state of the LED will be indicated on the terminal, when its is ON ( Motion detected ) when it is OFF ( No Motion detected ). 

---- All you have to do is to create your project, activate UART2, make PB15 in output mode and PB5 in the INPUT mode, the generate your code and copy the 
                                                        content of the main attached                                                                  ----





         /*************** Interface PIR sensor and the STM32 board *********************/
 

                          PIR SENSOR    ||    STM32WL
                       ---------------------------------------
                              VCC               3.3V
                              GND               GND 
                              OUT               IN (PB5)
                      -----------------------------------------
