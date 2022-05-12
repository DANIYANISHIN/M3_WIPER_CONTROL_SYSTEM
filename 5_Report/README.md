# WIPER CONTROL SYSTEM

Wiper is an essential component that used to wipe raindrops or any water from the vehicle’s windscreen.
The previous system was used to activate the wiper manually and the process of pulling up the wiper is difficult to be handled. 
Thus, this system is proposed to solve these problems. 
The objectives of this project are to upgrade the older cars system by providing automatic wiping system, to improve the system by using sensor with actuator and to design a basic program that will fully operate with the system.
The concept of this proposed wiper system is similar with other existing conventional wiper.
In this project we are trying to simulate the wiper control system  on software.

# WORKING PROCESS
* The RED LED is considered for the ACC position. Once the push button is pressed for 2 seconds, the RED LED keeps continuously glowing until the stop of the engine signifying the engine condition to be turned ON.
* On press of the user input push button, the other three Blue, Green and Orange LEDs come ON one at a time with the set frequency. The frequency changes on every alternate key press, 3 frequency levels with 1, 4 and 8 Hz.
* The LED glow pattern stops on the 4th press; the wiper action starts with the next press.
* If the push button is pressed for 2 seconds continuously, the RED light goes off and the pattern stops bringing it to default position which signifies the engine is turned OFF.

# SWOT ANALYSIS
## Strength

* The wiper comes back to default position even if stooped in the middle
* Safety for the driver as well as the passengers in the vehicle
* Clear Visibility to the Driver for neat ride.

## Weakness 
* The total cost of the wiper system is high if implemented in real-time.
* The major disadvantage is that STM32 contains only one button for all the operation
* User has to undergo a sequence to acquire desired result and can't attain his result directly with the press of the button.

## Opportunities
* Rain sensing and automatic operation can be implemented as further enhancement.

## Threats 
* Replacing the board is not possible if it malfunctions.
* Can't have more functions as the functionality of the board is very basic.

# 5WS AND 1H
## WHAT
It is Wiper Control system which is generally deployed in all the automobiles in order to ensure safety for the passengers and drivers during rainy conditions.

## WHERE
It is an element which is present in the windshield of the automobile.

## WHO
It is highly useful for drivers of any kind of automobile who needs clear vision of the road in case of dust or rain.

## WHEN
It is recommended to operate during dust or rain

## WHY
To get a clear vision of the road.

## HOW
It is implemented with the help of STM32 with the desired operation of turning on the engine, changing of speeds and turning off with the help of Embedded c Programming.

# REQUIREMENTS
## High level requirements
| ID | Description | Status |
| --- | --- | --- | 
| HR_01 | ACC Mode Operation |	Implemented |
| HR_02 |	Wiper ON |	Implemented |
| HR_03 |	Wiper Speed Change |	Implemented |
| HR_04 |	Wiper OFF |	Implemented |
## Low level requirements
| ID |	Description | Operation |	Status |
| --- | --- | --- | --- |
| LR_01 |	Button pressed once for 2 secs | Red LED ON |	Implemented |
| LR_02 |	Button pressed second time | 1 Hz speed - Blue, Green Orange alternative |	Implemented |
| LR_03	|Button pressed third time | 4 Hz speed - Blue, Green Orange alternative |	Implemented |
| LR_04	|Button pressed fourth time | 8 Hz speed - Blue, Green Orange alternative |	Implemented |
| LR_05 |	Button pressed again for two seconds |Turn Off all LEDs |	Implemented |


# BEHAVIORAL DIAGRAM
![behavioral diagram wiper](https://user-images.githubusercontent.com/101271806/168133411-5ebd4cc9-c075-4901-ba3f-9d417d63b2f3.png)


# STRUCTURAL DIAGRAM
![structural diagram wiper](https://user-images.githubusercontent.com/101271806/168134079-0356ef4b-7d5f-4bf1-b160-da439a3d53da.png)

# TEST CASES 

## High Level Test Cases
| Test ID | Description | Exp.i/p | Exp.o/p | Actual o/p | STATUS |
| --------|:------------|:--------|:--------|:-----------|:-------------|
| 1 | check if the BUTTTON is pressed  | program execution | Microcontroller/Engine starts | LED ON(RED)| PASS |
| 2 | check if the BUTTTON is pressed  | program execution | WIPER starts | LED ON(BLUE)| PASS |
| 3 | check if the BUTTTON is pressed  | program execution | WIPER starts | LED ON(GREEN)| PASS |
| 4 | check if the BUTTTON is pressed  | program execution | WIPER starts | LED ON(ORANGE)| PASS |
| 5 | check if the BUTTTON is pressed  | - | Microcontroller/Engine stops | LED TURNED OFF| PASS |









## Low Level Test Cases
| Test ID | Description | Exp.i/p | Exp.o/p | Actual o/p | STATUS |
| --------|:------------|:--------|:--------|:-----------|:-------------|
| 1 | check if the BUTTTON is pressed  | program execution | Microcontroller/Engine starts | LED ON(RED)| PASS |
| 2 | check if the BUTTTON is pressed again | program execution | WIPER starts and speed of wiper is slow | LED ON(BLUE)| PASS |
| 3 | check if the BUTTTON is pressed again | program execution | WIPER starts and speed of wiper is moderate | LED ON(GREEN)| PASS |
| 4 | check if the BUTTTON is pressed again | program execution | WIPER starts and speed of wiper is good | LED ON(ORANGE)| PASS |
| 5 | check if the BUTTTON is pressed again | - | Microcontroller/Engine stops | LED TURNED OFF| PASS |







