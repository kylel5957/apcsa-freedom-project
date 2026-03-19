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

<img width="304" height="139" alt="image" src="https://github.com/user-attachments/assets/6d385a8b-f201-4ad0-8469-7c65d1f37cc1" />

Here, I had changed some numbers so that the loop starts at 0 and ends at 5. I changed the variable being printed to the loop so that it would print each stage it was on. I was expecting that it would only print up to 4 because, without specifying, I thought that the loop would be exclusive.

<img width="391" height="143" alt="image" src="https://github.com/user-attachments/assets/fc9e5a7d-2f9f-471a-9192-5ea15f6542b4" />

However, contrary to my belief, the loop was inclusive. Having set the loop from 0-5, I thought it would've run like it was 0<5, but it was not true. The loop ran inclusively, which meant 0<=,5 which was why it had printed everything from 0-5.
This is important to remember because it means that we always need to tailor our loops inclusively and not exclusively. Additionally, when utilizing loops, it would come in handy and make the process easier to understand with the numbers you input.

#### Next Steps
To keep the momentum going and keep on learning Swift, not to fall behind, and keep on learning new concepts to utilize for the project.



## Learning Log 6 
### 12/10/25

* In [this](https://www.youtube.com/watch?v=36ipzqIQKIk&list=PLMRqhzcHGw1b89DXHOVA77ozWXWmuBkWX&index=7) video, he continues to expand on while loops and their functionality.
* I learned that there is a different type of while loop, which is the "Repeat Loop". What's different is that instead of the usual structure of while which looks like

```JS
while condition {
    some code
}
```

* The loop runs when the condition is true; the repeat loop flips it on its head. With the structure like

```JS
repeat {
    some code 
} while condition
```

* Now the difference in this code is that the repeat loop ensures that the loop will run at least once before checking the condition to run again, eliminating the need for external code to just repeat what the while loop would need.

<img width="421" height="196" alt="image" src="https://github.com/user-attachments/assets/8be7c912-01fa-4387-bc77-a4f37dd00ef4" />
<img width="387" height="70" alt="image" src="https://github.com/user-attachments/assets/99bd5683-7d73-42b7-bb93-a23c710c2546" />

* Here, I declared an integer set to 1 and then set up two loops. In the results below, only "Number is greater than 1" is printed because, even though both CONDITIONS are wrong, the repeat loop ensures the code inside runs at least once, eliminating extra code that would've been needed. 

* Now I also watched another [video](https://www.youtube.com/watch?v=CLmZxVkN9gw&list=PLMRqhzcHGw1b89DXHOVA77ozWXWmuBkWX&index=8) on functions, and they are extremely similar to JS functions in their structure.
* Here I learned about functions and their structure, which is parallel to JS.

```JS
func name() {
    some code
}

name()
```

* This allows you to bunch code together so that they can all be executed in one line repeatedly.
* Below I have created a function and called it so that it would print whatever was in the function

<img width="302" height="159" alt="image" src="https://github.com/user-attachments/assets/a179f867-a23b-4a56-b6cc-6c032fc9ff15" />
<img width="363" height="55" alt="image" src="https://github.com/user-attachments/assets/3ce0c4ac-75cc-4151-a521-b5a6ff5dfabd" />

* Utilizing functions would allow me to significantly cut down the code I would need to write for repeated actions

#### Follow Up 
* I would like to continue to learn more concepts and continue to work alongside Joe to improve our knowledge of Swift so that we can finally start working on our end goal.
  


# Leaning Log 7
## 1/9/26

* From the videos about [optionals](https://www.youtube.com/watch?v=IG_JCxSPa_k&list=PLMRqhzcHGw1b89DXHOVA77ozWXWmuBkWX&index=14), I learn about the utility of the `?` and `nil` value, which can be excellent placeholders.
* When declaring a variable, the option to have it with no value is not allowed, while the placeholder `nil` works, it would then make the variable assigned to it unable to be properly used; additionally, the datatype needs to be explicitly stated, which then further narrows your options.
* However, to utilize the "optional", such as in a conditional statement, you must first "unwrap" the optional (the "?") by using the ("!"), the unwrapper.

* Part of the optional family would be optional binding and optional chaining, whose syntax is similar to optionals.

```JS
let x: Int = 10         // regular variable set to a value
let y: Int? = x + 5     // optional (can be nil)


class RandomAge {

    func age() -> Int {
        return Int.random(in: 1...10)
    }

}


// OPTIONAL
let whatAge: RandomAge? = RandomAge()

// OR
let whatAge:int? (Wrapped)
let whatAge:int! (Unwrapped)


// OPTIONAL BINDING
if let unwrappedAge = whatAge {
    print(unwrappedAge.age())
}


// OPTIONAL CHAINING
whatAge?.age()


// The if statement first checks if the optional is not nil,
// then assigns the unwrapped value and runs the function.
```

* Swift is a type-safe language, meaning that each syntax must be specific and won't run until errors are all cleared.
* Optionals exist to prevent common data mistakes and allow for empty variables without explicitly setting a value.
* The difference between `let whatAge:int?` and `let whatAge:int!` is that the one that's wrapped would bring up safety checks and ensure it's used correctly, while the unwrapped one doesn't.

<img width="392" height="287" alt="image" src="https://github.com/user-attachments/assets/142892a2-3887-4361-8b16-49235af6387f" />

<img width="425" height="103" alt="image" src="https://github.com/user-attachments/assets/ac437c3c-d8c3-49c7-ab36-e181a605b810" />

* Here in my codespace, I show how in my function that returns a number from 1 to 10, I declare "whatAge" as an optional, with it possibly being a nil value or calling the class.
* Then, in the next line, I made it so that if the optional does have a value rather than nil, it would declare a variable, setting it to the value the function returns and printing it out.
* In the running of the code, there was a value, and it wasn't nil, so the function returns "5".

### Follow Up 

* In the following learning logs, I hope to continue to understand how to utilize the different syntax in unique ways to create a good product. This lesson was dense with the idea of optionals being foreign, and I will continue to practice and do my best to understand it.



# Learning Log 8 
## 3/8/26

* The swift [beginner playlist](https://www.youtube.com/watch?v=rNyTxjGSp8Q&list=PLMRqhzcHGw1b89DXHOVA77ozWXWmuBkWX&index=17) now focuses its attention on explaining collection types. Here, I learn about arrays and dictionaries.
* To simplify, arrays in Swift are similar to arrays in Java; however, Swift's arrays are dynamic, and that means they are changeable in size. They also share the same property that they cannot mix data types, and only return the data type you set the array as.
* There are numerous built-in methods that can be used on arrays, such as: `.count`; `.append`; `.insert`; `.remove(at: int)`; `.firstIndex(of: String)`; `.lastIndex(of: String)`; `.first`; `.last`.
* The methods are very intuitive and work as they seem, returning the first, last, or any specific element. Swift also runs on 0-index counting, so it's important to consider that when counting and utilizing the numbers.
* Dictionaries are what they sound like. In Swift, you create them using `var name = [dataType:dataType]()` by first creating "keys", and you can assign them values, which then can be referred back to or utilized in various ways.
* Additionally, when looping through a dictionary, you can use something called a tuple, "a comma-seperated list of types, enclosed in parenthesis"
* To print integer values from a result alongside a string is done by using String Interpolation. `("Hello I am \age years old")`
  
```JS
//initialize the array
var fruits:[String] = ["apple", "pears", "berries"]

//adds "dates" at index 1
fruits.insert("dates", at: 1)

//this adds "grapes" to the end of the array
fruits += ["grapes"]

//calls array
print(fruits)
print("In total I have \(fruits.count) fruits")

// PRINTS 
// ["apple", "dates", "pears", "berries", "grapes"]
// In total I have 5 fruits
```
<img width="488" height="475" alt="image" src="https://github.com/user-attachments/assets/988aa123-cbe8-4575-9481-e8798fde3cf6" />

<img width="203" height="69" alt="image" src="https://github.com/user-attachments/assets/1bc4a8f4-0f01-489a-b983-6428acd83fbc" />


* The results are exactly what is to be expected, and this would be extremely beneficial whether I am collecting data or creating secret code games.
* Each line is roughly explained, and the syntax isn't that difficult to understand

### Next Steps
* My next step would now be to get a Mac, which I already am in the process of doing. By achieving this step, I can further collaborate with Joe on the creation of the game.
* Since this is also the last topic of the videos, I am going to continue to look for online resources to keep on learning how to write Swift in a beneficial manner.


# Learning Log 9 
## 3/19/26

* Moving on to learning more about app creation, the first step is to understand how the UI works and how I could design it to be appealing and operational.
* I began this first step by watching [a tutorial](https://www.youtube.com/watch?v=Ys59M1qFAfo) on how to do so by understanding the whole process broken down.
* Views are what the users see, and the modifiers are what are applied to the views to change their look and feel. Finally, the container is what dictates placement and how everything is organized.
* The first simple step is to import an image, which would be uploaded to the assets folder after creating a project on Xcode.
* After, inside the body, you can use `Image("image-name")` to display the image on the screen.
* At first, the image would cover the entire screen, so to get around that, you use `.resizable() and .aspectRatio(contentMode: .fit)`
* Additionally, there are various ways to change the image, such as `.cornerRadius(int)`. It is also easy to look through the library, which lists all the different views and modifiers available for use.

```JS

import SwiftUI

struct ContentView: View {
    var body: some View {
        Image("Rice")
            .resizable()
            .aspectRatio(contentMode: .fit)
            .cornerRadius(20)
    }
}

struct ContentView_Previews: PreviewProvider {
    static var previews: some View {
        ContentView()
    }
}

```

<img width="300" height="650" alt="image" src="https://github.com/user-attachments/assets/cb8ce35e-1306-4451-8112-bd52bd84d409" /><img width="300" height="650" alt="image" src="https://github.com/user-attachments/assets/fa802f55-6a5e-4676-81d7-721e4cb2ff81" />

* The images appeared as they should with the image fitting on the screen rather than being incredibly zoomed in.

### Next Steps 
* My next steps are to continue navigating Xcode and possibly understand how to write more behind-the-scenes things that would make the page more interactive
* Additionally, I want to learn how to set a background image and buttons.
