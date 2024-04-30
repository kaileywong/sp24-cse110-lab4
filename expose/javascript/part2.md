1. At line 12, the value of `i` (3) will be printed (this is the length of the `prices` array). `i` is declared as a var, which means it has function scope. So even though it is declared in the for loop, it is still accessible outside the loop scope to print its value at line 12 (still within the function).

2. At line 13, the value of the `discountedPrice` variable (150) will be printed.  `discountedPrice` is declared as a var, so it has function scope and will still be accessible within the function, but outside the for loop, to print its value. The value will be 150 because this is the calculation for `discountedPrice` after the last iteration of the for loop runs using the last element of the array (300).

3. At line 14, the value of `finalPrice` (150) will be printed. `finalPrice` is a var and at line 14 is still within the function scope. Its value at this point will be from the last calculation within the for loop. In this case, the calculation for the last element of the array (300) is 150 (the rounding is redundant in this case).

4. This function returns the `discounted` array, which is an array of discounted prices that uses the given `discount` to calculate the discounted price for each amount in `prices`. In this case, the `prices` array is `[100, 200, 300]` and the discount is `0.5`. The for loop goes through each value in the array to calculate the discounted price (rounded up to 2 decimal points) and adds it to the `discounted` array. The final returned array in this case will be `[50, 100, 150]`.

5. This code causes an error because the `i` variable is declared using let, which means it has block scope. In this case, it will only be accessible within the for loop, and at line 12 this is outside the scope of that loop. So trying to print the value of `i` will result in an error.

6. This code causes an error because the `discountedPrice` variable is declared using let, which means it has block scope. For this code, it will only be accessible within the for loop. At line 13, the variable is outside the scope of that loop so trying to print its value will result in an error.

7. At line 14, the value of `finalPrice` (150) will be printed. `finalPrice` is declared at the beginning of the function with let, so at line 14 it is still within the function scope. Its value at this point will be from the last calculation within the for loop. In this case, the calculation for the last element of the array (300) is 150.

8. This function returns the `discounted` array. It uses the given `discount` to calculate the discounted price for each element in `prices`, which in this case is `[100, 200, 300]` and the discount is `0.5`. The for loop will go through each value in the array to calculate the discounted price rounded to 2 decimal places then add it to the `discounted` array. The final returned array in this case will be `[50, 100, 150]`.

9.  This code causes an error because the `i` variable is declared using let. THis means it has block scope and in this case, it will only be accessible within the for loop. At line 11 this is outside the scope, so trying to print the value of `i` will result in an error.

10. At line 12, the code will print the value of the const variable `length` (3). At line 4, the variable is declared to be `prices.length`, or the length of the `prices` array, which is 3 in this case. The declaration is within the scope of the function, so the variable is still within scope at line 12, and its value will be printed.

11. This function returns the array assigned to the `discounted` variable. It uses the given `discount` to calculate the discounted price for each element in `prices`, in this case `[100, 200, 300]` with `discount` as `0.5`. The for loop will go through each value in the array to calculate the discounted price rounded to 2 decimal places then push it to the `discounted` array. This is valid even though `discounted` is a const variable because the value is not being reassigned, but the array assigned to it is being updated. The final returned array for the variable in this case will be `[50, 100, 150]`.

12. 
A. `student.name`

B. `student['Grad Year']`

C. `student.greeting()`

D. `student['Favorite Teacher'].name`

E. `student.courseLoad[0]`

13.  
A. `'32'`: `2` is converted to its string representation `'2'` then concatenated

B. `1`; `'3'` is converted to an integer then `3-2` is calculated

C. `3`: `null` is converted to 0 then `3+0` is calculated

D. `'3null'`: `null` is converted to its string representation `'null'` then concatenated

E. `4`: `true` is converted to `1` then added

F. `0`: `false` and `null` are each converted to the `0` representation then added

G. `'3undefined'`: `undefined` is converted to its string representation `'undefined'` then concatenated

H. `NaN`: `undefined` becomes `NaN` and subtracted from the integer representation of `'3'`, `3` is still `NaN`

14.   
A. `true`: `'2'` is converted to its integer representation `2` which is larger than `1`

B. `false`: the string `2` is lexicographically after `12`

C. `true`: the string `'2'` is converted to its integer representation `2` which is equal to `2`

D. `false`: the `===` operator checks equality without type conversion, a string and number of different types

E. `false`: `true` is converted to `1` which is not equal to `2`

F. `true`: `Boolean(2)` has a truthy value and will be equal to the boolean `true`

15.  The `==` operator checks for equality using type conversions (more of a 'test') whereas the `===` operator is a strict equality operator that checks for equality without type conversions.

17.  If the function is called with `modifyArray([1,2,3], doSomething)` the returned result will be the array `[2,4,6]`. In this case, the function `doSomething` is passed to `modifyArray` as the `callback` variable. The function will have `newArr` initialized to be empty, then the loop will go through each element in the array `[1,2,3]` and push the result of the `callback` function on that element to the `newArr` array. `doSomething` here multiplies the value it is passed by 2, so the resulting array stored at `newArr` will be `[2,4,6]`.

19.  The code first prints `1`, `4`, then `3` (even with a timeout of 0 it will go on a queue until the thread has finished executing). A second later the code will print `2`.
