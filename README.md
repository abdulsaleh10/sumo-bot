# Sumobot

During my software engineering internship at GE Appliances, I participated in their exciting Sumobot competition. Alongside a team of three, we built a robot featuring a microcontroller, two wheels, IR sensors, and line sensors. We added a unique twist: a "scooper" rigged with hinges and a sharp metal plate. Although Sumobot rules typically restrict certain dimensions, they don't limit height. So, we designed our scooper to stay upright at the start and then drop during the match via a clever motor "jerk", giving us a competitive edge without breaking any rules. Our goal was to outmaneuver and push the opposing bot out of the ring. Through agile development, we tackled design challenges and coded our way to victory with Byte-Basher, our champion Sumobot.

Fight 1 | Fight 2
:-: | :-:
<video src=https://github.com/abdulsaleh10/sumo-bot/assets/89872422/b4cc05f0-5541-401b-babc-ea058e176f84 width=180/> | <video src=https://github.com/abdulsaleh10/sumo-bot/assets/89872422/96deccd4-f6ca-49b9-84d4-8a0bb020532b width=180/>

To design the algorithm for our robot's movements, we methodically set the pin connections on our microcontroller. We controlled the motor's speed using PWM signals sent via an analog pin, while directional control was handled by digital pins. Our sensor arrangement combined analog and digital signals. We used five infrared sensors to assess opponent proximity and change our robot's trajectory accordingly. We also included a line sensor, enabling our robot to track the perimeter of the battlefield and ensure that it remained within its boundaries. Our strategy, designed using state machines and timers written in embedded C, was programmed into the microcontroller using a Raspberry Pi.
