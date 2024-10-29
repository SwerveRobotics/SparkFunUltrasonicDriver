# Header
This repository contains a driver for integrating the [SparkFun Ultrasonic Distance Sensor - TCT40 (Qwiic)](https://www.sparkfun.com/products/24805), an I2C device, into the FTC SDK. You may want to use this sensor because, as of 2024, the walls of the competition area are clear, and so a conventional laser distance sensor would not be able to detect the wall. 

# Installation:
## Step 1:
First, go to your `build.gradle` file and go to `repositories`. Add `maven { url "https://jitpack.io" }` as a repository. (If it's already there, don't do anything.)
```Java
repositories {
  // Your other stuff here...
  maven { url "https://jitpack.io" }
}
```

## Step 2:
Then, go to `dependencies` in the same `build.gradle` file. Add `com.github.SwerveRobotics:UltrasonicDistanceSensor:0.0.1` as a dependency.
```Java
dependencies {
  // Your other stuff here...
  implementation 'com.github.SwerveRobotics:UltrasonicDistanceSensor:0.0.1'
}
```

## Step 3:
Now, you may type `import org.swerverobotics.ftc.UltrasonicDistanceSensor` in one of your Java class files to import the driver!
