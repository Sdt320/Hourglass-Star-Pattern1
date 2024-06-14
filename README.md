# Hourglass-Star-Pattern1
Let's refine the "Hourglass Star Pattern" to ensure it fits the classic hourglass shape correctly. The hourglass pattern should have a symmetrical top and bottom half, centered around the middle. Here’s the adjusted C program to generate the hourglass pattern:

### C Program for Hourglass Star Pattern

```c
#include <stdio.h>

int main() {
    int i, j, n;
    printf("Enter the number of rows for the half of the hourglass: ");
    scanf("%d", &n);

    // Upper part of the hourglass
    for (i = 0; i < n; i++) {
        for (j = 0; j < i; j++) {
            printf(" ");
        }
        for (j = i; j < 2*n - i - 1; j++) {
            printf("*");
        }
        printf("\n");
    }

    // Lower part of the hourglass
    for (i = n-2; i >= 0; i--) {
        for (j = 0; j < i; j++) {
            printf(" ");
        }
        for (j = i; j < 2*n - i - 1; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

### Explanation:

1. **Input Handling:**
   - The user inputs the value `n`, which represents half the height of the hourglass pattern.

2. **Upper Part:**
   - The outer loop `for (i = 0; i < n; i++)` iterates from 0 to `n-1`.
   - The first inner loop `for (j = 0; j < i; j++)` prints leading spaces.
   - The second inner loop `for (j = i; j < 2*n - i - 1; j++)` prints stars. The condition ensures that the number of stars decreases symmetrically as `i` increases.

3. **Lower Part:**
   - The outer loop `for (i = n-2; i >= 0; i--)` iterates from `n-2` to 0.
   - The first inner loop `for (j = 0; j < i; j++)` prints leading spaces.
   - The second inner loop `for (j = i; j < 2*n - i - 1; j++)` prints stars. The condition ensures that the number of stars increases symmetrically as `i` decreases.

### Result:

If the user inputs `5`, the program will generate the following hourglass pattern:

```
*********
 *******
  *****
   ***
    *
   ***
  *****
 *******
*********
```

### Pattern Name

This pattern is called the **"Hourglass Star Pattern"** because it visually resembles an hourglass, with a symmetrical top and bottom half of stars.
