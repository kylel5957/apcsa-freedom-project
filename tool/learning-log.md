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

