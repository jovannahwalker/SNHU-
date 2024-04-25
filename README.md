# SNHU-
# Extended Factorial Calculation Project

## Summarize the project and what problem it was solving:
This project calculates the factorial of a given number using a function in C++. Factorial is the product of all positive integers up to the given number. The extended version includes error handling for negative inputs and integer overflow cases, along with unit tests using the Catch2 testing framework for validation.

## What did you do particularly well?
I implemented error handling to gracefully handle negative inputs and integer overflow situations. The inclusion of unit tests using Catch2 ensures the correctness of the factorial calculation function under various scenarios.

## Where could you enhance your code? How would these improvements make your code more efficient, secure, and so on?
One improvement could be incorporating more comprehensive error messages in the error handling code. This would provide users with clearer feedback on why their input is invalid or why an overflow error occurred. Additionally, optimizing the factorial function for performance in handling large inputs could be explored.

## Which pieces of the code did you find most challenging to write, and how did you overcome this? What tools or resources are you adding to your support network?
Handling integer overflow cases was challenging, especially ensuring that the program detects and handles overflow appropriately without crashing. I studied integer limits and consulted documentation to understand how to detect and handle overflow conditions. Using the Catch2 testing framework for unit tests provided valuable feedback and validation during the development process.

## What skills from this project will be particularly transferable to other projects or course work?
The skills of implementing error handling, writing unit tests, and dealing with numeric constraints (such as integer overflow) are highly transferable. Understanding and addressing potential edge cases in program logic are crucial skills that can be applied to various programming tasks.

## How did you make this program maintainable, readable, and adaptable?
I used meaningful variable names, clear comments, and structured the code into functions with specific responsibilities. Error handling and input validation enhance the program's reliability and user experience. Unit tests provide a safety net for future changes or additions, ensuring that existing functionality remains intact.
