# Intro to JavaScript Objects Lab - Lab Exercise

![Hero image](./assets/hero.png)

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

Copy and paste each of the following exercises into your JavaScript file. To check your work, open the file in a web browser and inspect the console output, or run the file in your terminal using node app.js.

### Exercise 1
The answer for this exercise has been provided for you: 

```javascript
console.dir(pokemon, { maxArrayLength: null })
```

Spend some time inspecting the pokemon data we magically have access to in the
`pokemon` array that is being logged below. You have not seen this console
method before, but we're using it here so that you're able to see all of the
pokemon in the console. By default, only the first 100 items in an array are
shown - we're overriding that behavior here.

Take note of the shape of the data here. Each pokemon object in the array has:
- a number, which is a number between 1 and 151
- a name, which is a string
- a type, which is a string
- hp (hit points), which is a number
- a starter boolean.

There's some game-specific terminology here, so if you've never played pokemon
here's a quick primer on what these mean:
- All pokemon have a number that acts as a unique identifier
- All pokemon have a type that indicates their primary abilities. Pokemon 
  generally have multiple types, but we're only using a pokemon's primary type 
  here to make working with this data more manageable.
- All pokemon have hit points - essentially a quantitative measure of a 
  pokemon's constitution.
- At the start of a game, a player must select a starting pokemon. Acceptable 
  starting pokemon objects will have a starter property with a value set to 
  true. Four pokemon fit this criterion:
  - Pokemon 1: Bulbasaur
  - Pokemon 4: Charmander
  - Pokemon 7: Squirtle
  - Pokemon 25: Pikachu

When you've completed your inspection of the data, you can comment out the
console.dir method and use the console.log method to log JUST the name of the 
Pokemon with the number 59 using the index of the Pokemon in the array you 
observed. Feel free to uncomment the console.dir as needed to help you 
complete the rest of the lab.

### Exercise 2

```javascript
console.log(game)
```

Take a moment to familiarize yourself with the `game` object being logged.
It has four properties: `party`, `gyms`, and `items`. All of these hold or will hold an array of objects.

Note that in a full-fledged application, this game object would likely be broken up
into many smaller objects with more specific jobs - we're using one object here
for simplicity and utility to ease your learning experience.

- As you move through the exercises `game.party` will hold an array of pokemon 
  objects that will be retrieved from the `pokemon` array discussed in Exercise
  Two. These are pokemon that you have caught!
- game.gyms holds an array of objects, each representing a gym in the game.
  (gyms are essentially checkpoints placed throughout the game). Note the 
  `completed` boolean property on each, this will be important later.
- game.items holds an array of objects, each representing an item held in an
  player inventory.

When you've completed your inspection of the data, you can comment out the
console.log and move on to Exercise Three. Feel free to uncomment the
console.log as needed to help you complete the rest of the lab.

### Exercise 3

```javascript
// Add a difficulty property to the game object above.
// Give it a value of your choice.

// Solve Exercise Three here:


console.log('Exercise 3 result:', game.difficulty)
```


### Exercise 4

```javascript
/*
Select a pokemon from the `pokemon` data with a starter property value set to 
`true` and add it to the `game.party` array. 

Solve Exercise Four here:
*/


```

### Exercise 5

```javascript
/*

Select three more pokemon of your choice from the `pokemon` data and add them 
to the `game.party` array.

Solve Exercise Five here:
*/



```

### Exercise 6

```javascript
/*
Sort the pokemon in the `game.party` by their total hit points (`hp`) in
descenting order from the greatest to the least.

Solve Exercise Six here:
*/

```

### Exercise 7

```javascript
/*

Complete the gyms that have a difficulty below 3 (change the value of
`complete` in the qualifying objects from false to true).

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

More Hints: The existing starter pokemon will be *replaced* in your party with
            the pokemon that it evolved into.

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
- Accept an object on a parameter called `pokemonObj`
- Add the `pokemonObj` to the `game.party` array.
- not return anything

After writing this method, make use of it by calling it and passing in a 
pokemon object of your choice from the `pokemon` data to catch it.

Solve Exercise Eleven here:

*/
```

### Exercise 12

```javascript


```