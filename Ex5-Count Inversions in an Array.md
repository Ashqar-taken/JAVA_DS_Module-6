# Ex5 Count Inversions in an Array
## DATE: 29.07.2026
## AIM:
To write a Java program  to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j

## Algorithm
1. Import the necessary libraries.
2. Define the array by getting elements from user.
3. Declare a count variable to count the number of inversions.
4. Use for loop to iterate through the array. 
5. If the inversion condition is satisfied then increment count.
6. Display the final count.

## Program:
```
/*
Program to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
Developed by: Ashqar Ahamed S T
RegisterNumber: 212224240018
*/

import java.util.Scanner;
/* To write a Java program  to Count the number of inversions in 
an array where inversion is defined as: arr[i] > arr[j] and i < j */
public class Day5 {
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the number of ELements: ");
        int n = sc.nextInt();
        int[] arr = new int[n];
        System.out.println("Enter the ELements: ");
        for(int i=0;i<n;i++)
        {
            arr[i] = sc.nextInt();
        }
        int count = 0;
        for(int i=0,j=i+1;i<n && j<n;i++,j++)
        {
            if(arr[i] > arr[j])
                count++;
        }

        System.out.println("Final Count of Inversions : " + count);
    }
}


```

## Output:

<img width="590" height="245" alt="output Day5" src="https://github.com/user-attachments/assets/6f061fa9-1821-439a-b189-8b74c601bf48" />


## Result:
Thus the Java program to to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < jis implemented successfully.
