# Ex4 You are given a Java program that performs matrix addition. If Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension, what will be the nature (even/odd/mixed) of the resulting matrix?
## DATE: 11.08.25
## AIM:
To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.

## Algorithm
Start the program.

Read the dimensions of both matrices (rows and columns). Check whether Matrix A and Matrix B have the same dimensions. If not, display “Matrices are not of same dimension” and stop.

Read Matrix A and check each element: If every element is odd, continue.

If any element is even, mark A as invalid and stop further checking.

Read Matrix A and check each element: If every element is odd, continue.

If any element is even, mark A as invalid and stop further checking.

If both matrices are valid, compute the resultant matrix (e.g., A + B or any operation specified). Determine the nature of the resultant matrix:

If all elements are odd, print “Resultant matrix is an Odd Matrix”.

If all elements are even, print “Resultant matrix is an Even Matrix”. Otherwise, print “Resultant matrix is a Mixed Matrix”.

Display the Resultant Matrix.

Stop the program. 

## Program:
```
/*
Program to ind the nature of resultant matrrix.
Developed by: Mugil Murgan
RegisterNumber:  212223230127
*/

import java.util.Scanner;

public class MatrixAddition {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int rows = sc.nextInt();
        int cols = sc.nextInt();

        int[][] A = new int[rows][cols];
        int[][] B = new int[rows][cols];
        int[][] result = new int[rows][cols];

        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                A[i][j] = sc.nextInt();
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                B[i][j] = sc.nextInt();
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                result[i][j] = A[i][j] + B[i][j];
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                System.out.print(result[i][j] + " ");
            }
            System.out.println();
        }

       
    }
}
```

## Output:

<img width="422" height="624" alt="image" src="https://github.com/user-attachments/assets/8711f81e-5705-4f46-9aac-dc78c6aaad8b" />


## Result:
Thus, the java program to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix is implemented successfully.
