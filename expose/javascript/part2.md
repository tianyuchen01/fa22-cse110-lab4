1. Number 3 will be printed in the console.<br>
   This is because i is a var, it has a scope throughout the whole function discountPrices. i was last updated in the for loop to value 3 which is prices.length, thus 3 will be printed in the console.

2. Number 150 will be printed in the console.<br>
   This is because discountedPrice is a var, it has a scope throughout the whole function discountPrices. discountedPrice was last updated in the for loop to value 150 by prices[i] * (1 - disount), therefore 150 will be printed in the console.

3. Number 150 will be printed in the console.<br>
   This is because finalPrice is a var, it has a scope throughout the whole function discountPrices. finalPrice was last updated in the for loop to value 150 by Math.round(discountedPrice * 100) / 100, therefore 150 will be printed in the console.

4. The function will return a list [50, 100, 150].<br>
   The function return the list discounted, which is updated to contain each discounted price in order calculated from the given prices and the discount. Given the input, the returned list would be [50, 100, 150].

5. 