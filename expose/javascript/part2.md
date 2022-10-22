**1. Number 3 will be printed in the console.**<br>
   This is because i is a var, it has a scope throughout the whole function discountPrices. i was last updated in the for loop to value 3 which is prices.length, thus 3 will be printed in the console.

**2. Number 150 will be printed in the console.**<br>
   This is because discountedPrice is a var, it has a scope throughout the whole function discountPrices. discountedPrice was last updated in the for loop to value 150 by prices[i] * (1 - disount), therefore 150 will be printed in the console.

**3. Number 150 will be printed in the console.**<br>
   This is because finalPrice is a var, it has a scope throughout the whole function discountPrices. finalPrice was last updated in the for loop to value 150 by Math.round(discountedPrice * 100) / 100, therefore 150 will be printed in the console.

**4. The function will return an array [50, 100, 150].**<br>
   The function returns the array discounted, which is updated to contain each discounted price in order calculated from the given prices and the discount. Given the input, the returned array would be [50, 100, 150].

**5. ReferenceError: i is not defined**<br>
   This is because variable i is of type let, which means that its scope is only in the block of the for loop where it is declared. Since line 12 is out of the scope, i is not defined there, thus this line has this error.

**6. ReferenceError: discountedPrice is not defined**<br>
   This is because variable discountedPrice is of type let, which means that its scope is only in the block of the for loop where it is defined. Since line 13 is out of the scope, discountedPrice is not defined there, thus this line has this error.

**7. Number 150 will be printed in the console.**<br>
   finalPrice is of type let, and it has a scope in the block of the function discountPrices. discountedPrice was last updated in the for loop to value 150 by prices[i] * (1 - disount), therefore 150 will be printed in the console.

**8. The function will return an array [50, 100, 150].**<br>
   The function returns the array discounted, which is updated to contain each discounted price in order calculated from the given prices and the discount. Given the input, the returned array would be [50, 100, 150].

**9. ReferenceError: i is not defined**<br>
   i is a let, therefore its scope is only within the for loop where it is defined. Line 11 is out of the for loop, thus i is not defined there, causing this error.

**10. Number 3 will be printed in the console.**<br>
    Since length is a const defined in the function, it has a scope throughout the whole function. Since the value is not changed, length stores the length of the array prices, which is 3. Thus, 3 will be printed.

**11. The function will return an array [50, 100, 150].**<br>
    The function returns the array discounted, which is updated to contain each constant discounted price in order calculated from the given prices and the discount. Given the input, the returned array would be [50, 100, 150]. Notice that discounted array is a const, but this only means that discounted is a constant reference and cannot be reassigned to another array. We can still change the elements within discounted.

**12.** Notations:<br>
   **A. student.name**<br>
   **B. student["Grad Year"]**<br>
   **C. student.greeting()**<br>
   **D. student["Favorite Teacher"].name**<br>
   **E. student.courseLoad[0]**<br>

**13.** Arithmetic<br>
   **A. output: '32'**<br>
      number 2 is converted to string '2' to concatenate with string '3'<br>
   **B. output: 1**<br>
      string '3' is converted to number 3 to perform arithmetic calculation 3 - 2<br>
   **C. output: 3**<br>
      null is converted to number 0 to add with 3<br>
   **D. output: '3null'**<br>
      null is converted to string 'null' to concatenate with string '3'<br>
   **E. output: 4**<br>
      true is converted to number 1 to add with 3<br>
   **F. output: 0**<br>
      false and null are both converted to number 0 to add together<br>
   **G. output: '3undefined'**<br>
      undefined is converted to string 'undefined' to concatenate with string '3'<br>
   **H. output: NaN**<br>
      string '3' is converted to number 3 for this arithmetic expression, but when converting to number, undefined becomes NaN. Therefore, this expression becomes 3 - NaN, which has a result of NaN, which is a computational error.<br>

**14.** Comparison<br>
   **A. true**<br>
      string '2' and number 1 are different types, thus they are converted to numbers to compare. '2' is converted to number 2, and since 2 > 1 is true, '2' > 1 is also true.<br>
   **B. false**<br>
      '2' and '12' are both strings, so it carries out a normal string comparison. The first character '2' is greater than '1', this '2' > '12', which means that '2' < '12' is false.<br>
   **C. true**<br>
      string '2' and number 2 are different types, thus they are converted to numbers to compare. '2' is converted to number 2, and since 2 == 2 is true, 2 == '2' is also true.<br>
   **D. false**<br>
      Since they are compared by strict equality check, type matters. Number 2 and string '2' are of different types, thus 2 === '2' is false.<br>
   **E. false**<br>
      boolean true and number 2 are of different types, thus true is converted to number 1. Since 1 == 2 is false, true == 2 is false.<br>
   **F. true**<br>
      Boolean(2) is true. Since true === true, true === Boolean(2).<br>

**15.** == is non-strict equality check. When the left and right have different types, it will first convert them into numbers and then compare for equality (however, null == undefined is true). === is strict equality check. When the left and right have different types, it will immediately return false without type conversion. It only returns true when both type and value equal.

**16.** [part2-question16.js](part2-question16.js)

**17. The result will be an array [2, 4, 6].**<br>
   modifyArray first create a newArr, then it has a for loop to push things into newArr. Specifically, in line 4, callback(array[i]) represents doSomething(array[i]), which returns 2 times the i-th indexed number in the given array. Therefore, newArr has the same size of the given array, and each element in newArr is 2 times the corresponding element in the given array. Thus, the result is a new array [2, 4, 6].

**18.** [part2-question18.js](part2-question18.js)

**19.** Output is the following:<br>
1<br>
4<br>
3<br>
2<br>
