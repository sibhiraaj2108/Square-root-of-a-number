# Find the square root of a number

## AIM:
To write a program to find the square root of a number.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Define a function.
2. Assign number_iters = 100 in the function to perform 100 iteratios.
3. Set i = 0.
4. Calculate  number = 0.5 * (number + a / number) for 100 iterations.
5. Return number

## Program:
```
/*
Program to find the square root for the given number(newton's method) using function.
Developed by: sibhiraaj R
RegisterNumber: 24010177
*/
```

## Output:
![image 1](<Screenshot 2024-11-13 141314.png>)
![image 2](<Screenshot 2024-11-13 141331.png>)
![image 3](<Screenshot 2024-11-13 141338.png>)

##  program
        def newton_sqrt(b, tolerance=1e-10):
            x = b / 2.0  
            while True:
                x_next = 0.5 * (x + b / x)
                if abs(x - x_next) < tolerance:
                    return x_next
                x = x_next
        number = int(input())
        sqrt_result = newton_sqrt(number)
        print(f"Square root of the number: {sqrt_result}")


## Result:
Thus the program to find the square root for the given number(newton's method) using function is written and verified using python programming.
