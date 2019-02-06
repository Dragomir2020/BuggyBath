# Buggy Bath

### Video Link
[Buggy Bath Video](https://www.youtube.com/watch?v=dpkyupwqfvU&t)

**INTRODUCTION**

The Buggy Bath is a fully automated car wash that uses the latest technology to get cars perfectly clean. It combines sensors that monitor the car&#39;s progress through each phase of the car wash, and motors that run water pumps and fans. Different levels of wash are available, Basic, Advanced, and Supreme, which correspond to the level of water and soap used. A seven segment display will show the user what type of wash they have selected. The system is completely automated and will step the user through the process along the way. The Buggy Bath will be a low maintenance cash flow that will surely pay off.

**USER MANUAL**

1. Drive car up to car wash

Pay attention to the stoplight during the entire duration of the wash. This will tell you when to drive forward, when to stop, and when to slowly drive through certain parts of the wash.

At the beginning, the stoplight will be a green light while the car wash waits for you to select your wash type and pull up to the start line.

1. Push button to select wash type

There are three different levels of wash: Basic, Advanced and Supreme, which have different water and soap levels to handle cars of varying levels of cleanliness.

In order to choose a wash type, use the pushbutton to cycle through the options. One push gives a Basic wash, two pushes for Advanced wash, and three for Supreme wash. Once a wash type is chosen it will be displayed on the screen for the user to confirm. A &quot;B&quot; will show for a Basic wash, an &quot;A&quot; for Advanced wash, and &quot;S&quot; for Supreme wash.

1. Drive Car into bay until light turns from green to red

Pull your car all the way to the start line, and the light changes from green to red indicating that you need to stop your car. The car wash has begun and you need to stop and wait for your car to be soaped up.

1. Put your car in park, while the system is washing your car

This is to ensure that you remain in the same place while the soap is applied and the brushes clean your car. Moving around may cause the machines to wash the same place twice as they rotate through the cleaning cycle.

1. When it is done the light will turn yellow

The yellow light means that the cleaning process is complete and it is time to begin the drying process.

1. Drive car out of bay slowly past drying fan

The yellow light means that you need to drive slowly out of the car wash bay to maximize drying time in front of the fan. Once you reach the exit of the bay you may proceed at a normal speed.

**DESIGN DESCRIPTION**

![Design Diagram](./imgs/imp)diagram.png)

The Buggy Bath will be implemented on a small scale in a waterproof clear container. The container will have a grate and water in the bottom. A pump will be used to pump water onto the toy car and to rinse after washing. The motor will be used to spin strips of fabric to clean the car. The system will have feedback in the form of leds and a seven segment display. The location of the car will be tracked with light sensors. Finally, when the car wash is done the yellow led will be lit telling the user to drive slowly out and past the fans.

**TEST PLAN**

**Tests for start sensor and selecting wash type:**

The start sensor is a phototransistor sensor that will be tested by checking if the sensor recognizes changes in light values. A toy car will be rolled up to the sensor and the light value will be recorded. If the light value is in the predetermined threshold for an object in front of the sensor, then the start sensor is working correctly.

Once the light sensor itself is working correctly, we will test if the sensor is starting the rest of the car wash program once a car arrives. This will be done by checking the next step, which is selecting the type of wash desired. A push button will be used to select the wash type, with one push for Basic wash, two pushes for Advanced wash, and three pushes for Supreme wash. Once the user selects a wash type, the first letter of the wash will be displayed on the 7 segment display (i.e. B, A or S). If the user is able to select which kind of wash they want and it is displayed on the 7 segment display, then the start sensor is correctly starting the car wash.

Both of these elements were tested and working correctly. We tested the light sensor in a variety of different light conditions to ensure that it worked in any lighting, and the program successfully calibrated itself to adjust for background lighting levels. The 7 segment display was able to be set to B, A or S, and the wash length of the corresponding cycle was timed to ensure the program ran the correct cycle.

**Tests for water pump:**

The water pump needs to be tested to ensure that the water stream is aimed at the car. This will involved placing the car in the car wash bay at the location where the cleaning stage will happen, and adjusting the water hose until the car gets adequately coated in the water-soap mixture. This will involve some trial and error of manually moving the hose.

After testing and some adjustment, the water pump was successfully aimed at the car. One issue we ran into was the hose getting hit by the spinning brush, so we had to reattach it higher in the ceiling to ensure it was away from moving parts.

