# EmergingSysArch-Tech
CS-350 Emerging Sys Arch &amp; Tech at SNHU

MileStone 2 
Summarize the project and what problem it was solving.

In this Project, we had to use the UART module in our microcontroller to input one character at a time to take in the consecutive input of "ON" to turn on an LED and "OFF" to turn off an LED, and implement the code inside of a state machine.

What did you do particularly well?

This was my first time working with a state machine, so I decided to find out the code for the UART first and then figure out how to use the state machine. It did take me some time to figure out the code behind turning the LED on and off, but I didn't realize until after creating the state machine that I was making the process harder than it actually was. State machines are supposed to be designed to show movement from one state to another, so as long as the pathways are interpreted correctly, the development of the code should be easier. It was this project that made me realize the importance of planning out the state machine diagram early to help expedite the solving of a problem in my code.

Where could you improve?

After looking at the teacher's feedback, I realized that when inputting the characters for "ON" and "OFF," I had already changed them to ASCII to match the UART inputs. This was fine for this code; however, it made it non-portable. I should have also been more detailed when commenting on what my code does to clarify any misunderstanding of what certain numbers or variables represent. For example, I had that the path to turning the LED on was for the input to be 157, but I didn't explain that 157 was the combination of ('O' + 'N') = 157 in ASCII.

What tools and/or resources are you adding to your support network?

When working with embedded devices, I intend to use state machines more often, as I believe that they will make work much easier.

What skills from this project will be particularly transferable to other projects and/or course work?

Whether working with embedded systems or not, I realize that thorough planning out code before coding actually begins can make a project run exceptionally smoother. By developing diagrams for your anticipated code, you are showing you creating a strong layout for your code, which will make it easier to troubleshoot and debug your code if problems arise.

How did you make this project maintainable, readable, and adaptable?

Going back, I plan to make this project maintainable, readable, and adaptable by fixing the short-sighted mistake that I made by not making my code portable and by commenting out areas that I failed to comment on before to make sure other can completely understand the code and decision I made in the design.

Project One
Summarize the project and what problem it was solving.

For this project, we had to create a digital thermostat that read the temperature of a room, check to see if the temperature was above or below a set point that could be adjusted with the press of a button, and turn  a light on or off based on the comparison to represent a heater turning on and off, and output all of this to the screen using the UART on the microcontroller.

What did you do particularly well?

This project had a lot of moving parts; I started off by creating the state machines one at a time, first checking the buttons to change the setpoint, then the state machine to check the temperature, and lastly, the state machine to update the lights. Once I had my state machines, I worked on creating the Task Scheduler, which took some time to figure out at first, but ultimately went smoothly. 

Where could you improve?

When adding the temperature sensor and UART display function to the state machines, I quickly noticed that the code would freeze. After doing some research, I found that this was because the state machine had to wait for the sensor, which would cause it to crash. My solution to this was to create flags in the state machine that would trigger when the state machine went into a state, and when the state machine exited the state, I would take the opportunity to use those peripherals and reset the flags at the same time. Though this did help mem to solve the problem, I wasn't entirely sure if it was the correct/proper way to do so.

What tools and/or resources are you adding to your support network?

If and when I work with embedded systems in the future, I will make sure to definitely take advantage of the state machine and task schedulers to implement my code. I found that using the combination of these two tools made everything run pretty smoothly; it also made it easier to pinpoint problems when troubleshooting for errors.

What skills from this project will be particularly transferable to other projects and/or course work?

Working with embedded devices, in general, will be transferable to other projects, in school, and in the future. Embedded systems have become such an integral part of today's society that we see them everywhere we turn; I believe having the knowledge and knowing how to work on these systems will prove to be a valuable asset in the future.

How did you make this project maintainable, readable, and adaptable?

For this project, I made sure to follow coding best practices and comment out everything, discussing my reason for every bit of code that I created so that the code can be properly understood and maintained by anyone who may come after me. 
