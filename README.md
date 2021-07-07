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
let clone = 1...150


Answer:
```
for num in 1...150 {
print(num)
}
```

***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

Answer:
```
for num in 142..<159 {
    print(num)
}
```
***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**
Answer:
```
for evenNum in 15...80 {
    if evenNum % 2 == 0 {
        print(evenNum)
    }
}
```

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**
Answer:
```
for oddNumber in 19...51 {
    if oddNumber % 2 == 1 {
        print(oddNumber)
    }
}
```

***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**
Answer:
```
for numEndIn5 in 5..<100 {
    if numEndIn5  % 5 == 0 && numEndIn5 % 10 != 0 {
        print(numEndIn5)
    }
}
```

***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**
Answer:
```
for numEndIn7 in 1...40 {
    if numEndIn7 % 10 == 7 {
    print(numEndIn7)
    }
}

```


***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

Answer:
```
for numDiv3 in 20...150 {
    if numDiv3 % 3 == 0 {
        print(numDiv3)
    }
}
```

***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`
Answer:
```
for numDiv32 in 20...150 {
    if numDiv32 % 3 == 0 && numDiv32 % 2 == 0  {
        print(numDiv32)
    }
}
```

***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

Answer:
```
for number in 20...150 {
    if number % 10 == 4 {
    print(number)
    }
}
```

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

```
for number in 20...150 {
    if number == 31 || number == 35 || number == 40 || (number >= 40 && number <= 60) {
    print(number)
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

```
Answer:
It will be an infinite i+1= 1 will always be greater than 3 so there are no limitations.
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
Answer:
```
while (i > 3) {
    i += 1
    print(i)
    if i == 9 {
        break
    }
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

***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i > 3) {
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
