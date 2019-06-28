# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**

var daNumbas = 0
let daRange = 1...150

for _ in daRange {
daNumbas += 1
print(daNumbas)
}


***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

var daNumbas = 0
let daRange = 142..<159

for _ in daRange {
daNumbas += 1
print(daNumbas)
}

***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

var daNumbas = 0
let daRange = 15...80

for _ in daRange {
daNumbas += 1
if daNumbas % 2 == 0 {
print(daNumbas)
}
}

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

var daNumbas = 0
let daRange = 19...51

for _ in daRange {
daNumbas += 1
if daNumbas % 2 != 0 {
print(daNumbas)
}
}

***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

var daNumbas = 0
let daRange = 7...40

for _ in daRange {
daNumbas += 1
if daNumbas % 10 == 7 {
print(daNumbas)
}
}

***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

var daNumbas = 0
let daRange = 20...150

for _ in daRange {
daNumbas += 1
if daNumbas % 3 == 0 {
print(daNumbas)
}
}

***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

var daNumbas = 0
let daRange = 20...150

for _ in daRange {
daNumbas += 1
if daNumbas % 2 == 0 && daNumbas % 3 == 0 {
print(daNumbas)
}
}

***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

var daNumbas = 0
let daRange = 20...150

for _ in daRange {
daNumbas += 1
if daNumbas % 10 == 4 {
print(daNumbas)
}
}

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

var daNumbas = 0
let daRange = 20...150

for _ in daRange {
daNumbas += 1
if (daNumbas == 31 || daNumbas == 35 || daNumbas >= 40 && daNumbas <= 60) {
print(daNumbas)
}
}

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
It will run infinite times because "i" initialize at 5 and 5 is always greater than 3

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

while (i > 3) && i < 9 {
i += 1
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

while (i > 3) && i < 1005 {
i += 1
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

while (i > 3) && i < 1005 {
i += 1
if i % 2 == 0 {
print(i)
}
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
The result is the same but the method is different due to the While function executes based on condition first and the Repeat function runs the block first then checks the condition of While.

***
## Question 16

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

Break stops the function once a condition is met whereas continue progresses the function even if the condition is met.

***
## Question 17

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
## Question 18

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
## Question 19

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
## Question 20

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

***
## Question 21

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

***
## Question 22

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
## Question 23

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
