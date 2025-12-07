# Tool Learning Log

## Tool: **Swift**

## Project: **Freedom Project**

---
## Learning Log 1
### 9/30/25:
* Looking at the swift documentation, I downloaded Swift and VS50 code
* Looked at the [swift documentation](https://www.swift.org/documentation/) and see how it's written and utilized
* I then created a file and named it myProject.swift with the `.swift` being extremely important for the file to run
* As I initiated everything, I started with a string of code to see how it worked.

* For my first code, I wanted a simple print and so I typed in `print("Hello World");`
* I also tried using different strings and concatenations

* I also declared variables and used those to combine with other to create longer texts
* As they both fundementally are the same but take on different approaches, it felt familiar but also different

* `var greet = "Hello World"`
* `var time = ",morning!"`
* `print(greet + time)`
* That print would result in "Hello World, morning!"

* For next week I plan to watch some videos and look more through the documentation to learn more about swift


## Learning Log 2
### 10/27/25
* Watching [Swift Tutorials](https://www.youtube.com/watch?v=zcLMOTEDd8Y&list=PLMRqhzcHGw1b89DXHOVA77ozWXWmuBkWX&index=2), I have learned more about swift and it's uniqueness
* By appending `:String` to something like `var firstName = "Tom` to create `var firstName:String = "Tom`, you can restrict the data intake to only be strings
* Alongside `:String`, there are also `:Float`, `:Double`, and `:Bool`, which all tell you the exact data type stored in a variable
* Though not necessary, it's beneficial for clarity and visibility, showing clear intent on the data type you want to take in, which can prove useful when debugging
* The most efficient way for me to run the code after all my changes would be to press run the project, then type `swift run`
<img width="389" height="58" alt="image" src="https://github.com/user-attachments/assets/49dd95d9-8df5-423e-8a95-14ac4317c0b6" />

* The parallels between Swift and Java seemed to show with declaring variables and now conditionals

#### If Statements
* The if statements in Swift are the same as Java, just without the parentheses around the condition
```JS
let name: String = "Goodbye!"
let decision: Bool = true
let num3: Double = 32.23
let num2: Int = 24

if num2 > 23{
    print("Thats bigger than 23!")
}

if num3 > 23.22{
    print("Thats a big number!")
}

if decision == false {
    print("It's false")
}
else if name == "Goodbye!"{
    print("Adios!")
}
else {
    print("The end")
}
```

* This conditional would print
<img width="370" height="119" alt="image" src="https://github.com/user-attachments/assets/93b40092-dad5-49b0-b134-fcda6f0fa534" />

* The results printing "Thats bigger than 23!" is correct and works as intended
* It moves onto the next condition of `num3 > 23.22` which correctly prints `"Thats a big number!"`
* Next, it goes onto the conditional chain, which correctly deems the first conditional as wrong and prints `"Adios!"` because of the second conditional being true.
* The difference here is that in Swift, you *can directly check* if the string is equal to a variable, unlike Java.

### Next Steps
* I will aim to continue to learn more about Swift and how to properly utilize it's features to create a functioning project

## Learning Log 3
### 11/14/25

* From what I've [watched](https://www.youtube.com/watch?v=R4U42rkmHDk&list=PLMRqhzcHGw1b89DXHOVA77ozWXWmuBkWX&index=5), I now understand how the new concept `switch` works in Swift
* `switch` allows you to run through various conditions on one specific variable, clearing the syntax and allowing for more concise code
* `switch` works with various data types such as: `int, double, char, string, bool`, and more
* The syntax of switch is similar to `if statements`, and they go as follows

```JS

switch 'variable' {

case condition1:
    print(anything)
case condition2, condition3:
    print(anything)
default:
    print(anything)

}

//example with int below

int a = 3
switch a {
case 1:
    print("The number is 1")
case 2, 3:
    print("The number is 2 or 3")
default:
    print("It's not 1, 2, or 3")
}

// ^ prints "The number is 2 or 3"
```

* Switch allows for multiple conditions on one line or different conditions on different lines, just like an if statement chain.
* `case` signifies the start of a new condition, while `default` works as an else statement, printing if none of the conditions are met.

* 

<img width="593" height="289" alt="image" src="https://github.com/user-attachments/assets/b5af6363-43fe-4121-9a38-a7c13db336c9" />
<img width="428" height="116" alt="image" src="https://github.com/user-attachments/assets/cd51597c-5735-4214-8ac8-4818e96bafa8" />

* It prints out `"The string is Hello or World"`, which, as the variable shows, is true
* Having followed step by step, it's clear how convenient this feature is. Being able to work with various data types eliminates the need for unnecessarily long if-conditional chains.
* This feature can be especially useful when looking for specific phrases or numbers, making the syntax and readability simpler for longer conditions

#### Next Steps
I want to start merging my understanding of Swift with Joe so that we both are on track and can build off each other's understanding of Swift's features.


## Learning Log 5 
### 12/1/25

* From [the continuation](https://www.youtube.com/watch?v=KV7Ts9sm850&list=PLMRqhzcHGw1b89DXHOVA77ozWXWmuBkWX&index=6) of the previous playlist, CodeWithChris continues to break down each concept of Swift.
* This video talks about loops, this time they are completely different from anything I've seen before, the structure is similar yet different.
* The loop structure is as follows

```JS
for varName in lowerValue...higherValue{
    code 
}
```
I had decided to implement something similar while following the tutorial, and wondered if the interactions within and outside the loop would stay the same as the other loops.

<img width="342" height="173" alt="image" src="https://github.com/user-attachments/assets/b3ee58eb-fc9d-48c4-bbe5-38e70bff3829" />

Here, I declared an integer, independent from everything. In the loop, I made it so that with each iteration, it would save the current value and add the iteration number. With each loop run, it would also print the current value, which can be seen below.

<img width="387" height="89" alt="image" src="https://github.com/user-attachments/assets/955c68ed-9fea-4264-9787-6987463f6366" />

Here it prints `1, 3, and 6`, which makes sense. With the value starting at 1, the following 1+2=3, and finally the 3+3=6. For my next test, I wanted to make it more apparent how the loops run without any external variables involved. So after this test, I removed the concatenation and kept the print command inside while changing what it printed.