**Tests for foaming brush:**

The brush will be tested to make sure the servo motor is moving when the start sensor tells the carwash to start. The first test will be with just the motor connected to the board, no brush attached yet, to make sure that the motor is moving as expected. Once that test has passed the brushes will be attached and they will be tested to make sure they are brushing the entire car.

The motor ran successfully the first time we connected it to the board, so we proceeded to making the brush and attached it to the motor. A car was placed inside the car wash with the motor and brush running, and the brush successfully cleaned the car.

**Tests for fan:**

The fan will turn on once the car is done with the brushing. The stoplight will show a yellow light, which tells the user to slow down to maximize drying time. The yellow LED illuminating will trigger the fan to turn on.

The fan was tested with varied voltage and current values until we found a fan speed that was appropriate for this project. We had to choose a speed that was fast enough to dry the car but slow enough that it didn&#39;t make the whole car wash shake.

**Tests for LED stop light:**

The LED needs to change during the car wash when the car reaches certain points in the bay, so it needs to be tested to ensure that the light changes at the correct location. This includes testing the LED once the car pulls up to the start line in the bay, making sure the light changes from green to red. The LEDs need to be tested in operation with the wash cycle timing, to ensure that the LED switches to yellow as soon as the wash cycle is done.

The LED was tested and it was working correctly. The light successfully changed colors when the driver was supposed to stop, slow down, or proceed forward.

**Parts List and Budget Info**

The following are needed to construct the Buggy Bath car wash.

- PBasic Homework Board
  - Included in kit purchased for class
- Relay x 3
  - 1 included in kit purchased for class, other two were borrowed from classmates
- Fan x 1
  - Pulled from an old pc owned by Ann, $0
- Pump x 1
  - Bought from Amazon, $8.99
- Green LED x 1
  - Included in kit purchased for class
- Red LED x 1
  - Included in kit purchased for class
- Yellow LED x 1
  - Included in kit purchased for class
- Servo Motor x 1
  - Included in kit purchased for class
- Cloth x 1
  - Cut up from an old rag, $0
- Push Button x 1
  - Included in kit purchased for class
- Light Sensor x 1
  - Included in kit purchased for class
- Seven Segment x 1
  - Included in kit purchased for class
- Plastic Container x 1
  - Bought from Target, $1.99
- Toy Car x 1
  - Already owned by Ann, $0
- 1m Pump Hose x 1
  - Came with pump, $0
- Grate x 1

Total project cost: $10.98

**Timeline**

Figure 10 shows the timeline of the project in the form of a Gantt Chart. Week 1 was the week of 10/14, and week 8 was the week of 12/2.

**Design Alternatives**

Some alternative design decisions that were made included different features of the car wash that we considered adding. We wanted to add more functionality to car wash and make it more elaborate, but unfortunately many ideas had to be removed to make the project more realistic. Budget and power supply was a deciding factor in many ideas.

Part of the original design that we eventually changed was having a separate dispenser for the soap and water. We had thought that this would be more effective at removing dirt from the car, since the car would have double the cleaning time. However the addition of more components requires more power, and we decided that for the scale of this project it would not be feasible to run pumps for both the soap and water. It was then decided that instead of pre-rinsing the car with water then spraying it with soap that these two steps would be combined, and the car will be sprayed with a soapy water mixture.



**Bugs/Issues and Remedies**

A major issue with this car wash was the concern of water damage/electrocution. Mixing electricity and water always has potential for dangerous outcomes, so we had to change a few parts of our final design in the name of safety. The LED stoplight, push button, and 7 segment display all had to remain on the breadboard mounted on the roof of the car wash because these components are not waterproof. In a real car wash these control would be inside the actual car wash so the user could interact with them, but this was not feasible for our project.

At first the light sensor was in backwards and the program was not able to get an average at the beginning, but this was simply remedied by flipping it around. The program had minimal bugs since most of the components were already used in class and the program is very straightforward. One interesting problem to solve with the code was looping around when the button is pressed. This was accomplished by using a modulo operator and if statements to capture the remainders. By incrementing a counter the wash type could be updated. Using this same method the control flow for the length of wash can be altered. Finally, to compensate for the number of pins. Only the segments on the seven segment that are altered were connected to pins. The other segments were attached to high to always be on.

