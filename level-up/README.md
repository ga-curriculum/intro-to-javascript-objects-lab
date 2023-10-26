# ![Intro to JavaScript Objects Lab - Level Up](./assets/hero.png)

### Exercise 18

```javascript
/*
Add a new property to the `game` object called `collection` and initialize its
value to an empty array.

Copy the `catchPokemon` method that you wrote in Exercise Twelve, and paste 
it below. Modify it so that:
- Ensure that no more than six pokemon can be in the party at any given time. 
  Excess pokemon should be placed in the `game.collection` array.
- It's up to you how to distribute pokemon in a situation where more than six 
  would be placed into the `game.party` array.

Again, for the purposes of this exercise, it's ok to have a negative number of pokeballs.

After updating the method, make use of it by calling it and passing in a 
pokemon object of your choice from the `pokemon` data to catch it.

Also, log the `game.items` array to confirm that the pokeball quantity is being decremented.

Solve Exercise Eighteen here:
*/


```

### Exercise 19

```javascript
/*
Copy the `catchPokemon` method that you just wrote above, and paste it below.
The time has come to make it so that we cannot catch a pokemon when we do not 
have any pokeballs to catch it with. 

Modify the method so that if there are no pokeballs a message will be 
displayed that there are not enough pokeballs to catch the desired pokemon.
Also ensure that the pokemon isn't added to the `game.party` or the 
`game.collection`.

Solve Exercise Nineteen here:
*/

```

### Exercise 20

```javascript
/*
Copy the `catchPokemon` method that you just wrote above, and paste it below.
Modify is so that you can just pass in the name of a pokemon instead of an 
entire object and the method will look up the pokemon from the data set for you.

The string that is passed in should be allowed to be any case (for example if 
the string 'PiKacHU' is passed to the function it should match to 'Pikachu' in
the data set). 

If there is not a match then return a string noting that the selected pokemon
does not exist. Ensure you do not decrement the pokeball count if an invalid
pokemon name is passed in, and also ensure that the pokemon isn't added to the
`game.party` or the `game.collection`.

Solve Exercise Twenty here:
*/

```

### Exercise 21

```javascript
/*
Dynamically construct an object with the existing `pokemon` data sorted by the 
different pokemon types. The object will have this structure:

{
  grass: [
    { number: 1, name: 'Bulbasaur', type: 'grass', hp: 45, starter: true },
    { number: 2, name: 'Ivysaur', type: 'grass', hp: 60, starter: false },
    { number: 3, name: 'Venusaur', type: 'grass', hp: 80,starter: false },
    * more grass type pokemon objects...
  ],
  fire: [
    { number: 4, name: 'Charmander', type: 'fire', hp: 39, starter: true },
    * more fire type pokemon objects...
  ],
  water: [
    * water type pokemon objects...
  ],
  * etc... until there is an array for every pokemon type!
}

Log the object when it's constructed.

Solve Exercise Twenty-One here:
*/

```
