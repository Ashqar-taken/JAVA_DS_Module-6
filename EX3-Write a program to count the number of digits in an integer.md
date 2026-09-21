# EX3 Write a program to count the number of digits in an integer.
## DATE: 27.07.2026
## AIM:
To write a java prograom to count the number of digits in an integer.

## Algorithm
1. Import the necessary libraries.
2. Input the elements from the user.
3. Obtain the number to count the digits from the user.
4. Define a recursive function to find the nubmer of digits in the given integer.
5. Display the result.

## Program:
```
/*
Program to to count the number of digits in an integer
Developed by: Ashqar Ahamed S T
RegisterNumber: 212224240018
*/

import java.util.Scanner;

public class Day3 {
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter number: ");
        int num = sc.nextInt();
        int count = countDigits(num);
        System.out.println("The number of digits in " + num + " is: " + count);
    }

    public static int countDigits(int num)
    {
        if(num == 0)
            return 0;

        return 1 + countDigits(num / 10);
    }
}

```

## Output:

<img width="625" height="176" alt="output Day3" src="https://github.com/user-attachments/assets/e3f9dbac-8367-4aad-8f8c-ac94a656ba30" />


## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
