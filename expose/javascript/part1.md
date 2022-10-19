1. values added:  20

2. final result:  20

3. values added:  20

4. ReferenceError: result is not defined <br>
   This is because variable result is of type let, it only has a scope within the block of the if statement where it is declared. Since line 13 is out of that block, variable result is not defined at that spot, which causes error.

5. TypeError: Assignment to constant variable.<br>
   The program will crash at line 7 when we try to reassign the const variable, which causes the error. Line 9 is not executed.

6. TypeError: Assignment to constant variable.<br>
   Same as above, the program will crash at line 7 when we try to reassign the const variable, which causes the error. Line 13 is not executed.