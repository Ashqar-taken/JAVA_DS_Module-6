# Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?
## DATE: 28.07.2026
## AIM:
To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.

## Algorithm
1. Import the necessary libraries.
2. Create two matricies A and B with given elements.
3. Declare a third matrix and use nested for loops to add matrix A and matrix B
4. Display the third matrix to find the nature of the resulting matrix.

## Program:
```
/*
Program to ind the nature of resultant matrrix.
Developed by: Ashqar Ahamed S T 
RegisterNumber: 212224240018
*/

import java.util.Scanner;
public class main{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int m = sc.nextInt();
        int[][] arr1 = new int[n][m];
    
        for(int i=0;i<n;i++)
        {
            for(int j=0;j<m;j++)
            {
                arr1[i][j] = sc.nextInt();
                
            }
        }
        int[][] arr2 = new int[n][m];
        for(int i=0;i<n;i++)
        {
            for(int j=0;j<m;j++)
            {
                arr2[i][j] = sc.nextInt();
            }
        }
        
        int[][] arr3 = new int[n][m];
        for(int i=0;i<n;i++)
        {
            for(int j=0;j<m;j++)
            {
                arr3[i][j]  = arr1[i][j] + arr2[i][j];
                System.out.printf("%d ",arr3[i][j]);
            }
            System.out.println();
        }
        
    }
}

```

## Output:

<img width="603" height="647" alt="output Day4" src="https://github.com/user-attachments/assets/17d01fa9-bcab-43e3-9046-ba3c6bb745e8" />


## Result:
Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.
