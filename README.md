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

for i in 0...150 {
    print(i)
}


***

## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

for num in 142..<159 {
    print(num)
}
***

## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

for num in 15...80 where num % 2 == 0 {
    print(num)
}

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

***
for num in 19..<15 where num % 2 == 1 {
    print(num)
}
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

***
for num in 5..<100 where num % 10 == 5 {
    print(num)
}
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

for num in 1...40 {
if num % 10 == 7 {
    print(num)
  }
  }

***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

***
for num in 20...150 where num % 3 == 0 {
    print(num)
}
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

***
for num in 20...150 where num % 3 & num % 2 == 0 {
    print(num)
}
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

***
for num in 20...50 {
if num % 10 == 4 {
    print(num)
  }
  }
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

***
flet num = 20...150
for number in num {
    switch number {
    case 40...60:
        print(number)
        fallthrough
    case 31:
        print(number)
    case 35:
        print(number)
    default:
        print( )
    }
}
## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

// Your explanation here
```
WHEN YOU PUT += 1 IT MEANS YOU ADD 1 TO ALL VARIABLE i WHICH IS INFINITE & over 3
***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```

var i = 5
while (i < 10) {
    i += 1
    print(i)
    }
    
***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```

var i = 5
for _ in 1...1000 {
print(i)
}
***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
var i = 5
for _ in 1...1000 {
print(i % 2 ==0 )
}
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
loop one is using a while loop and loop two is using a REPEAT WHILE loop. They will both run the same in this case because they are BOTH LOOPING within the code. 
# Bonus =)

***
## Question 1

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

***
break stops the loop and gets out of the scope entirely and continue will just move on to the next case. 

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

[]1 yes
[]2 yes 
[]3 yes
[]4 no
[]5 no 
[]6 no
[]7 no
[]8 yes
[]9 yes
[]10 yes

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
the same as question 2 above
[]1 yes
[]2yes
[]3yes
[]4no
[]5no
[]6no
[]7no
[]8yes
[]9yes
[]10yes

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
