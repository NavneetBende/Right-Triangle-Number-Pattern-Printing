PRINTING PATTERN:
1

23

456

78910

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Initialise an integer variable count=0 for incrementing
Take the number of rows as input from the user  and store it in any variable.(‘r‘ in this case).
Run a loop ‘r’ number of times to iterate through each of the rows. From i=0 to i<r. The loop should be structured as for( i=0 ; i<r : i++).
 Run a nested loop inside the main loop to print the digits in each row of the triangle. From j=0 to j<i. The loop should be structured as for( j=0; j<=i ; j++).
In the nested loop increment count and print it.
In the main loop print a new line.
Code in C:
#include<stdio.h>
int main()
{
int i,j,r,count;                         //declaring integer variables i,j for loops , r for number of rows and count for increment in value
count=0;                                //initialising count
printf("Enter the number of rows :\n"); //Asking user for input
scanf("%d",&r);                       //taking number of rows and saving it in variable r
for(i=0;i<r;i++)                     // loop for number of rows
   {
      for(j=0;j<=i;j++)              // loop for digits per each row
        {
           count++;                 //incrementing count
           printf("%d",count);      //printing digits
        }
      printf("\n");                 // printing newline after each row
   }
}
TAKING INPUT:DISPLAYING OUTPUT:
