# Entry 4
##### 3/14/26

### Continuation after blog 3

Having now finished the Swift beginner's tutorial playlist on YouTube, I now have a better understanding of how Swift works and the type of language it is. Now my goal is to impart that knowledge when writing about Xcode. Having recently acquired a MacBook, I can write Swift and retroactively see the result of what I wrote. Now I have to collaborate with Joe to finally create something that would be akin to our final project. I am going to focus on trying to acomplish what was written out in our plan so that we can finish in a timely manner.

### New Syntax

* Arrays --> A way to store data by collecting data of one type. 
* Dictionaries --> A method of storing data by giving definitions a key. 
* Numerous built-in methods can be used on arrays, such as: `.count`; `.append`; `.insert`; `.remove(at: int)`; `.firstIndex(of: String)`; `.lastIndex(of: String)`; `.first`; `.last`.

```JS
*Arrays*

//initialize the array
var fruits:[String] = ["apple", "pears", "berries"]

//adds "dates" at index 1
fruits.insert("dates", at: 1)

//this adds "grapes" to the end of the array
fruits += ["grapes"]

//prints out everything
print(fruits)
print("In total I have \(fruits.count) fruits")


*Dictionaries*

//declare dictionary
var dictionary = [String:String]()

//declares and assigns keys with its value
dictionary["Period 1"] = "English"
dictionary["Period 2"] = "Economics"

//tie keys to variables for ease of access
var p1 = dictionary["Period 1"]
var p2 = dictionary["Period 2"]

//directly changing a value
dictionary["Period 2"] = "APCSA"

//print one specific key
print(p1) //"Optional("English") --> Optional because it could be empty or a value

//loops through the keys and prints out the values
for (key, value) in dictionary {
    print("\(key) is \(value)")
}
    }
}
//Prints
//Period 1 is English
//Period 2 is APCSA
```

### Comments 
The various ways of data storage allow for numerous possibilities of how we can sort user input and utilize said information. However, although I may have understood some fundamentals, Swift apps require more than just code and require the designing of the UI, which I still need to learn about, and how code interacts with the interface to create a pleasing interface for users. Having recently acquired my Mac, I will work towards tinkering around with the UI while asking Joe to collaborate and create a functioning first game.

### EDP (Engineer Design Process)
Currently, as we have all the necessary tools to begin creating a game, we are on steps 4 and 5: actually creating and implementing what we have learned and planned out. Creating the prototype would mean having created the interface (what the user sees) and the user experience (how interactions go), which would place us somewhere in between as we start working towards that goal collaboratively.

### Skills

#### Embracing Failure
Recently, everything seems to be off course, and nothing makes sense, which has led me to consistent failures. The pressure seems to have increased, and time seems scarce, but I didn't let that stop me. Although I felt significantly set back from the constant failures, rather than seeing that as the end, I viewed those errors and mistakes as an opportunity to grow. I have realized that rarely anything goes as you want without significant work poured into the outcome, which is how I have been honing this skill. I learned that although failure might hurt in the moment, when you review and grow from your mistakes, it feels exponentially fulfilling, which helps me strive to continue to grow, despite my failures and mistakes.

#### Growth Mindset
My mindset has shifted numerous times due to my experiences working on the project and even while doing homework. Similarly connected, embracing failure, the growth mindset allowed me to reach out for help without any shame. By understanding that simple point, I was able to continue to grow despite the setbacks each time. I have acknowledged that, rather than trying to rush my learning, sometimes it takes time to process and to understand what I am looking at. The persistence and efforts in trying to learn are what have shaped my understanding of the language. Rather than giving up after reaching an obstacle, I strive to patiently understand the problem and to review and look back when I don't understand 

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
