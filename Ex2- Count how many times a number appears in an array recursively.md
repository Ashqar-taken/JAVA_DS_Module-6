# Ex2 Count how many times a number appears in an array recursively.
## DATE: 27.07.2026
## AIM:
To write a Java program to Count how many times a number appears in an array recursively.

## Algorithm
1. Import the necessary libraries.
2. Input the elements from the user.
3. Obtain the number to count from the user.
4. Define a recursive function to find the count of the target.
5. Display the result.

## Program:
```
/*
Program Count how many times a number appears in an array recursively.
Developed by: Ashqar Ahamed S T
RegisterNumber: 212224240018
*/

import java.util.Scanner;
/* Count how many times a number appears in an array recursively. */
public class Day2 {
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the number of Elements: ");
        int n = sc.nextInt();
        int[] arr = new int[n];
        System.out.println("Enter the ELements: ");
        for(int i=0;i<n;i++)
        {
            arr[i] = sc.nextInt();
        }
        System.out.println("Enter the number to count: ");
        int N = sc.nextInt();
        int count = CountArray(arr, n, N);
        System.out.println("The number of times " +  N + " appears in the array is: " + count);
    }

    public static int CountArray(int[] arr, int n, int target)
    {
        if(n==0)
            return 0;

        int count = CountArray(arr, n-1, target);

        if(arr[n-1] == target)
            count++;

        return count;
    }
}

```

## Output:

<img width="636" height="135" alt="output Day2" src="https://github.com/user-attachments/assets/e44dd49b-a7cb-4c78-9198-2b50657fb10e" />


## Result:
Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.
