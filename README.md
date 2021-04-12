# The Automated Diagnostic Tool built on Arduino-enhanced joint evaluation algorithm
The Automated Diagnostic Tool built on Arduino-enhanced joint evaluation algorithm


## Materials List
*	Arduino UNO, MEGA Imported acrylic board (ARD050902)
*	axis tilt sensor equipped with gyro, acceleration, and geomagnetic sensors
*	Knee protector (brace) (Neoprene Sports)
*	9V E Type Bexel Batteries
*	Arduino compatible Wi-Fi development board
*	Arduino Uno IoT Board Compatible WIFI board (SZH-EK080)
*	Arduino GPS receiving module (SMG)
*	Elbow guard (Bodyon)
*	Calf belt compression band (Bodyon)
*	Eco-friendly soldering paste (EXSO)
*	Digital pocket tester (HIOKI)
*	Compression wrist strap
*	9V D Type Battery Cell (BEXEL)
*	Clear acrylic case for Arduino Uno
*	9V L Holder DC Connector Type (SZH-BH006)
*	Test Socket Jumper Cables

## Experimental Procedure

### Arduino Design and Manufacturing
After purchasing the materials, we took the following steps to build an Arduino-powered device.

* We glue-gunned Wemos D1 Mini to two MPU9250 on the top of the knee protector
* We glue-gunned D1 Mini and MPUS 9250.
* We uploaded the code (code porting) and supplied power to Wemos D1 Mini via a USB cable.

### Software Algorithm
1. Serial communication check 
2. Initializing the MPU9250 
3. MPU9250 initial calibration 
4. polling loop start 
  *	Set the flag, after completing the angle calculation of mpu9250 
  *	If both flags are set
    *	 Calculate the angle difference
    *	Serial output (angle difference, upper IMU angle, lower IMU angle) 
    *	Clear all 2 flags
  *	Back to polling loop start


#### Flow chart
![image](https://user-images.githubusercontent.com/82205054/114388246-67161200-9bce-11eb-892d-0df51add76db.png)


### Data Analysis
![image](https://user-images.githubusercontent.com/82205054/114388329-81e88680-9bce-11eb-9576-d86fb224eeb2.png)

![image](https://user-images.githubusercontent.com/82205054/114388386-9462c000-9bce-11eb-94ff-74f81f06020a.png)

![image](https://user-images.githubusercontent.com/82205054/114388400-97f64700-9bce-11eb-8d86-1bbafd7ae59f.png)


