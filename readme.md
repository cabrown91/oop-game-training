Alicia Brown
<br>[Original Repo](https://github.com/sf-wdi-31/oop-game-training)

The training was good. I appreciate doing some planning and thinking before jumping into coding the game. I can use this to structure my code for the game.


#Model a Racing Game with OOP


### User Stories & Game Mechanics
1. A user can see a track with two game pieces on it (cars).
2. A user can press a key to move a car across the track.
3. If the user moves their car across the track faster than the other car, they've won the race.
4. A user can reset the game to start over.

### Data Structures for "Racing Game"

**Car**
  - `carImage` (string)
  - `Car` (Function - constructor)

**Game**
  - `moveCar()` (Function - moves the car on keypress)
  - `reset()` (Function - resets the game!)
  - `Game(numCars)` (Function - constructor)
  - `hasWon()` (Function - check if the game has been won!)
  - `celebrate()` (Function - display a win message)

### Development Stories

1. A user can see a track with two game pieces on it (cars).
  * Create HTML structure to display at least two `Cars` on screen (Handlebars?).
  * `Game(numCars)` allows a user to specify how many cars will be racing in the race, and a keypress value will be assigned for each car to move in the game.


2.  A user can press a key to move a car across the track.
  * Add keypress event listener to cars that:
     - moves the cars across the track (`moveCar`)
     - detects where each car is located on the page/track
     - checks if the car has cross the finish line

3. If the user moves their car across the track faster than the other car, they've won the race.
  * Assuming `hasWon()` gave false for both cars:
    - keypress continues to allow the cars to move across their respective tracks
  * Assuming `hasWon()` gave true for one car:
    - the game is over, and a player has won
      * If so, show a win screen (`celebrate`)

4. A user can reset the game to start over.
    - once a winner has been determined, a user can click a `reset()` button to start a new race


###Potential Challenges / Development Questions

1. How to detect the location of each car on it's respective track (margin?, window position?)
2. Can more than one player win?
3. Cool car movement animation?
4. Set up a win counter?
