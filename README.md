# Types Variables Logic and Operations Lab 2

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

You are given three grades obtained by 3 students, which are stored in variables `grade1`, `grade2`, `grade3` and all of type `Double`.
Create a variable called `yourGrade` of type `Double` and give it a value.
Print `"above average"` if your grade is greater than the class average or `"below average"` otherwise.

```swift
var grade1 = 7.0
var grade2 = 9.0
var grade3 = 5.0

__________________

var classAverage = (grade1 + grade2 + grade3)/3

var yourGrade = 6.6

print("The class average is", classAverage)
if yourGrade > classAverage {
    print("Your grade is above average")
} else{
    print("Your grade is below average")
}

***
## Question 2

You are given a number. Print even if the number is even or odd otherwise.

```swift
let number = 2

_________
var evenNumber = number % 2 == 0

if evenNumber == true {
    print("This number is even")
} else{
    print("This number is odd")
}

```

***
## Question 3

You are given two numbers `a` and `b`. Print `"divisible"` if `a` is divisible by `b` and `"not divisible"` otherwise.

```swift
var a = 12
var b = 3

_________

if a % b == 0 {
print("divisible")
} else {
print("not divisible")
}
```

***
## Question 4

You are given three variables `a`, `b` and `c`. Check if at least two variables have the same value. If that is true, print `"At least two variables have the same value"` otherwise print `"All the values are different"`.

```swift
var a = 2
var b = 3
var c = 2
___________

if a == b || b == c || a == c{
    print("At least two variables have the same value")
} else{
    print("All the values are different")
}

```

***
## Question 5

You are working on a smart-fridge. The smart-fridge knows how old the eggs and bacon in it are. You know that eggs spoil after 3 weeks (21 days) and bacon after one week (7 days). Given `baconAge` and `eggsAge` (both in days) determine if you can cook bacon and eggs, or which ingredients you need to throw out. If you can cook bacon and eggs, print `"you can cook bacon and eggs"`. If you need to throw out any ingredients, for each one print a line with the text `"throw out"` + bacon or eggs.

```swift


var baconAge = 7 // the bacon is 6 days old
var eggsAge = 21 // eggs are 12 days old
___________
var baconExpire = 7
var eggsExpire = 21


if (baconAge <= baconExpire) && (eggsAge <= eggsExpire){
    print("You can cook bacon and eggs")
}
if (baconAge <= baconExpire) && (eggsAge > eggsExpire ){
    print("Throw out eggs")
}
if (baconAge > baconExpire) && (eggsAge <= eggsExpire ){
    print("Throw out bacon")
}
if (baconAge > baconExpire) && (eggsAge > eggsExpire){
    print("Throw out both eggs and bacon")
}

```

***
## Question 6

You are given a year, determine if it’s a leap year. A leap year is a year containing an extra day. It has 366 days instead of the normal 365 days. The extra day is added in February, which has 29 days instead of the normal 28 days. Leap years occur every 4 years. 2012 was a leap year and 2016 will also be a leap year.
The above rule is valid except that every 100 years special rules apply. Years that are divisible by 100 are not leap years if they are not also divisible by 400. For example 1900 was not a leap year, but 2000 was. Print `"Leap year!"` or `"Not a leap year!"` depending on the year you are provided.

```swift
let year = 2014

_________
let year = 2014

if year % 400 == 0 {
    print ("leap year")
} else if year % 100 == 0 {
    print ("Not a leap year")
} else if year % 4 == 0 {
    print ("Leap year")
} else {
    print ("Not a leap year")```

***
## Question 7

If you use `random()` it will give you a random number within a specified range. Generate a random number and use it to simulate a coin toss. Print `"heads"` or `"tails"`.

```swift
let randomNum = Int.random(in: 0...100)

_____________

if randomNum % 2 == 0 {
    print("Heads")
} else{
    print("Tails")
}

Hint: use an if/else block along with the `%` operator

***
## Question 8

You are given four variables `a`, `b`, `c` and `d`. Print the value of the smallest one.

```swift
var a = 5
var b = 6
var c = 3
var d = 4
______________

var smallestVar = a

if b < smallestVar{
smallestVar = b
}
if c < smallestVar{
smallestVar = c
}
if d < smallestVar{
smallestVar = d
}

```

***
