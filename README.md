# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1: Start Program

Step2: Use from output import robot.

Step3: Choose the x,y,z - axis movement distance(meters).

Step4: Give ep_chassis.move to move straight.

Step5: Give time.sleep() for a break.

Step6: Give ep_chassis.drive_speed to have a circular movement.

Step7: End Program

## Program
```python
from robomaster import robot
import time
from robomaster import camera

if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

    ep_chassis.move(x=2.6, y=0, z=0, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=102,g=0,b=102,effect="on")

    ep_chassis.move(x=0.3, y=-0, z=75, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=153,effect="on")

    ep_chassis.move(x=1, y=0, z=0, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=87,b=34,effect="on")

    ep_chassis.move(x=0, y=-1.55, z=0, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=87,b=34,effect="on")

    ep_chassis.move(x=0, y=-0.2, z=60, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=167,g=255,b=235,effect="on")

    ep_chassis.move(x=1.28, y=0, z=0, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=167,g=255,b=235,effect="on")

    ep_chassis.move(x=0, y=0, z=45, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=102,g=0,b=0,effect="on")

     ep_chassis.move(x=1.1, y=0, z=0, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=102,g=0,b=0,effect="on")

    ep_chassis.move(x=0.5, y=0, z=95, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=153,effect="on")

    ep_chassis.move(x=1.9, y=0, z=0, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=153,effect="on")

    ep_chassis.move(x=0.3, y=0, z=85, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=0,b=102,effect="on")

    ep_chassis.move(x=0.5, y=0, z=0, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=0,b=102,effect="on")

    ep_chassis.move(x=0, y=0, z=0, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=102,g=204,b=153,effect="on")

    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()
```

## MobileRobot Movement Image:

![WhatsApp Image 2023-12-24 at 14 15 49_0dd32a51](https://github.com/Aadithya2201/mobilerobot-openloopcontrol/assets/145917810/9c833ac4-dc89-490d-adde-1ada3fc7acfb)


Insert image here

![WhatsApp Image 2023-12-29 at 4 54 37 PM](https://github.com/Henriprasath/mobilerobot-openloopcontrol/assets/144979077/4ddd1d55-3193-4006-a802-920c777e162d)



## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here
https://youtu.be/YsLccT8xdmI?si=mOlj3RxVYPPlloUJ
## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
