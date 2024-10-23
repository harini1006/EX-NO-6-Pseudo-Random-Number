# EX-NO-6-Pseudo-Random-Number

# AIM: 

Implementation of Pseudorandom Number Generation Using Standard library

# Algorithm:
Algorithm for Pseudorandom Number Generation:

Accept user input for the number of random numbers (count), minimum value (min), and maximum value (max).

Initialize the random seed using the current time (srand(time(NULL))).

Start a loop that runs count times to generate random numbers.

In each iteration, calculate a random number between min and max using the formula (rand() % (max - min + 1)) + min

Print the generated random number.

Repeat until count random numbers are generated, then terminate the program.

# Program:
```
Developed by:Harini V
Register no.: 212222230044
```
```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);
    printf("Enter the minimum value: ");
    
    scanf("%d", &min);
    printf("Enter the maximum value: ");
    scanf("%d", &max);
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }
    return 0;
}

```

# Output :
![{292EBFCA-7141-4A74-963C-A162B6303C2C}](https://github.com/user-attachments/assets/5c758db3-b7ea-4737-b4e2-b1ef7f8c6874)




# Result:
Thus the program to generate random numbers is implemented successfully











