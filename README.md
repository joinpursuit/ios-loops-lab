# Kelby Mittan
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

# Answer

```swift
for i in 1...150 {
    print(i)
}

```

***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

# Answer

```swift
for i in 142..<160 {
    print(i)
}
```
***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

# Answer

```swift
for i in 15...80 where i % 2 == 0 {
    print(i)
}
```
***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

# Answer

```swift
for i in 19...51 where i % 2 != 0 {
    print(i)
}
```

***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

# Answer 

```swift
for i in 1..<100 where i % 10 == 5 {
    print(i)
}
```

***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

# Answer

```swift
for i in 1..<100 where i % 10 == 7 {
    print(i)
}
```

***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

# Answer

```swift
for i in 20...150 where i % 3 == 0 {
    print(i)
}
```

***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

# Answer

```swift
for i in 20...150 where (i % 3 == 0 && i % 2 == 0) {
    print(i)
}
```

***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

# Answer

```swift
for i in 20...150 where i % 10 == 4 {
    print(i)
}
```

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

# Answer 
```swift
for i in 20...150 where i == 31 || i == 35 || (i >= 40 && i <= 60) {
    print(i)
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
```
# Answer
## This loop will run an infinite number of times because adding 1 to i = 5 then i = 6 and so on will always be greater than 3.


***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
# Answer
```swift
var i = 5

while (i > 3 && i <= 9) {
    i += 1
}
```

***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
# Answer
```swift
var i = 5

while (i > 3) {
    i += 1
    if i == 1005 {
        break
    }
}
```
# or
```swift
var i = 5

repeat {
    i > 3
    i += 1
} while i < 1005
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
# Answer
```swift
var i = 5

while (i > 3) {
    i += 1
    if i == 1005 {
        break
    }
}
if i % 2 == 0 {
    print(i)
}
```
# or

```swift
var i = 5

repeat {
    i > 3
    i += 1
} while i < 1005
if i % 2 == 0 {
    print(i)
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
# Answer
##  Both loops will have the same output, but are different in how they process the code. The difference is that the the first loop is telling a program that "while" a condition is true to complete a following process. Whereas is the second loop the program is told to initialize a process until a condition is met.

# Bonus =)

***
## Question 1

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

# Answer
## A continue statement will end the execution of the specified conditions of a loop statement but will continue the loop statement, a break will actually end the execution of a loop statement all together.

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
# Answer
[X]1
[X]2
[X]3
[]4
[]5
[]6
[]7
[X]8
[X]9
[X]10

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

[X]1
[X]2
[X]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10

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
# Answer
## This loop will print:

x = 1 , y = 1
x = 2 , y = 1
x = 3 , y = 1

It prints this way because once y == 2 in the inner loop it goes back to continuing to execute the outer loop

***
## Question 5

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

# Answer

```swift

for x in 1...10 {
  for y in 1...10 {
    print("(\(x),\(y))")
    }
}
```

***
## Question 6

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

# Answer

```swift

for x in 1...10 {
  for y in 1...10 {
        if (y - x >= 5) || (x - y >= 5) {
            print("(\(x),\(y))")
        }
    }
}
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
# Answer
```swift
var N = 5

var square = 1

while square <= N {
    print(square * square)
    square = square + 1
}
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
# Answer
```swift
var N = 2

for _ in 1...N {
    for _ in 1...N {
        print("*", terminator: "")
    }
    print("")
}
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```
# Answer
```swift
var N = 3

for _ in 1...N {
    for _ in 1...N {
        print("*", terminator: "")
    }
    print("")
}
```

Hint 1
Try printing a single line of * first.

Hint 2
You can use print("") to print an empty line.

***
