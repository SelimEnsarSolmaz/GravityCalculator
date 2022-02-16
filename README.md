# GravityCalculator
Modify the example program to compute the position of an object after falling for 10 seconds, outputting the position in meters.

**DESCRIPTION**

outputting the position in meters. The formula in Math notation is: x(t) = 0.5 × at 2 + vit + xi Variable Meaning Value a Acceleration (m/s 2 ) -9.81 t Time (s) 10 vi Initial velocity (m/s) 0 xi Initial position 0 Note: The correct value is -490.5 m. Java will output more digits after the decimal place, but that is unimportant.

**Original Code**

```
class GravityCalculator {
    public static void main(String[] arguments) {
        double gravity = -9.81; // Earth's gravity in m/s^2
        double initialVelocity = 0.0;
        double fallingTime = 10.0;
        double initialPosition = 0.0;
        double finalPosition = 0.0;
        System.out.println("The object's position after " + fallingTime + " seconds is " + finalPosition + " m.");
    }
}

```
This code will output


![image](https://user-images.githubusercontent.com/99800269/154255956-56ac7ba6-f5fa-43b3-9f6b-fc1aa86343e7.png)


**My modified code**
```
public class GravityCalculator {
    public static void main(String[] arguments) {
        double gravity = -9.81; // Earth's gravity in m/s^2
        double initialVelocity = 0.0;
        double fallingTime = 10.0;
        double initialPosition = 0.0;
        double x; /*finalPosition = 0.0;*/
        x=(0.5 * ( gravity * (fallingTime * fallingTime)) + (initialVelocity * fallingTime) + (initialPosition));
        System.out.println("The object's position after " + fallingTime + " seconds is " + x /*finalPosition + */  + " m.");
    }

}
```
**And this is the output of the formula**
(I include the unmodified codes as comments)

![image](https://user-images.githubusercontent.com/99800269/154256962-263a9ed5-deb7-4c33-8ba2-9e1f5fe48a82.png)


