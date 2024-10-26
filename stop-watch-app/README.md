# Stopwatch Application

A simple stopwatch application built with React that allows users to start, stop, and reset a timer. The stopwatch displays time in hours, minutes, seconds, and milliseconds. The application features a sleek, user-friendly interface with styled buttons and a display.

## Features

- **Start**: Begins timing and displays the elapsed time.
- **Stop**: Pauses the stopwatch while keeping the current elapsed time.
- **Reset**: Resets the stopwatch to 0.
- **Responsive Display**: Displays elapsed time in hours, minutes, seconds, and milliseconds.

## Code Overview

### Stopwatch Component

The `Stopwatch` component manages the timer and provides start, stop, and reset functionalities.

- **State and Refs**:
  - `isRunning`: Tracks whether the stopwatch is running.
  - `elapsedTime`: Stores the elapsed time in milliseconds.
  - `intervalIdRef`: Stores the interval ID to allow clearing the timer.
  - `startTimeRef`: Tracks the time when the stopwatch started or resumed.

- **Functions**:
  - `start`: Sets `isRunning` to `true`, calculates elapsed time based on current time and previously elapsed time, and begins a timer interval.
  - `stop`: Pauses the stopwatch by clearing the interval and setting `isRunning` to `false`.
  - `reset`: Resets `elapsedTime` to `0` and stops the stopwatch.
  - `formatTime`: Formats the elapsed time into hours, minutes, seconds, and milliseconds for display.

  
## How to Use

1. Click **Start** to begin the stopwatch.
2. Click **Stop** to pause the stopwatch.
3. Click **Reset** to reset the stopwatch to zero.

