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

```swift 

for i in 0...15 { // 150 for hw
    print(i)
}

```

***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

```swift

for i in 142..<159 { 
    print(i)
}
```

***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

```swift 
for i in 1...10 { // 150 for hw
    if i % 2 == 0 {
        print(i, terminator: ",")
}
}
```

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

```swift 
for i in 1...10 { // 150 for hw
    if i % 2 != 0 {
        print(i, terminator: " ")
    }
}
```

***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

```swift 
for number in 1...100 where number % 10 == 5 {
    print("\(number)", terminator: ", ")
}
```
***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

```swift 
for number in 1...40 where number % 10 == 7 {
    print("\(number)", terminator: ", ")
}
```
***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

```swift 

for i in 20...150 where i % 3 == 0 {
    print(i, terminator: " ")
}
```
***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`
```swift
for i in 20...150 where i % 3 == 0 && i % 2 == 0 {
    print(i, terminator: " ")
}
```
***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`
```swift 
for number in 20...150 where number % 10 == 4 {
    print("\(number)", terminator: ", ")
}
```

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

```swift 
print("These are the special numbers:")
for number in 20...150 where number == 31 || number == 35 || number >= 40 && number <= 60{
    print("\(number)", terminator: ", ")
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
```
Answer: 

// This is an infinite loop. Variable i starts off fullfilling the i>3 condition and is then incremented by 1 only increasing the value. i will never be less then 3.
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

```swift
var i = 5

while (i <= 9) {
    i += 1
}
```
***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 0

while (i <= 1000) {
     
        print(i)
    
    i += 1
}
```

***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 0

while (i <= 1000) {
    if i % 2 == 0 {
        print(i)
    }
    i += 1
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
```
//Answer: The first loop is a while loop and the second is a repeat/while loop. Both outputs will be the same, printing the value of i after incrementing it by one. This is because the conditon for both the loops is the same, both are incrementing by 1 and both print statements are the same.
```

# Bonus =)

***
## Question 1

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

```
//Answer: 

The Break statment is used to exit a loop. 
The continue statement tells a loop to stop what it is doing and to continue to the next value. 

for cookie in 0..<5 {
    if cookie < 4 {
        continue
    } else {
        break
    }
}
print("Ameni is happy")

```

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

***
## Question 5

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

***
## Question 6

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

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

***
