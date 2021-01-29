DevTools: Debugging
* The bug is that the type of both **num1** and **num2** are string when inputting, which made the **result** a string as well. Adding two string means concatenate two string, which creates the bug that when I input 4 and 10, it just output 410.
* I would fix this by convert both **num1** and **num2** type into number. So what I did was to put a **Number()** when the function is declaring both **num1** and **num2** in **printSum()** function. See more on my screenshot of **fixed_version.png**

DevTools - Network Tab
1. citylots.json
2. part2.js
3. 11.1MB
4. 7.04s
5. Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.117 Safari/537.36
6. Apache
7. Tue, 26 Jan 2021 22:14:13 GMT
8. application/json
9. fetchData
