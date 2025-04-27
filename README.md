
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```
#include <stdio.h>

int main() {
    char ch1, ch2, ch3;

    printf("Enter first character: ");
    scanf(" %c", &ch1);

    printf("Enter second character: ");
    scanf(" %c", &ch2);

    printf("Enter third character: ");
    scanf(" %c", &ch3);


    printf("Characters in reverse order: %c %c %c\n", ch3, ch2, ch1);

    return 0;
}

```


## OUTPUT:
![reverse](https://github.com/user-attachments/assets/26824b45-fa57-4bef-80c4-f7a41cb6cff7)


















## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```
#include <stdio.h>

int main() {
    int A;

    // Reading the value of A
    printf("Enter a number: ");
    scanf("%d", &A);

    // Checking if A is positive
    if (A > 0) {
        printf("A is a positive number.\n");
    } else {
        printf("A is not a positive number.\n");
    }

    return 0;
}


```

# OUTPUT:
![positive](https://github.com/user-attachments/assets/72b883e2-3991-455d-8ed1-ec9b28617017)
![negative](https://github.com/user-attachments/assets/6b707766-b442-4c18-8298-ad1248e5da0c)


# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```
#include <stdio.h>

int main() {
    float num1, num2, min;

    // Reading two fractional numbers
    printf("Enter first fractional number: ");
    scanf("%f", &num1);

    printf("Enter second fractional number: ");
    scanf("%f", &num2);

    // Using ternary operator to find minimum
    min = (num1 < num2) ? num1 : num2;

    printf("The minimum number is: %.2f\n", min);

    return 0;
}
```

## OUTPUT:
![min](https://github.com/user-attachments/assets/9967ad30-14fb-4695-a456-8893051be3e2)



## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int value;

    // Reading the input value
    printf("Enter a number: ");
    scanf("%d", &value);

    // Checking if the value is equal to 1
    if (value == 1) {
        printf("The value is equal to 1.\n");
    }

    return 0;
}
```

## OUTPUT:
![equal to 1](https://github.com/user-attachments/assets/e01ab2e8-2cac-423c-a7c2-ac1a20f05c69)



## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
```
int main() {
    int m1,m2,m3;
    float Tot, percentage;

    // Reading the input value
    printf("Enter a num m1: ");
    scanf("%d", &m1);
    printf("Enter a num m2: ");
    scanf("%d", &m2);
    printf("Enter a num m3: ");
    scanf("%d", &m3);
    Tot=m1+m2+m3;
    percentage=Tot/3;
    
    printf("Total = %.2f\n",Tot);
    printf("Percentage = %.2f\n",percentage);
   
    if (percentage >= 60) {
        printf("Division = First");
    }
    else if(percentage >= 48){
        printf("Division = Second");
    }
    else if(percentage >= 36){
        printf("Division = Pass");
    }
    else{
        printf("Division = Fail");
    }
```

## OUTPUT:
![marks](https://github.com/user-attachments/assets/1d494959-b954-4250-8eca-6f4d34cf0e0f)


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

