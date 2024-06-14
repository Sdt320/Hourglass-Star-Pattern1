# Hourglass-Star-Pattern1
 The hourglass pattern should have a symmetrical top and bottom half, centered around the middle.
#Explanation:

I##nput Handling:

The user inputs the value n, which represents half the height of the hourglass pattern.
##Upper Part:

The outer loop for (i = 0; i < n; i++) iterates from 0 to n-1.
The first inner loop for (j = 0; j < i; j++) prints leading spaces.
The second inner loop for (j = i; j < 2*n - i - 1; j++) prints stars. The condition ensures that the number of stars decreases symmetrically as i increases.
##Lower Part:

The outer loop for (i = n-2; i >= 0; i--) iterates from n-2 to 0.
The first inner loop for (j = 0; j < i; j++) prints leading spaces.
The second inner loop for (j = i; j < 2*n - i - 1; j++) prints stars. The condition ensures that the number of stars increases symmetrically as i decreases.
##Result:
If the user inputs 5, the program will generate the following hourglass pattern:


*********
 *******
  *****
   ***
    *
   ***
  *****
 *******
*********
Pattern Name
This pattern is called the "Hourglass Star Pattern" because it visually resembles an hourglass, with a symmetrical top and bottom half of stars.

