# Entry 3
##### 2/7/26

###  Update from Blog #2

Coming back from the week-long break, I have been watching videos on Swift documentation and have learned new syntax that is extremely beneficial when writing functions or classes. Over the break, I have tinkered with the new concepts to get a better understanding and feel of conditionals. Additionally, I have been exposed to the idea of `nil`, `!`, and `?`. I look forward to continuing to watch the entirety of the [playlist of videos](https://www.youtube.com/watch?v=IG_JCxSPa_k&list=PLMRqhzcHGw1b89DXHOVA77ozWXWmuBkWX&index=45).

### Optionals

This idea contains a lot of information. Mainly, it introduces the idea of hidden values and temporary values. 

* `!` --> "Unwraps/Opens" the `?` to check whether there truly is a value or nil within the variable that has `?` attached.
* `?` --> "Wraps" a variable with a cloak; you won't know if the value is nil or a real value 
* `nil` --> Since you can't declare a variable without a value, `nil` comes in handy when declaring the datatype, for example, `var variable:String?`, allowing for flexibility and not restraining the datatype to be a string.

Below are some examples of the various types of using optionals and their flexibility when utilized. 

```JS
let x: Int = 10         // regular variable set to a value
let y: Int? = x + 5     // optional (can be nil)


// When called, returns a random integer from 1 to 10
class RandomAge {

    func age() -> Int {
        return Int.random(in: 1...10)
    }

}


// OPTIONAL (Could be a nil value or an int)
let whatAge: RandomAge? = RandomAge()



// OR (? being unknown or ! being explicit, stating that there IS an int)
let whatAge:int? (Wrapped)
let whatAge:int! (Unwrapped)



// If let checks if whatAge is nil, if not, it'll be stored within unwrappedAge.
// The code will then be run; if it is nil, it will be skipped

// OPTIONAL BINDING
if let unwrappedAge = whatAge {  
    print(unwrappedAge.age())
}


//Checks whether whatAge? is nil, if not, it'll call age(), if so, it'll get skipped
// OPTIONAL CHAINING
whatAge?.age()
```

### Thoughts

Swift to this point has certainly ramped up the complexity and difficulty of introducing a complex idea such as optionals. Still, this would supplement my learning, as well as what I would do in the future on my project. I will continue to tinker in order to retain my understanding of Swift, as well as looking upon [documentation](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/guidedtour/) to fill in the gaps in my knowledge.


### EDP (Engineer Design Process) 
Joe and I are on steps 3 and 4; as we continue to brainstorm new ideas, we are also pinning some possible and probable solutions in order to begin working on something. We have learned a lot of skills over the past year and can begin planning how our vision may start to look in the future and our project.


### Skills 

#### How to Google
With Swift still being somewhat of a novel language to me, I have googled information and guides on the side to answer little questions of mine. Rather than solely relying on Swift tutorial videos on YouTube, to get a better understanding of Swift, I have googled various documentation and the experiences others had in order to get a better understanding of my coding language. Furthermore, questions that involved concepts outside of Swift, such as collaboration and add-ons, are not included in the Swift tutorials I watched, which further necessitates the need to responsably google information I don't know.

#### How to read
This skill directly ties into the previous skill, yet also differs in its unique way. Throughout all the googling and documentations, the need to read properly became a cornerstone of how I understood Swift as a language. To add on, the skill of reading extended more in my understanding of Swift more than simply reading documentation, but also coherently reading the code. Without training my ability to read properly, I would've fallen behind and simply not have equipped myself with the necessary tools to learn a new language.  

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
