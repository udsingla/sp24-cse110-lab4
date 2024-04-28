1. It will print out the number 3. This is because variables defined using var have a function scope so the value of variable i can be used throughout the function discountedPrices. Since line 12 is within this function, it can access the value and print out 3. (it is 3 as the loop runs up till length of price which is 3 and once i becomes 3, it exits the loop and reaches line 12).
2. It prints out 150 since it is the discounted price of the last element in prices array. The value of discountedPrice gets updated in every iteration of the loop and when the loop exits it has the last value from the array.
3. It prints out 150 as well. This is again the rounded value of the discountedPrice from last question. Since it gets updated every iteration as well, it will be 150 as well.
4. The function will return an array containing the discounted prices of the input array after discounting those prices by the given discount [ 50, 100, 150 ]. This is because discounted is an array and the function successfully calculates the discounts and adds the discounted prices to the discounted array which is returned at the end.
5. It will throw an error as let has a block scope and the variable i is defined in a for loop using let, so the value of i will only be accessible inside the for loop block. As a result line 12 will return an error that the variable is not defined.
6. It will throw an error as let has a block scope and the variable discountedPrice is defined in the block of for loop. The variable is not accessible outside of the for loop because of which it shows an error of variable not defined.
7. It will print out 150. This is because finalPrice is defined outside the for loop and in the function block. This means the value can be accessed and updated by the for loop and it also remains available after the for loop ends within the block of the function. Since line 14 is inside the function block, it can access the updated value. It is 150 as it is the discounted price of the last item in the input array. The for loop runs thrice and goes through every element of the array so the latest value that the variable has is of the last element in the input array.
8. The function will return an array containing the discounted prices of the input array after discounting those prices by the given discount [ 50, 100, 150 ]. This is because discounted is an array and the function successfully calculates the discounts and adds the discounted prices to the discounted array which is returned at the end. Since discounted is defined using let in the function block and not in the for loop block, it can get updated in the for loop and also be accessed by the return statement at the end which is inside the function block.
9. It will throw an error as let has a block scope and the variable i is defined in a for loop using let, so the value of i will only be accessible inside the for loop block. As a result line 12 will return an error that the variable is not defined.
10. It will print out 3 as that is the length of the input array which is stored in the length variable using const in the function and since it is being accessed inside the function and not being updated, it will print out that value.
11. The function will return an array containing the discounted prices of the input array after discounting those prices by the given discount [ 50, 100, 150 ]. This is because discounted is an array and the function successfully calculates the discounts and adds the discounted prices to the discounted array which is returned at the end. Even though discounted is a const variable, it is still mutable as an array. Const only prevents it from being reassigned. In the program we are not reassigning the value of discounted but just adding elements in the array. Since reassigning doesn't take place, we are successfully able to return the array with the discounted prices.

<br>
12. 

A) student.name

B) student['Grad Year']

C) student.greeting()

D) student['Favorite Teacher'].name

E) student.courseLoad[0]

<br>
13.

A) '32' - This was given as '3' is a string and when we do + 2, it converts 2 to a string which can then be concatenated with 3.

B) 1 - This was outputed as - operator cannot be performed on strings so in this case '3' gets converted to integer and then it is 3 - 2 which gives 1.

C) 3 - This is because 3 is an integer and null is converted to 0 in numerical terms so 3 + 0 is still 3.

D) '3null' - Since '3' is a string, null gets converted to a string 'null' and gets concatenated.

E) 4 - Since true has value 1, adding 3 to it gives 4

F) 0 - Since false has value 0 and null also has value 0, they both add up and give result 0.

G) '3undefined' - This is because '3' is a string and when we do + undefined, undefined gets converted to string 'undefined' and as a result gets concatenated.

H) NaN - The '-' operator as seen before results in converting the string to numerical value. However, undefined cannot be converted to a numerical value as a result it returns not a number (NaN).

<br>
14.

A) true - '2' gets converted to numerical value for comparison as the other value is number and this makes the statement 2 > 1 true.

B) false - Since both values are strings, they are compared using lexographical order and according to that '2' > '12' so it makes the statement false.

C) true - This is true as when we use '==', it converts the values to the same data type and only checks is those values after conversion are equal.

D) false - This is because when we use '===', it checks for both type equality as well as value equality which means they both need to be of the same tyoe as well. Here string and number are not the same type.

E) false - true has the value 1, so when converted, 1 is not equal to 2 and this gives false.

F) true - This is because 2 gets type casted to Boolean and since any number other than 0 is true, we get true from the statement since the value is true for both and the type is same as well.

<br>
15. '===' is for strict equality checks while '==' is for loose equality checks. '==' compares two values for equality after converting them to a common type. On the other hand, the '===' compares both the value and the type of the operands, which means no type conversion is performed. '==' allows for a more flexible comparison as type differences can be ignored. '===' makes sure that the comparisons are clearer as both value and type must be equal for it to return true.


<br>
<br>
17. The result will be that it will return a new Array with the elements which are numbers multiplied by 2 of the original input array. This is because in the input to modifyArray, we give an array [1,2,3] and a function doSomething. Inside modifyArray, it creates a newArr array and then it starts a for loop that runs for the length of the input array. With every iteration it calls the callback function parameter on the input array elements. In this case the callback function parameter is the doSomething function. The doSomething function multiplies the number by 2 and returns that value. So, we get this new value and it is pushed into the newArr array. Once this is done for every element in the input array, the for loop ends and the newArr array is returned which has the updated values of the original input array.


<br>
<br>
19. The output is:

```
1
4
3
2
```

Here everything except 2 gets printed immediately while 2 gets printed after 1 second. When printNums is called, it prints out 1, then goes to next line where it encounters a timeout for 1000 milliseconds = 1 second. So the number 2 is printed after 1 second. The program, however, doesn't wait and goes ahead to next line where it encounters another setTimeout but this time with time 0. Even though the time is 0, it is still not executed immediately and the program goes on to the next line i.e. line 5 and 4 is printed out. After that 3 is printed out and when 1 second has passed, 2 is printed out to the console as well.
