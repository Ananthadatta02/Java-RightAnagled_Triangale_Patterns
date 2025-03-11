# Right-Angled Triangle Pattern in Java

## Overview
This Java program prints a right-angled triangle pattern using asterisks (`*`). It uses nested loops to control the number of rows and columns, incrementing the count of asterisks printed in each row.

## Code Explanation
```java
public class RightAngledTriangle
{
    public static void main(String[] args)
    {
        int star = 1; // Variable to control the number of '*' printed in each row
        
        for(int i = 0; i <= 3; i++) // Outer loop controls the number of rows
        {
            for(int j = 1; j <= star; j++) // Inner loop controls the number of '*' per row
            {
                System.out.print("*"); // Prints '*' without a newline
            }
            star++; // Increments star to print one more '*' in the next row
            System.out.println(); // Moves to the next line after printing '*' for the current row
        }
    }
}
```

## Breakdown of the Code

### 1. **Variables:**
   - `int star = 1;` → Initializes the variable `star`, which determines the number of `*` in each row.

### 2. **Outer `for` Loop (`for(int i = 0; i <= 3; i++)`)**
   - Runs **4 times** (`i = 0` to `i = 3`), controlling the number of rows printed.
   - Iterates from `0` to `3`, meaning the triangle will have **4 rows**.

### 3. **Inner `for` Loop (`for(int j = 1; j <= star; j++)`)**
   - Controls the number of `*` printed in each row.
   - Runs from `1` to `star`, meaning the number of `*` increases in each row.

### 4. **Printing Statements:**
   - `System.out.print("*");` → Prints `*` in the same line.
   - `System.out.println();` → Moves to the next line after printing all `*` for a given row.

### 5. **Increment Statement (`star++`)**
   - Increases the value of `star` after each row to ensure the next row has one more `*` than the previous.

## Output of the Program
```
*
**
***
****
```
This output forms a right-angled triangle with 4 rows.

## Time Complexity Analysis
- The **outer loop** runs `n` times (`O(n)`).
- The **inner loop** runs from `1` to `n`, resulting in a **total of `O(n^2)` iterations** in the worst case.
- Hence, the **time complexity is O(n²)**.

## Space Complexity Analysis
- The program uses only a few integer variables (`star`, `i`, and `j`), so the **space complexity is O(1)** (constant space usage).

## Summary
- This program prints a right-angled triangle of `*` characters.
- Uses **nested loops** to control row and column output.
- Uses **increment operations** to progressively increase the number of `*` per row.
- **Efficient with O(n²) time complexity** but requires only constant extra space.

## Clone
```
git clone https://github.com/Ananthadatta02/Java-RightAnagled_Triangale_Patterns.git
```
