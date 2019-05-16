# Gimbal-Project
Karen Zhang
Gimbal
Mixed Media, 3D Printing

This project is a self-stabilizing gimbal by using Arduino Nano, MPU6050 sensor, and three servos that control ‘row’, ‘pitch’, and ‘yaw’. 

The MPU6050 IMU has both 3-Axis accelerometer(a vehicle's capacity to gain speed within a short time.) and 3-Axis gyroscope(a device consisting of a wheel or disk mounted so that it can spin rapidly about an axis which is itself free to alter in direction. ), so totally it is 6-Axis motion tracking device.

3 Parts of The Process
1.MPU6050 Arduino Code
In the beginning, the code initialized the wire.h library and set the sensor through the power management register. To do that, we need to look up the datasheet of the sensor to find the registered address and request to read all 6 registers for the X, Y and Z axes. The result is the printing values of this sensor on the serial monitor, and when I move the sensor the values changes.

2.3D Visualization
After reading the values on the serial monitor, we can send the data in Arduino to processing (software) through the serial port. After we run the sketch, we can see the 3D visualization of how the sensor working.

3. Putting Everything Together
I 3D printed the components of it and put them all together. I use three servos, and each of them controls the action of ‘row’, ‘pitch’, and ‘yaw’. I used a buck converter as well, to converts 7.4V voltage 5V voltage.


