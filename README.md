"""
Countdown Timer

This program takes a user-defined number of seconds as input and counts down to 0,
printing each number with a short delay.
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
