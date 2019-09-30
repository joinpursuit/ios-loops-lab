# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**

/* Question #1 Answer

for i in 1...150{
    print(i)
}

*/

***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

/* Question #2 Answer

for i in 142..<159{
    print(i)
}

*/

***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

/* Question #3 Answer

for i in 15...80 where i % 2 == 0 {
    print(i)
}

*/

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

/* Question #4 Answer

for i in 19...51 where i % 2 == 1 {
    print(i)
}

*/

***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

/* Question #5 Answer

for i in 1..<100 where i % 10 == 5 {
    print(i)
}

*/


***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

/* Question #6 Answer

for i in 1...40 where i % 10 == 7 {
    print(i)
}

*/

***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

/* Question #7 Answer

for i in 20...150 where i % 3 == 0 {
    print(i)
}

*/

***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

/* Question #8 Answer

for i in 20...150 where i % 2 == 0 && i % 3 == 0 {
    print(i)
}

*/

***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

/* Question #9 Answer

for i in 20...150 where i % 10 == 4 {
    print(i)
}

*/

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

/* Question #10 Answer

for i in 20...150 where i  == 31  || i == 35 || i == 40 || i == 60 {
    print(i)
}

*/

***
## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

// Your explanation here
```
/* Question #11 Answer

The above loop will run indefinitely because the loop lacks a terminating condition. The only condition for the loop is for i to be greater than 3. Once inside the loop, i increases indefinitely.

*/

***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}

/* Question #12 Answer

var i = 5

while( i > 3 && i < 9)
{
    i += 1
}

*/
```

***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3) {
    i += 1
}

/* Question #13 Answer

var i = 5
var j = i

while( i > 3 && i < j + 1000)
{
    i += 1
}

*/
```

***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i > 3) {
    i += 1
}

/* Question #14 Answer

var i = 5
var j = i

while( i > 3 && i < j + 1000)
{
    i += 1
    if(i % 2 == 0){
        print(i)
    }
}

*/
```

***
## Question 15

What's the difference in syntax between the following two while loops?  Will their outputs be different?  Explain why or why not.

```swift
var i = 1
//loop one
while i <= 10 {
    print("i = \(i)")
    i += 1
}

//loop two
var i = 1

repeat {
    print("i = \(i)")
    i += 1
} while i <= 10

/* Question #15 Answer

The difference in syntax between loops one and two is that loop two will execute the code within its scope without checking for a condition for the first iteration. Loop one will not enter the loop if the conditions are not met first. I believe in this case, the outputs would be the same because the condition for entry into loop one is true. However, if the value of i exceeds 10, loop one will not even be entered, and thus have no output, while loop two will execute once, outputting one line.

*/
```

# Bonus =)

***
## Question 1

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

/* Bonus Question #1 Answer

Break will exit from a loop prematurely, while continue will force the next iteration of the loop to occur. 

for i in 1...100{
    if( i%2 == 0 ){
        continue
    }
    print(i)
}

for i in 1...100{
    if( i%2 == 0 ){
        break
    }
    print(i)
}

The loop with the continue statement will print only odd numbers. When it encounters the continue statement, the loop will move on to the next iteration without printing i to the screen. However, the second loop will simply terminate after the first time it encounters an even number.

*/
***
## Question 2

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}
```

[]1
[]2
[]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10

/* Bonus Question #2 Answer

The loop will print the numbers 1, 2, 3, 8, 9, and 10.

*/

***
## Question 3

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```

[]1
[]2
[]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10

/* Bonus Question #3 Answer

The loop will print the numbers 1, 2, and 3.

*/

***
## Question 4

Without using Xcode, what will the loop below print?  Explain below.

```swift
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}
```
/* Bonus Question #4 Answer

The loop will print 
x = 1, y = 1
x = 2, y = 1
x = 3, y = 1

*/
***
## Question 5

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

/* Bonus Question #5 Answer

var x = 0
var y = 0

while ( x <= 10 ) {

    while( y <= 10 ) {
    
        print("(\(x),\(y))")
        y += 1
        
    }
    x += 1
    y = 0
}

*/
***
## Question 6

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

/* Bonus Question #6 Answer

var x = 0
var y = 0

while ( x <= 10 ) 
{
    while( y <= 10 ){
    
    if ( (x - y) >= 5 || (y-x) >= 5 ){
    
        print("(\(x),\(y))")
        
        }
        
        y += 1
        
    }
    x += 1
    y = 0
}

*/

***
## Question 7

Print the first `N` square numbers. A **square number**, also called perfect square, is an integer that is obtained by squaring some other integer; in other words, it is the product of some integer with itself (ex. 1 = 1*1, 4 = 2 * 2, 9 = 3* 3 …).

Example:
Input: `var N = 5`

Output:
```swift
1
4
9
16
25
```

/* Bonus Question #7 Answer

for i in 1...N{
    print(i * i)
}

*/


***
## Question 8

Given an integer N draw a square of N x N asterisks. Look at the examples.

Example 1:
Input: `var N = 2`

Output:
```swift
**
**
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```

Hint 1
Try printing a single line of * first.

Hint 2
You can use print("") to print an empty line.

/* Bonus Question #8 Answer

var x = 0
var y = 0

while ( x <  N ){

    while( y < N ){
    
        print("*", terminator:"")
        y += 1
        
    }
    
    x += 1
    y = 0
    print()
}

*/
***
