# Permutations-In-Which-N-People-Can-Occupy-R-Seats-In-A-Classroom-C-Program

Which n people can occupy r seats in a classroom in C
Which n people can occupy r seats in a classroom in C programming helps in identifying the r number of seats that can be occupied by n number of people. Such a program is known as the possible permutations. Here, We need to write a code to find all the possible ways in which n people can occupy r number of seats in a classroom/theater.

Permutations In Which N People Can Occupy R Seats in C
Way 2 Of Asking Question
Write code to find all possible permutations in which n people can occupy r seats in a theater
Problem Statement :
In a classroom some of the seats are already occupied by students and only a few seats are available in the classroom. The available seats are assumed as r and n number of students are looking for the seat. We need to find in how many different permutations n number of students can sit on r number of chairs.

Algorithm
Input number of students in n
Input number of seats in r
Use permutation formula { factorial(n) / factorial(n-r) }
Print Output
Permutations in which n people can occupy r seats in aclassroom in C programming
Related Pages
Octal to Binary conversion

Quadrants in which a given coordinate lies
 
Maximum number of handshakes

Addition of two fractions

Replace all 0’s with 1 in a given integer

While loop in C
C code
Run
//Permutations in which n people can occupy r seats
#include<stdio.h>
    
//function for factorial
int factorial(int num)
{
    int fact=1;
    for(int i=num; i>=1 ;i--)
        fact*=i;
    return fact;
}
    
//main program
int main()
{
    int n,r;
    printf("Enter number of people: ");
        
    //user input
    scanf("%d",&n);
    printf("Enter number of seats: ");
        
    //user input
    scanf("%d", &r);
        
    //finding all possible arrangements of n people on r seats
    // by using formula of permutation
    int p = factorial(r)/factorial(r-n);

    //printing output
    printf("Total possible arrangements: %d",p);

    return 0;
}
Output
Enter number of people: 5
Enter number of seats: 9
Total possible arrangements: 15120
