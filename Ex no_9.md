# EX 9 C program to find the sum of odd digits using do while loop.
## AIM:
To write a C program to find the sum of odd digits using do while loop.

## Algorithm
1. Start the program.

2. Initialize a variable to store the sum of odd digits (e.g., sum = 0).

3. Input the number from the user (e.g., num).

4. Set a loop to iterate through each digit of the number:

5. Use the do-while loop to extract the last digit of the number.

6. Check if the extracted digit is odd:

7. If it is odd (i.e., digit % 2 != 0), add it to the sum.

8. Remove the last digit from the number (i.e., num = num / 10).

9. Repeat the loop until the number becomes zero.

10. Display the sum of the odd digits.

11. End the program.

## Program:
```c
#include <stdio.h>
 int main()
 {
   int num, digit, sum = 0;
  scanf("%d", &num);
  if (num < 0) {
   num = -num;
  }
 do
 {
   digit = num % 10;
        if (digit % 2 != 0) {
          sum += digit;
 }
  num = num / 10;
     }
while (num != 0);
  printf("Sum of odd digits is: %d\n", sum);
   return 0;
 }
```

## Output:
![image](https://github.com/user-attachments/assets/d316844d-a96d-4ca7-a21c-7d34fc7a9848)

## Result:
Thus the program was executed and the output was verified successfully.
