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

answer below:

```swift

for i in 1...150 {
    print(i)
}

// OR you can use a repeat-while

var number = 1
repeat {
    print(number)
    number += 1
} while number <= 150
```

***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

answer below:

```swift

//using a for loop
for i in 143..<159 {
    print (i)
}

//using a while loop
i = 143
while i < 159 {
    print(i)
    i += 1
}

//using a repeat-while loop
i = 142
repeat {
    i += 1
    print(i)
} while i <= 158

```

***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

answer below:

```swift

for i in 15...80 where i % 2 == 0 {
    print(i)
}

```
***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

answer below:

```swift

for i in 19...51 where i % 2 != 0 {
    print(i)
}
```
***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

answer below:

```swift

for i in 2..<100 where i % 10 == 5 {
    print(i)
}

```
***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

answer below:

```swift

for i in 1...40 where i % 10 == 7 {
    print(i)
}

```
***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

answer below:

```swift

for i in 20...150 where i % 3 == 0 {
    print(i)
}

```
***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

answer below:

```swift

for i in 20...150 where i % 3 == 0 && i % 2 == 0 {
    print(i)
}

```

***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

```swift

for i in 20...150 where i % 10 == 4 {
    print(i)
}

```
***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

answer below:

```swift

for i in 20...150 where i == 31 || i == 35 || (i - 40 >= 0 && i - 60 <= 0) {
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

// Your explanation here

The loop will run endlessly.  In basic terms: while "i is greater than 3, add 1 to i" Would mean when the loop goes over its first iteration and realizes i = 5, it will keep adding to i.  
```

***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}

answer below:

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

while (i > 3) {
    i += 1
}

answer below:

i = 5
while (i > 3) {
    i += 1
    if i == 1005 {
        break
    }
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

answer below:

var i = 5

while (i > 3) {
    i += 1
    if i % 2 == 0 {
        print(i)
    }
    if i == 1005 {
        break
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
answer below:

The difference in syntax between the following two while loops is that the former evaluates the condition set in the loop at the START of the loop, while the latter evaluates the condition set at the END of the loop.
Their outputs will be same because they still iterate over the same conditions.  

# Bonus =)

***
## Question 1

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

answer below:

`break` forces the compiler to leave the loop, while `continue` makes the loop begin immediately, even if there's still code to be executed remaining in the loop.
```swift

var i = 10
while (i < 19) {
    i += 1
    continue
    print (i)
}

while (i < 19) {
    i += 1
    break
}



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

[x]1
[x]2
[x]3
[]4
[]5
[]6
[]7
[x]8
[x]9
[x]10

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

[x]1
[x]2
[x]3
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
answer below:

x = 1, y = 1
x = 2, y = 1
x = 3, y = 1

The loop prints out the numbers in the outerloop range as well as the innerloop range - EXCEPT for when y = 2, this forces the for loop to start again at a new index in the range of the outerloop.  

***
## Question 5

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

answer below:

```swift

for x in 0...10 {
    for y in 0...10 {
        print( "\(x), \(y)")
    }
}

```
***
## Question 6

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

answer below:

```swift
for x in 0...10 {
    for y in 0...10 {
        if x - y >= 5 || y - x >= 5 {
            print( "\(x), \(y)")
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
answer below:

```swift
var N = 5
while i <= N {
    print (i * i)
    i += 1
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

answer below:

```swift

for _ in 1...N {
    square.append("*")
}
for _ in 1...N {
    print(square)
}

```

***
