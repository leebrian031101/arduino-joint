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
![image](https://user-images.githubusercontent.com/82205054/114650238-d863db00-9d1c-11eb-8aa9-b7c690da7ee0.png)

![image](https://user-images.githubusercontent.com/82205054/114650252-e0237f80-9d1c-11eb-88ee-63affb42b6c1.png)


![image](https://user-images.githubusercontent.com/82205054/114388400-97f64700-9bce-11eb-8d86-1bbafd7ae59f.png)


![image](https://user-images.githubusercontent.com/82205054/114723937-0cb7b580-9d76-11eb-9e0d-cbf2d139460c.png)

![image](https://user-images.githubusercontent.com/82205054/114724077-2bb64780-9d76-11eb-8d45-6d7346673965.png)

![image](https://user-images.githubusercontent.com/82205054/114724125-3670dc80-9d76-11eb-8b1a-02c0d0fe376c.png)


![image](https://user-images.githubusercontent.com/82205054/114724179-44266200-9d76-11eb-954b-9ae1fe670512.png)

![image](https://user-images.githubusercontent.com/82205054/114724203-4983ac80-9d76-11eb-9e6b-2aa72d53d50c.png)

![image](https://user-images.githubusercontent.com/82205054/114724228-4dafca00-9d76-11eb-9c2f-4f54b90692ab.png)



