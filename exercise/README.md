# ![Intro to JavaScript Objects Lab - Lab Exercise](./assets/hero.png)

## Introduction

This lab provides an opportunity to practice defining, accessing, and manipulating objects.

### A quick note before you dive in
Don't hesitate to collaborate with your classmates when working through labs.

If you get stuck during the lab, we recommend revisiting the lesson materials first. They're designed to provide you with the information and examples that will help you complete the exercises.

## Lab Exercises

First, copy and paste the following `game` object into `app.js`:

```javascript
const game = {
  party: [],
  gyms: [
    { location: "Pewter City", completed: false, difficulty: 1 },
    { location: "Cerulean City", completed: false, difficulty: 2 },
    { location: "Vermilion City", completed: false, difficulty: 3 },
    { location: "Celadon City", completed: false, difficulty: 4 },
    { location: "Fuchsia City", completed: false, difficulty: 5 },
    { location: "Saffron City", completed: false, difficulty: 6 },
    { location: "Cinnabar Island", completed: false, difficulty: 7 },
    { location: "Viridian City", completed: false, difficulty: 8 },
  ],
  items: [
    { name: "potion", quantity: 4 },
    { name: "pokeball", quantity: 8 },
    { name: "rare candy", quantity: 99 },
  ],
}
```

Copy and paste each of the following exercises into your JavaScript file. To check your work, open the file in a web browser and inspect the console output, or run the file in your terminal using `node app.js`.

### Exercise 1

Spend some time inspecting the `pokemon` array by running the following command:

```javascript
console.dir(pokemon, { maxArrayLength: null })
```

You have not seen this console method before, but we're using it here so that you're able to see all of the pokemon in the console. By default, `console.dir` and `console.log` display only the first 100 items in an array.  `{ maxArrayLength: null }` will tell `console.dir` to display all items in the array.  This option is not available to `console.log`, which is why we need to use `console.dir`

Take note of the shape of the data here. Each pokemon object in the array has:

- a number, which is a number between 1 and 151
- a name, which is a string
- a type, which is a string
- hp (hit points), which is a number
- a starter boolean.

There's some game-specific terminology here, so if you've never played pokemon here's a quick primer on what these mean:

- All pokemon have a number that acts as a unique identifier
- All pokemon have a type that indicates their primary abilities. Pokemon generally have multiple types, but we're only using a pokemon's primary type here to make working with this data more manageable.
- All pokemon have hit points - essentially a quantitative measure of a pokemon's health.
- At the start of a game, a player must select a starting pokemon. Acceptable starting pokemon objects will have a starter property with a value set to true. Four pokemon fit this criterion:
  - Pokemon 1: Bulbasaur
  - Pokemon 4: Charmander
  - Pokemon 7: Squirtle
  - Pokemon 25: Pikachu

When you've completed your inspection of the data, you can comment out the `console.dir` method and use the console.log method to log JUST the name of the Pokemon with the number 59 using the index of the Pokemon in the array you observed. Feel free to uncomment the console.dir as needed to help you complete the rest of the lab.

### Exercise 2

Run the following:

```javascript
console.log(game)
```

Take a moment to familiarize yourself with the `game` object being logged. It has four properties: `party`, `gyms`, and `items`. All of these hold or will hold an array of objects.

- As you move through the exercises `game.party` will hold an array of pokemon objects that will be retrieved from the `pokemon` array discussed in Exercise 1. These are pokemon that you have caught!
- `game.gyms` holds an array of objects, each representing a gym in the game.  (gyms are essentially checkpoints placed throughout the game). Note the `completed` boolean property on each, this will be important later.
- `game.items` holds an array of objects, each representing an item held in an player inventory.

When you've completed your inspection of the data, you can comment out the console.log and move on to Exercise 3. Feel free to uncomment the console.log as needed to help you complete the rest of the lab.

### Exercise 3

```javascript
/*
Add a difficulty property to the game object above.  Give it a value of your choice.

Solve Exercise Three here:
*/


```


### Exercise 4

```javascript
/*
Select a pokemon from the `pokemon` array with a starter property value set to `true` and add it to the `game.party` array. 

Solve Exercise Four here:
*/


```

