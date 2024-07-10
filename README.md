# Powder-despenser

These are the CAD files and explanation for powder despenser with precision and accuracy.

## Components Used

- 360 servo motors.
- Linear actuators.
- Weighing machine
- 3D printed / Fabricated custom parts.

## Working
The images below are the various parts of full working machine.

![image](https://github.com/Bhajneet-Singh-Bedi/Powder-despenser/assets/92092790/3a3a2756-7d2f-4251-abe4-269484c057f9)

### Weighing machine
![image](https://github.com/Bhajneet-Singh-Bedi/Powder-despenser/assets/92092790/0df238d4-6e52-4859-98d2-8c4ac29922ad)

### Dispensing Cone
![image](https://github.com/Bhajneet-Singh-Bedi/Powder-despenser/assets/92092790/c6ae1625-3aaf-4706-ab59-c626ec346a3f)

### Chamber Assembly
![image](https://github.com/Bhajneet-Singh-Bedi/Powder-despenser/assets/92092790/90fb550f-7a22-4fe1-b22b-8555b7ede501)

### Chamber Base
![image](https://github.com/Bhajneet-Singh-Bedi/Powder-despenser/assets/92092790/d36448cc-7d3d-4586-b9b6-3d013caaf7a8)




## Explanation
Chamber assembly consists of two parts. The outer cone and inner cone. The outer cone holds vaiours kinds of powders and inner cone acts as a barrier stopping the powder to spill over.

#### Step-1
First the Chamber base rotates 90 degrees so that the base of chamber assembly aligns with the dispensing cone. This is done using 360 servo( yellow, chamber base)

#### Step-2
Then the linear actuator(green, chamber base) brings down the whole base down. 

#### Step-3 (Dispensing Step)
In this step the cube(red, dispensing cone) helps to lift the inner cone(pink, chamber assembly) which then lets the powder to fall on the weighing machine(blue) through a funnel.

![image](https://github.com/Bhajneet-Singh-Bedi/Powder-despenser/assets/92092790/1980c058-ff8f-424c-bbf2-15e49537c855)
![image](https://github.com/Bhajneet-Singh-Bedi/Powder-despenser/assets/92092790/8903f36c-0540-414c-9ff7-72f9e6b4ccb9)
The first image shows the inner cone holding the powder and second image shows the position of the inner cone when it is lifted with the help of the cube attached on dispensing cone which lets the powder to fall.

#### Step-4 (Weighing step)
The weight is calculated using the weighing machine which collects the powder. The value of weight is send to a microcontroller which uses PID controller and decides when to rise up the chamber base so that the inner cone goes down to the same resting position which stops the powder from flowing.

#### Step-5
After the required weight has been achieved, linear actuator pushes the base up.

#### Step-6
The 360 motor rotates to the required position (which powder to weight according to the chamber it is in) and then repeats the process.


## Appendix
- This system is very reliable as every time only a certain amount of powder is dropped through the mechanism. 
- It is also scalable and flexible as the number of chambers in the base can be increase or decrease according the choice of the operator. As seen in the picture currently it has 4 chambers, the number of chambers can be increase by changing the base or using a base with space for multiple chambers. Like below.
![image](https://github.com/Bhajneet-Singh-Bedi/Powder-despenser/assets/92092790/383298c6-a685-4fb6-a6da-07c67968e6cb)
- The operator will be provided with the interface in which
  - chambers are installed.
  - positions of chambers.
  - name of powder for ease of use.

- The program will automatically decide the rotation of the motor to target that specific powder according to the need of the operator.




