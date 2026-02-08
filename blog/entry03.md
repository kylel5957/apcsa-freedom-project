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


[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