### Exercise 5

```javascript
/*

Select three more pokemon of your choice from the `pokemon` data and add them to the `game.party` array.

Solve Exercise Five here:
*/



```

### Exercise 6

For this exercise, you'll need to make use of a compare function to define the sort order of `.sort()`. 

Check out the [documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#comparefn) for more information and examples. 

```javascript
/*
Sort the pokemon in the `game.party` by their total hit points (`hp`) in descending order from the greatest to the least.

Solve Exercise Six here:
*/

```

### Exercise 7

```javascript
/*

Complete the gyms that have a difficulty below 3 (change the value of `complete` in the qualifying objects from false to true).

Solve Exercise Seven here:
*/

```

### Exercise 8

```javascript
/*
Evolve the starting pokemon that you picked out in Exercise Four.

Hint: 
- Pokemon 1: Bulbasaur evolves into Pokemon 2: Ivysaur
- Pokemon 4: Charmander evolves into Pokemon 5: Charmeleon
- Pokemon 7: Squirtle evolves into Pokemon 8: Wartortle
- Pokemon 25: Pikachu evolves into Pokemon 26: Raichu

More Hints: The existing starter pokemon will be *replaced* in your party with the pokemon that it evolved into. Remember that you're working with an array of objects - what array method is ideal for replacing one element with another? 

Solve Exercise Eight here:
*/

```

### Exercise 9

```javascript
/*
Print out the name of each pokemon in your party.

Solve Exercise Nine here:
*/

```

### Exercise 10

```javascript
/*
Print out the name of every starter pokemon.

Solve Exercise Ten here:
*/
```

### Exercise 11

```javascript
/*
Add a method called `catchPokemon` to the `game` object. This method should:
- Accept an object as a parameter called `pokemonObj`
- Add the `pokemonObj` to the `game.party` array.
- not return anything

After writing this method, make use of it by calling it and passing in a pokemon object of your choice from the `pokemon` data to catch it.

Solve Exercise Eleven here:
*/
```

### Exercise 12

```javascript
/*
Copy the `catchPokemon` method that you just wrote above, and paste it below.  Modify it so that the quantity of pokeballs in the `items` array decrements by one each time the method is called.

For the purposes of this exercise, it's ok to have a negative number of pokeballs.

After updating the method, make use of it by calling it and passing in a pokemon object of your choice from the `pokemon` data to catch it.

Also, log the `game.items` array to confirm that the pokeball quantity is being decremented.

Solve Exercise Twelve here:
*/


```

### Exercise 13

```javascript
/*
Complete the gyms that have a difficulty below 6 (change the value of
`complete` in the qualifying objects from false to true).

Solve Exercise Thirteen here:
*/


```

### Exercise 14

```javascript
/*
Add a method called `gymStatus` to the `game` object. This method should:
- Not accept any arguments.
- Initially create a constant `gymTally` which is an object that has two properties: `completed` and `incomplete`, both of which are initially set to 0.
- Iterate through the objects in the `game.gyms` array and update the properties on `gymTally` as follows: 
  - `completed` should count how many gyms in the array have a value of `true` for their `completed` property. 
  - `incomplete` should count how many gyms in the array have a value of `false` for their `completed` property.
- Log the value of `gymTally`
- The method should not return anything.

For example, if five gym objects have a value of `true` on their `completed` property and three gym objects have a value of `false` on their `completed` property, the logged value would be: `{ completed: 5, incomplete: 3 }`.

Solve Exercise Fourteen here:
*/
```

### Exercise 15

```javascript
/*
Add a method called `partyCount` to the `game` object. This method should:
- Not accept any arguments
- Count the number of pokemon in the party
- return the found number of pokemon in the party

Solve Exercise Fifteen here:
*/
```

### Exercise 16

```javascript
/*
Complete the gyms that have a difficulty below 8 (change the value of `complete` in the qualifying objects from false to true).

Solve Exercise Sixteen here:
*/
```

### Exercise 17

```javascript
/*
Print the `game` object.

Solve Exercise Seventeen here:
*/

```

Congrats, you're done! If you'ld like to challenge yourself, you can continue on to Exercise in the level-up section. 
