# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)

```
## Output
### 1. Generic Articulated Robot
![280907503-cf2f46f2-23f8-4d78-912a-96adcb9113e6](https://github.com/Harish2404lll/Movement-of-Robot-Joints/assets/141472096/ed4c9483-1b67-4c5f-a600-940f154f6948)


### 2. robot.driveJoints(0,0,0,0,0,0)
![280907540-47210e6b-5d70-4f04-bb4f-9b2f60b24e47](https://github.com/Harish2404lll/Movement-of-Robot-Joints/assets/141472096/32d39751-2f59-484e-8815-1761c7bc1c31)


### 3. Movement of Joint1
![280907559-77289b1c-0e76-4d84-ac1d-0154ed3c2a9d](https://github.com/Harish2404lll/Movement-of-Robot-Joints/assets/141472096/422d828e-919a-447f-9870-526c63b3ac67)


### 3. Movement of Joint2
![280907585-810a803b-7872-4cef-853f-78503e03b9ec](https://github.com/Harish2404lll/Movement-of-Robot-Joints/assets/141472096/2704b59a-209e-46db-9cb9-efece80d8eae)


### 3. Movement of Joint3
![280907633-31e2b94c-7f96-4fae-add0-0bc40559bb07](https://github.com/Harish2404lll/Movement-of-Robot-Joints/assets/141472096/6c8a1af9-ace0-47ff-825c-9e6a9843dcfc)



## Result 
Thus the different robots joints are moved with the help of python list.


