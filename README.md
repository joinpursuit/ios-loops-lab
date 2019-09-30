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

Answer
```swift
for num in 1...150 {
    print(num)
}
```

***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

Answer
```swift
for num in 142..<159 {
    print(num)
}
```
***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

Answer
```swift
for num in 15...80 where num % 2 == 0 {
    print(num)
}
```
***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

Answer
```swift
for num in 19...51 where num % 2 == 1 {
    print(num)
}
```
***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

Answer
```swift
for num in 1..<100 where num % 10 == 5 {
    print(num)
}
```
***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

Answer
```swift
for num in 1..40 where num % 10 == 7 {
    print(num)
}
```
***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

Answer
```swift
for num in 20...150 where num % 3 == 0 {
    print(num)
}
```
***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

Answer
```swift
for num in 20...150 where num % 2 == 0 && num % 3 == 0 {
    print(num)
}
```
***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

Answer
```swift
for num in 20...150 where num % 10 == 4 {
    print(num)
}
```
***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

Answer
```swift
for num in 20...150 where num <= 60 {
    if num == 31 || num == 35 {
        print(num)
    } else if num >= 40 && num <= 60 {
        print(num)
    }
}
```
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
Answer
```swift
This will be an infinet loop since the condition is made to stop when i is less than 3 but in the loop it's only adding number to i and not subtracting. so i never gets less then 3
```
***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
Answer
```swift
var i = 5

while (i < 9) {
    i += 1
}
```
***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3 ) {
    i += 1
}
```
Answer
```swift
var i = 5
var count = 1

while (count < 1000 ) {
    i += 1
}
```
***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
Answer
```swift
var i = 5
var count = 1

while (count < 1000) {
    if i % 2 == 0 {
        print(i)
    }
}
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
```
Answer
```swift
The output will be the same since the while condition for both of the loop is set to stop on the same number
```
# Bonus =)

***
## Question 1

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

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


Answer
```swift
```
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


Answer
```swift
```
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
Answer
```swift
```
***
## Question 5

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

Answer
```swift
```
***
## Question 6

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

Answer
```swift
```
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
Answer
```swift
```
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
Answer
```swift
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

Answer
```swift
```
***
