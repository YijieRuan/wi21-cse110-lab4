1. Line 11 will output the length of the prices to the console because after the for loop, *i* will become *print.length*, which is the length of prices and since *i* was declared as **var**, which ignores the code block, meaning that *i* still exists after for loop.Therefore it will output successfully in terms of variable scope.
2. Line 12 will output the value of *discountPrice*, which is the price of discount, because *discountPrice* was declared as **var**, which ignores the code block. Therefore it will output successfully in terms of variable scope.
3. Line 13 will output the *finalPrice* of the last item in *Price*, which is declared as **var**, ignored the code block, which will print in terms of variable scope.
4. The function will output [50,100,150]. Since the *discount* is 0.5 and the for loop will make each price in *Price*, 100,200,300 in this case, multiply by **1-0.5**, round them, 50, 100, 150 in this case, and push them into array *discounted*. Therefore, the function will return the array *discounted* as [50,100,150].
5. Line 11 will have **ReferenceError: test is not defined** since *i* is declared as **let** and out of the scope of for loop.
6. Line 12 will have **ReferenceError: test is not defined** since *discountedPrice* is declared as **let** and out of the scope of for loop.
7. Line 13 will correctly print *finalPrice* of the last item in *Price* since the variable is declared outside of the for loop. 
8. The function will output [50,100,150]. The reason is the same as question 4 since nothing in terms of error or functionality has changed other than the **let** and **var**. This does not affect anything other than outputting these.
9. Line 11 will have error since *i* is declared as **let** and out of the scope of for loop. It will not output the test not defined error since the error before line 11 will occur before that.
10. Line 12 will have error since *discountedPrice* is declared as **const** and out of the scope of for loop.
11. Assuming all previous with no errors, line 13 will print 0, for *finalPrice* was declared as **const**, initalized as value 0, and unable to reassign the value due to the trait of **const**.
12. The function will have error since there exist multiple lines trying to reassign the **const** variables.
13. A. Accessing the value of the name property in the student object by **student.name**
    B. Accessing the value of the Grad Year property in the student object by **student['Grad Year']**
    C. Calling the function for the greeting property in the student object by **student.greeting()**
    D. Accessing the name property of the object in the Favorite Teacher property in student by **student['Favorite Teacher].name**
    E. Access the first index in the array of the courseLoad property of the student object by **student.courseLoad[0]**
14. A. ‘3’ + 2 will output **32** as 3 being a string, it became a concatenation.
    B. ‘3’ - 2 will output **1** as 3 being a string and 2 being a number with a none add expression, convert string into number and 3 - 2 equals to 1.
    C. 3 + null will output **3** as 3 being a number and null with numeber conversion will become 0, which made it **0 + 3 = 3**.
    D. ‘3’ + null will output **3null** as 3 being a string and concatenate with null.
    E. true + 3 will output **4** as 3 being a number and true with numeber conversion will become 1, which made it **1 + 3 = 4**.
    F. false + null will output **0** as false with number conversion will become 0 and null with numeber conversion will become 0, which made it **0 + 0 = 0**.
    G. “3” + undefined will output **3undefined** as 3 being a string and concatenate with undefined.
    H. “3” - undefined will output **NaN** since it will cause an error performing this operation and error will become **NaN**
15. A. ‘2’ > 1 outputs **true** because 2 as a string will convert into number 2 and larger than 1.
    B. ‘2’ < ‘12’ outputs **false** because both are strings and it will compare the first character, which is **2 < 1** and is false.
    C. 2 == ‘2’ outputs **true** because 2 as a string will convert into number 2 and is equal to 2.
    D. 2 === ‘2’ outputs **false** because first 2 is a number and second 2 is a string.
    E. true == 2 outputs **false** because true will converts into number 1 and does not equal to 2.
    F. true === Boolean(2) outputs **true** because *Boolean(2)* converts into **true** with the type boolean and *true === true*.
16. **"=="** checks if the values are equal. On the other hand, **"==="** checks if both the values and types are the same.
17. **'How are you?'** will be printed because *2==true* returns false and *2* will be converted into Boolean value and make the else if block **true** and return **'How are you?'**
18. see part1_18.js
19. The function will return **[6,8,10]**. The function puts array [1,2,3] and the doSomething function in the parameter. In the for loop, for each number in the array,the loop tries to call the doSomething function and add 2 to the number and then multiply two with the sum and push it into newArr. Therefore, **(1+2)X2 = 6**, **(2+2)X2 = 8**, **(3+2)X2 = 10**. which made the newArr **[6,8,10]**, and this is what is returned.
20. see part1_20.js
21. It will first output 1 then 4, then 3, then 2. Since 1 is the first called log, 2 and 3 has setTimeout, which made them into the next cycle, which made second output to be 4. 3 has 0 millisecond of delay so it will output before 2.