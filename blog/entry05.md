# Entry 5
##### 4/18/26

### Update from Blog 4
Having honed in on the interactive aspect of Swift, I sought to combine a button with a shape that would disappear as the user clicked on it, as a game. With my direction set, I first wanted to put that aside and  follow step by step a video on how to create a [card matching minigame](https://drive.google.com/file/d/1lEL9fTAbKJznsanTHrcyeM5_-VdvgND_/view) so that it could be integrated into the bigger system. After that was out of the way, I sought to create my clicking minigame. The first step was to combine a button with a shape, which was quite simple to do at first.

```Swift
Button(action: { print("Tapped!") }) {
    Circle()
        .fill(Color.blue)
        .frame(width: 50, height: 50)
}
```
With this, I took one step in the direction of completing my minigame. The next step was to have the button move when clicked to simulate a game that counted the number of circles you could click to reach a high score. To do this, I would need variables that held the new coordinates of the circle each time it was clicked on, as well as a function that could detect a user's input and run code to move the circle when clicked on. To achieve this, I needed to understand `.onTapGesture`, `.position()`, and the method to declare a global variable that could be accessed whenever. Watching a [video](https://www.youtube.com/watch?v=joUjsvWn2Eg) helped visualize everything.

```Swift
  @State private var newX: CGFloat = 150 //start x position 
  @State private var newY: CGFloat = 300 //start x position

  var body: some View {
      Circle()
          .fill(.blue)
          .frame(width: 80, height: 80)
          .position(x: x, y: y)
          .onTapGesture {
              x = .random(in: 50...300)
              y = .random(in: 50...600)
          }
  }
```

To continue, I wanted to add a countdown timer, which I had no clue how to implement. While researching this issue, I stumbled across a video demonstrating how a [simple countdown timer](https://www.youtube.com/watch?v=kIaO4UtzBHIhttps://www.youtube.com/watch?v=kIaO4UtzBHI) could be made, and so I liberally applied it to my project. 

```Swift
@State private var time = 30
@State var timerRunning = true

let timer = Timer.publish(every: 1, on: .main, in: .common).autoconnect()

Text("Time: \(time)")
    .onReceive(timer) { _ in
        if time > 0 && timerRunning {
            time -= 1
        }
    }

```
Each part of the countdown serves a unique purpose. To start, the clock needs to start at a time, so the predetermined time in this clock will be 30 seconds and will run if the code is written correctly. The timer is then set as a variable, as we will actively manipulate its value. Timer.publish() is a built-in method that creates a clock that can be connected and changed dynamically. The parameters in parentheses specify the time and location of the clock. `.autoconnect()` allows the clock to begin ticking; without it, you would need to tell it to tick manually. `.onRecieve()` specifies that when it gets a signal every second, it would deduct a second from the timer when it clears the conditions.

Having completed the framework of the game already, I sought to start everything with the click of a button so that this game could be easily integrated with other minigames. To do this, I went back to buttons and functions. By declaring some variables false at the beginning, I made it so that only when you clicked the button, the game would appear and run. 

```Swift

@State var gameStart = false

if !gameStart{
    Button(action: {
        startGame(in: geo.size)
    }){
        Text(time == 0 ? "Play Again" : "Start Game")
        //checks if time is 0 and if so, print the first string, if not, the other  
    }

func startGame(in size: CGSize) {
            score = 0
            time = 30
            gameStart = true
            timerRunning = true
            moveCircle(in: size)
        }
        
        func moveCircle(in size: CGSize) {
            newX = .random(in: 0...(size.width - 80))
            newY = .random(in: 0...(size.height - 80))
        }
```

### Thoughts
I made it so that when you clicked the start button, all the parameters would be set to their correct values and, therefore, allow the game to run smoothly. Additionally, when writing this code, I learned of the Ternary Operator, which was a shortcut for an if-else statement. `Text(time == 0 ? "Play Again" : "Start Game")` would essentially check if time was 0 and if so print "Play Again" and if not, "Start Game". Coding with Swift has shown me so many possibilities with a different language. 

### Engineer Design Process (EDP) 
At the current stage of our project, we are in the final stages of 7 and 8. We have created and tested the MVP and are moving on to the stages of improving it and possibly adding newer features to dynamically improve our game. Additionally, we can also start reflecting on what went smoothly and what was rough to further deepen our understanding.

### Skills

#### Creativity
Throughout this project, I had to harness my creativity when thinking of ways to create a unique game with my limited knowledge. Starting from the tinkering to one of my creations of a game, the creative process has revealed the handiness of being able to connect ideas and formulate new thoughts, just like how I sought to combine a shape with a button, and use buttons to create my entire homescreen menu. To add on, creativity was crucial when supporting Joe in integrating both our projects together to create something functional. 

#### Problem Decomposition
In my process of creating a game, I ran into countless walls, stopping because of various errors. By pinpointing where the errors occurred, I repeatedly broke my code apart to understand the issue so that it could be solved. In the creation of the game, it didn't come together in one piece smoothly, as evidenced by what I said earlier, making the button was the first step when decomposing how I could make this game. From the creation of the various buttons to the functions used to start the game, they were written with the ability to decompose a big problem into a multitude of smaller ones to solve.  

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
