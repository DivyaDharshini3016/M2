# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int m,n,i;
    scanf("%d %d",&m,&n);
    for(i=m;i<=n;i++)
    {
        if(i%2==0)
        {
          printf("%d ",i);
        }
        
    }
    printf("\n");
    return 0;
}
```
## OUTPUT:

![Screenshot 2025-04-28 131646](https://github.com/user-attachments/assets/e90e3ad9-1962-4d8f-a1ea-32d4d41116cf)

## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int rows, i, j;
    scanf("%d", &rows);
    for (i = 1; i <= rows; i++)
 {
    for (j = 1; j <= i; j++)
      {
           printf("*");
        }
        printf("\n");
    }
   return 0;
}
```
## OUTPUT:
![Screenshot 2025-04-28 131933](https://github.com/user-attachments/assets/1db61fa3-d2c3-4773-bd3b-c34bd44041d6)

## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include <stdio.h>
void add(int a, int b);
void subtract(int a, int b);
int main()
{
    int num1, num2;    
    scanf("%d", &num1);
    scanf("%d", &num2);
    add(num1, num2);  
    subtract(num1, num2); 
    return 0;
}
void add(int a, int b)
 {
    int sum = a + b;
    printf("Addition: %d\n", sum);
}
void subtract(int a, int b)
 {
    int diff = a - b;
    printf("Subtraction: %d\n", diff);
}
```

## OUTPUT:
![Screenshot 2025-04-28 132036](https://github.com/user-attachments/assets/b775a289-ac8a-4a6c-8540-41a3eac661f8)

## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>
int main()
{
    int n, sum = 0;
    scanf("%d", &n);
    
    for (int i = 1; i <= n * 2; i += 2) 
    {
        printf("%d ", i);
        sum += i;
    }

    printf("\n%d\n", sum);
    
    return 0;
}
```
## OUTPUT:
![Screenshot 2025-06-02 113601](https://github.com/user-attachments/assets/aee63a4d-13c0-4876-a37e-8d25528c9ffb)

## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.

# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include<stdio.h>
void fact();
int main()
{ 
    fact();
}
void fact()
{
    int fact=1;
    int i,num;
    scanf("%d",&num);
    for(i=1;i<=num;i++)
    fact=fact*i;
    printf("Factorial value is: %d",fact);
}
```
## OUTPUT:
![Screenshot 2025-04-28 132301](https://github.com/user-attachments/assets/4800ee48-c3bb-4033-a04b-061eebd776d7)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
