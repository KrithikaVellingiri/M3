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
#include <stdio.h>
#include <math.h>
void calculateEMI(double principal, double rate, int months);
int main() {
    double principal, rate;
    int months;
    scanf("%lf", &principal);
    scanf("%lf", &rate);
    scanf("%d", &months);
    calculateEMI(principal, rate, months);
    return 0;
}
void calculateEMI(double principal, double rate, int months) {
    double r, emi;
    r = rate / (12 * 100);
    emi = (principal * r * pow(1 + r, months)) / (pow(1 + r, months) - 1);
    printf("EMI = %.2lf\n", emi);
}
```

## OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8b899ce3-b044-4528-9952-9145f5d72b2f" />





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
int main() {
    int n = 6; 
    int t1 = 0, t2 = 1, nextTerm, i;
    printf("Fibonacci series for %d terms: ", n);
    for (i = 1; i <= n; i++) {
        printf("%d ", t1);
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;
    }
    printf("\n");
    return 0;
}
```
## OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/92ed09fb-e3ae-4a63-9d55-e3d5e9a73cc2" />








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
int main() {
    int n, i;
    scanf("%d", &n);
    int arr[n]; 
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The last element is: %d\n", arr[n - 1]);
    return 0;
}
```
## OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2630e090-536e-4be7-850d-7b58cd9adb52" />









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
    int n, i, count = 0;
    scanf("%d", &n);
    int arr[n];
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements = %d\n", count);
    return 0;
}
```

## OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c1b180c9-b2c4-4774-96c2-c401666e4a4f" />





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
    int n, i;
    scanf("%d", &n);
    int arr[n];     
    char result[n]; 
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0) {
            result[i] = 'E';   
        } else {
            result[i] = arr[i] + '0'; 
        }
    }
    printf("Updated array: ");
    for(i = 0; i < n; i++) {
        printf("%c ", result[i]);
    }
    printf("\n");
    return 0;
}
```
## Output:
 <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ec3421e5-3367-4f4b-95ce-ccefb080f410" />



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



