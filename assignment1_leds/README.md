# Assignment 1: LEDS

## Starting out in ROBOTICS!

Hello new fellow roboticist.
This tutorial series of assignments will guide you through your way to becoming an awesome robotics engineer.

The assignments are all based on each other, so you should do them in order, to be able to complete them.
There will be no reference solution published, however I am sure one exists, whereas I have one.

As you have made it to assignment 1, I assume you have successfully completed the install process described in the README.md in the root folder.

## At the blink of an eye

Your first task will be to program an LED so that it blinks with a frequency of 1Hz.
The tasks main goal is to make you a bit familiar with the language python and the basics of the framework.

To be able to work with a robot we have to import a robot into python.

```python
from robots.alice import Robot
```

Now we can create a robot simply by instancing 'Robot'.

```python
robot = Robot()
```

We can now change the leds of the robot by simply calling the set_led method on the newly created robot.

```python
robot.set_led(0, True)
```

Woohoo, the LED turned on! Now you should try to turn of the led after it was on for 2 seconds.

Hint: there is a 'time' module in python which might has a handy method.

If you managed turn off the LED after a certain time, you now can finish to implement the task by repeatedly turning the LED on and of at the correct time.
Remember the LED should blink at a rate of 1Hz.

## Bonus

Write your code so that you have a variable called HZ = 1 at the top of your code, which can be easily tuned to any rate.

Check that you also support odd numbers like HZ = 1.0 / 3.0 or HZ = 3.141