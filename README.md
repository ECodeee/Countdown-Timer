"""
# Countdown Timer

## Description
This program implements a simple countdown timer in Python. The user provides a number of seconds, and the program counts down from that number to zero, printing each number with a short delay.

## How It Works
1. The user inputs the number of seconds for the countdown.
2. The program prints each second, decrementing the value until it reaches zero.
3. A short delay (0.1 seconds) is added between prints to simulate a real-time countdown.

## Usage
To run the script, execute it in a Python environment and enter the desired countdown duration when prompted:
```sh
python countdown_timer.py
```
Then, enter the number of seconds you want the countdown to last.

## Example Output
```
Enter the countdown time in seconds: 3
3
2
1
0
```
"""

import time  # Import the time module to use the sleep function

def countdown_timer(seconds):
    """
    Function to perform a countdown from a given number of seconds to 0.
    Each number is printed with a small delay.
    """
    for i in range(seconds, -1, -1):  # Loop from the given number down to 0
        print(i)  # Print the current countdown number
        time.sleep(0.1)  # Pause execution for 0.1 seconds to simulate a countdown
    
# Example usage
seconds = int(input("Enter the countdown time in seconds: "))  # Take user input
countdown_timer(seconds)  # Call the countdown function with the input value
