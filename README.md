# Name:Manimaran V
# Reg.no:212224220060
# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
include <stdio.h>
#include <math.h>
void calculateEMI(float principal, float rate, int months)
{
float emi, amt, r, t;
r = rate / (12 * 100);
t = months;
emi = (principal * r * pow(1 + r, t)) / (pow(1 + r, t) - 1);
printf("The EMI for the loan is: %.2f\n", emi);
}
int main()
{
float principal, rate;
int months;
printf("Enter the principal amount: ");
scanf("%f", &principal);
printf("Enter the rate of interest (annual percentage): ");
scanf("%f", &rate);
printf("Enter the number of months: ");
scanf("%d", &months);
calculateEMI(principal, rate, months);
return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/5a0865a1-8ff7-4500-bdc2-1196d1961970)




## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
int n = 6;
int first = 0, second = 1, next, i;
printf("Fibonacci series for %d terms: \n", n);
printf("%d %d ", first, second);
for (i = 3; i <= n; i++)
{
next = first + second;
printf("%d ", next);
first = second;
second = next;
}
printf("\n");
return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/ae71323f-5977-4e0d-8ac1-dfd00bfb04e6)
![image](https://github.com/user-attachments/assets/cd3b8190-d3db-4820-8571-fdfdb40c2cf1)







## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
int n, i;
printf("Enter the number of elements: ");
scanf("%d", &n);
int arr[n];
printf("Enter %d elements:\n", n);
for (i = 0; i < n; i++)
{
scanf("%d", &arr[i]);
}
printf("The last element is: %d\n", arr[n - 1]);
return 0;
}
```
## OUTPUT


![image](https://github.com/user-attachments/assets/0828de3a-df69-45b3-a650-467463cb2736)







## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
int n, count = 0;
printf("Enter the number of elements: ");
scanf("%d", &n);
int arr[n];
printf("Enter %d elements:\n", n);
for (int i = 0; i < n; i++) {
scanf("%d", &arr[i]);
}
for (int i = 0; i < n; i++) {
if (arr[i] > 0) {
count++;}
}
printf("Total number of positive elements: %d\n", count);
return 0;
}
```

## OUTPUT


![image](https://github.com/user-attachments/assets/4e9ca598-035c-4f7c-9576-4dfbe592e460)



## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>
int main() {
Thus, the program to replace all even elements with 'E' in one dimensional array was
verified successfully.
int n;
printf("Enter the number of elements in the array: ");
scanf("%d", &n);
int arr[n];
printf("Enter the elements of the array:\n");
for (int i = 0; i < n; i++) {
scanf("%d", &arr[i]);
}
for (int i = 0; i < n; i++) {
if (arr[i] % 2 == 0) {
arr[i] = 'E';
}
}
printf("Updated array:\n");
for (int i = 0; i < n; i++) {
if (arr[i] == 'E') {
printf("'E' ");
} else {
printf("%d ", arr[i]);
}
}
printf("\n");
return 0;
}
```
## Output:
 
![image](https://github.com/user-attachments/assets/b75d0f33-9b50-462e-ae9b-4b11c164e8fb)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



