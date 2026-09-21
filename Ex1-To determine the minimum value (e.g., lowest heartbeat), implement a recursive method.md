# EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## DATE: 25.07.29
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm
1. Import the necessary utilities.
2. Obtain the number of sensor readings from user.
3. Declare a readings array with the number.
4. Obtain the sensor readings.
5. Define a method to recursively find minimum value.
6. Display the result.

## Program:

```
/*
Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by: Ashqar Ahamed S T
RegisterNumber: 212224240018
*/

import java.util.Scanner;

 public class Day1 {
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the number of sensor reeadings: ");
        int n = sc.nextInt();
        System.out.println("Enter the readings: ");
        int[] readings = new int[n];

        for(int i=0;i<n;i++)
        {
            readings[i] = sc.nextInt();
        }

        int min = findMin(readings, n);
        System.out.println("The minimum reading is: " + min);
    }

    public static int findMin(int[] arr, int n)
    {
        if(n==1)
            return arr[0];

        int min = findMin(arr, n-1);

        return Math.min(arr[n-1], min);
    }
}

```



## Output:

<img width="532" height="176" alt="output Day1" src="https://github.com/user-attachments/assets/ff14da28-068c-4edb-abd2-63aa402d185e" />


## Result:
Thus the JAVA prograM ti find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully
