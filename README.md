This stopwatch program is a simple timer that allows you to start, pause, and reset the timer. It displays time in the format hours : minutes : seconds : milliseconds and continuously updates every 10 milliseconds. Here’s a breakdown of its features and functionality:

Features
Start: Begins the timer, counting up from 00 : 00 : 00 : 000.
Pause: Stops the timer at the current time, allowing it to be resumed from the same point.
Reset: Stops the timer and resets the display to 00 : 00 : 00 : 000.
How It Works
Timer Initialization: The timer is initialized with hours, minutes, seconds, and milliseconds all set to 0. The display is formatted to show two digits for hours, minutes, seconds, and three digits for milliseconds.

Event Listeners:

The Start button sets an interval (setInterval) that calls the displayTimer function every 10 milliseconds.
The Pause button clears the interval, stopping the timer.
The Reset button clears the interval and resets the timer values back to zero.
Timer Update Logic:

Milliseconds increase by 10 on each interval.
When milliseconds reach 1000, they reset to 0, and seconds increase by 1.
When seconds reach 60, they reset to 0, and minutes increase by 1.
When minutes reach 60, they reset to 0, and hours increase by 1.
Display Formatting: The program formats each time unit (hours, minutes, seconds, milliseconds) with leading zeros to ensure consistent display, such as 01 : 02 : 03 : 004.

Example Usage
Pressing Start begins the stopwatch, displaying time from 00 : 00 : 00 : 000 and incrementing smoothly.
Pressing Pause will freeze the time display, allowing you to check the elapsed time.
Pressing Reset will clear the timer, setting it back to the initial 00 : 00 : 00 : 000 display.
