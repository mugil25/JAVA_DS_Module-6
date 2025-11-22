# EX3 Write a program to count the number of digits in an integer.
## DATE:11.08.25
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
Start the program.

Read an integer from the user.

Define a recursive function countDigits() that counts digits by dividing the number by 10 each time.

Base condition: if the number is 0, return 0.

Recursive step: return 1 + countDigits(number / 10).

Display the total count of digits. 

Stop the program. 

## Program:
```
/*
Program to to count the number of digits in an integer
Developed by: Mugil Murugan
RegisterNumber:  212223230127
*/
import java.util.Scanner;

public class CountDigits {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
     
        int num = sc.nextInt();
        
        int count = 0;
        int n = Math.abs(num); 
        
        
        if (n == 0) {
            count = 1;
        } else {
            while (n > 0) {
                n = n / 10;  
                count++;
            }
        }
        
        System.out.println("Number of digits: " + count);

        sc.close();
    }
}

```

## Output:
<img width="601" height="242" alt="image" src="https://github.com/user-attachments/assets/b2c2c162-498b-477d-a9ac-37b107992d20" />



## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
