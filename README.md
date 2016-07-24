# DeviceOrientationDemo

This is a Android studio demo using three methods to calculate the Attitude of the Android device.

This demo including three methods:

1、 using the SensorManager's method to calculate the Attitude by using the values of accelerometer and gyroscope.

    float[] attitudeValues = new float[3];
    float[] R = new float[9];
    SensorManager.getRotationMatrix(R, null, mAccValues, mMagValues);
    SensorManager.getOrientation(R, attitudeValues);
  
2、using MadgwickAHRS

3、using MahonyAHRS

The following picture is the screenshot of the MainActivity,which display the attitude of the device using three different method.

![image](https://github.com/EasyLiu-Ly/DeviceOrientationDemo/blob/master/DeviceOrientationDemo/screenShot.png)
