# IC-555-based-stepper-motor-controller
![maxresdefault](https://user-images.githubusercontent.com/19898602/123272521-71824f80-d51f-11eb-9317-3a77263ba1ee.jpg)

Hello friends this time I have developed a IC 555 based controller to control stepper motor
This controller can control speed as well as direction of stepper motor.
This small PCB based controller is very handy to test A4988 stepper driver IC and Stepper motors.
The main plus point of this controller is it does not required any coding.
Those of you have worked with stepper motor at any point of time 
they must know it is too much pain to run a stepper motor
Traditionally we need a microcontroller then we need a stepper driver IC then we need to write code to run stepper motor then we need to upload that code to our microcontroller.
All after this, we are able to run or stepper motor.
Suppose you just need to check your stepper motor or A4988 stepper driver or you need to 
run stepper motor for any simple application you have to go through traditional way
However, by using this controller simple just connect stepper motor wires and connect power supply to PCB 
that is it you are ready to go.
The PCB controller which I have used in this project is orderd from [JLCPCB.com](https://jlcpcb.com/IAT)
Further in this post we will learn in depth about how this controller work 


# VIDEO

[![](https://img.youtube.com/vi/RE0nTC17tEM/0.jpg)](https://www.youtube.com/watch?v=RE0nTC17tEM)

I also have a full video on this project on my youtube channel youu can watch the full video 
you will get most of the idea by watching this video 
to watch video juct click on above image

# HOW STEPPER MOTOR WORKS
Before going further first we need to know how actually stepper motor works.
stepper motors are very much different and complex from traditional DC motors
Stepper motor runs in steps as name suggest.
Basically stepper motors are brushless DC motors, normally a permanent magnet rotor placed in between of stator winding.

Stator winding then energize step by step in a sequential way so it get magnetize and force rotor to align with the magnetic field of stator coil.

in this way rotor begin rotate in small steps, due to this behavior the motor gets its name “stepper motor”

As we can see now by controlling the stator winding generations sequence we can precisely control the position of rotor without any position feedback system.

this quality of stepper motor makes is best suitable to be used were high precision motion is required like CNC machines.

![STEPPER-2](https://user-images.githubusercontent.com/19898602/123275483-fa9a8600-d521-11eb-8d4e-fa7ab2ac37de.gif)

Also here we have to note another best quality of stepper motor is High torque at low RPM & Holding torque.

We know that rotor of stepper motor rotates by sequentially energising stator coils.

if we energize a single set of coil with time delay respectively we get slower RPM of stepper motor.

hence we also get high torque because rotor is always in hold within the magnetic field of energized stator coils.

If we keep energize a single set of stator coil the rotor will be stay on its place with maximum torque.

# Driving methods

Single coil excitation mode
There are many methods to drive stepper motor.
how stepper motor works with single coil excitation is basic method to drive stepper motor.
![SINGLE-STEP-1536x771](https://user-images.githubusercontent.com/19898602/123275974-67ae1b80-d522-11eb-8efc-6cf1cc30470b.jpg)



Full step Mode
In full step drive mode 2 coils are excited at same time because of this it provide higher torque to the motor.
![full-step-1024x493](https://user-images.githubusercontent.com/19898602/123276037-7563a100-d522-11eb-945f-90ae72e65d9b.jpg)



Micro-stepping mode
Micro stepping mode is the now most famous way to control stepper motor, high precision can achieve by this drive mode.
Micro stepping mode give smooth and silent motion to stepper motor by providing variable controlled current to the coil in form of sine wave.

![micro-1024x477](https://user-images.githubusercontent.com/19898602/123276086-7e547280-d522-11eb-838e-c9bfc83a6743.jpg)

 
 # STEPPER DRIVER IC
 Till now we learn how stepper motor works, now we will see what we need to run stepper motor
So we have a stepper driver IC which we known as A4988 there are many other stepper driver IC
more or less all are work on same principle.

![0J10073 600](https://user-images.githubusercontent.com/19898602/123278053-40584e00-d524-11eb-86e1-c1bd8f9c2c21.jpg)

 

