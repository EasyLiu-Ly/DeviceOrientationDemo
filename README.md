# DeviceOrientationDemo

This is a Android studio project demo using three methods to calculate the Attitude of the Android device.

This demo including three methods:

1、 use the SensorManager's methods to calculate the Attitude by using the values of accelerometer and magnitude.

    float[] attitudeValues = new float[3];
    float[] R = new float[9];
    SensorManager.getRotationMatrix(R, null, mAccValues, mMagValues);
    SensorManager.getOrientation(R, attitudeValues);
  
2、use MadgwickAHRS algorithm

3、use MahonyAHRS algorithm

The following picture is the screenshot of the MainActivity,which display the attitude of the device using three different method.

![image](https://github.com/EasyLiu-Ly/DeviceOrientationDemo/blob/master/DeviceOrientationDemo/screenShot.png)
