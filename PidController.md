# About PID Controller

For small low torque motors with little or no gearing, one procedure you can use to get a good baseline tune is to probe its response to a disturbance.
For tuning a PID the following steps can be used:
- 1- Set all gains to zero.
- 2- Increase the P gain unit the response to a disturbance is steady oscillation.
- 3- Increase the D gain unit the oscillation go away 
- 4- Repeat step 2 and 3 until increasing the D gain does not stop all oscillation.
- 5- Set p and D to the last stable values.
- 6- Increase the I gain until it brings you to the setpoint with the number of oscillation desired. 

## PID
  Proportional, Integral, Derivation feedback loop
  
## Gain
 Amount of output given from each of the components of PID

## Feedforward
A known value supplied to the output as a guesstimate so the PID only has to make minor correction.


* PID controll lies at the heart of any advanced robotics motion.
* Essentially, it is a way of controlling something, i.e. a wheel or an arm, using information gathered by the surroundings, in robotics, data is usually gathered through sensors, like encoders, range sensors, light sensors, etc.
* 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI4MDQ2MDc4OF19
-->