README:

Light-weight-task-scheduler

This is a solution to a problem of toggling two LEDS or GPIOs namely, LED1 and LED2 at 1 sec and 2 sec interval respectively.

This project provides two solutions:

A bare-metal approach, where the LED toggling is done using a simple while loop.
A scheduler approach, where the LED toggling is done using a simple scheduler.
The solutions were implemented and tested using a Cortex M series processor on the Wokwi Simulator platform. The simulation links for both the solutions are provided in the respective code sections.

The bare-metal approach is simple and straightforward, but it is not scalable when there is a need to toggle many LEDs with different intervals. To overcome this problem, a simple scheduler was implemented. The scheduler is a preemptive scheduler that executes the tasks based on their priority.

The scheduler approach provides a scalable solution for toggling multiple LEDs with different intervals. To add new tasks, you can create a new task function and add it to the task list in the scheduler. The scheduler will automatically execute the tasks in the order of their priority.

The code for both the solutions is provided in the respective code sections. The code is written in C and uses the Pico standard library and the hardware GPIO library.

To run the code on the Wokwi Simulator platform, create a new project and copy-paste the code. Run the simulation to see the LED toggling in action.
