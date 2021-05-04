# Codewars Challenges

## Date: 5/4/2021

### By: Michael Lackey
#### [Website](https://michaellackey.com/) | [GitHub](https://github.com/mlackey9601) | [LinkedIn](https://www.linkedin.com/in/michaelglackey/)
***

### ***Description***

##### This is a repo for storing all [codewars](https://www.codewars.com/) challenges used over the course of General Assembly's Software Engineering Immersive.
***

## 8kyu
***

#### NAME: Holiday VI - Shark Pontoon
#### [LINK](https://www.codewars.com/kata/57e921d8b36340f1fd000059/train/javascript)
#### PROMPT: 
Your friend invites you out to a cool floating pontoon around 1km off the beach. Among other things, the pontoon has a huge slide that drops you out right into the ocean, a small way from a set of stairs used to climb out.

As you plunge out of the slide into the water, you see a shark hovering in the darkness under the pontoon... Crap!

You need to work out if the shark will get to you before you can get to the pontoon. To make it easier... as you do the mental calculations in the water you either freeze when you realise you are dead, or swim when you realise you can make it!

You are given 5 variables:

- sharkDistance = distance from the shark to the pontoon. The shark will eat you if it reaches you before you escape to the pontoon.

- sharkSpeed = how fast it can move in metres/second.

- pontoonDistance = how far you need to swim to safety in metres.

- youSpeed = how fast you can swim in metres/second.

- dolphin = a boolean, if true, you can half the swimming speed of the shark as the dolphin will attack it.

The pontoon, you, and the shark are all aligned in one dimension.

If you make it, return "Alive!", if not, return "Shark Bait!".

#### SOLUTION:
```javascript
solution here
```
***

## 7kyu
***

#### NAME: Exes and Ohs
#### [LINK](https://www.codewars.com/kata/55908aad6620c066bc00002a/train/javascript)
#### PROMPT: 
Check to see if a string has the same amount of 'x's and 'o's. The method must return a boolean and be case insensitive. The string can contain any char.

#### EXAMPLES:
```javascript
XO("ooxx") --> true
XO("xooxx") --> false
XO("ooxXm") --> true
XO("zpzpzpp") --> true // when no 'x' and 'o' is present, should return true
XO("zzoo") --> false
```

##### SOLUTION:
```javascript
solution here
```
***

#### NAME: Merge Two Arrays
#### [LINK](https://www.codewars.com/kata/583af10620dda4da270000c5/train/javascript)
#### PROMPT: 
Write a function that combines two arrays by alternatingly taking elements from each array in turn.

#### EXAMPLES:
```javascript
[a, b, c, d, e], [1, 2, 3, 4, 5] --> [a, 1, b, 2, c, 3, d, 4, e, 5]

[1, 2, 3], [a, b, c, d, e, f] --> [1, a, 2, b, 3, c, d, e, f]
```

The arrays may be of different lengths, with at least one character/digit.
One array will be of string characters (in lower case, a-z), a second of integers (all positive starting at 1).

#### SOLUTION:
```javascript
solution here
```
***

#### NAME: Basic Sequence Practice
#### [LINK](https://www.codewars.com/kata/5436f26c4e3d6c40e5000282/train/javascript)
#### PROMPT: 
A sequence or a series, in mathematics, is a string of objects, like numbers, that follow a particular pattern. The individual elements in a sequence are called terms. A simple example is 3, 6, 9, 12, 15, 18, 21, ..., where the pattern is: "add 3 to the previous term".

In this kata, we will be using a more complicated sequence: 0, 1, 3, 6, 10, 15, 21, 28, ... This sequence is generated with the pattern: "the nth term is the sum of numbers from 0 to n, inclusive".

```javascript
[ 0,  1,    3,      6,   ...]
0  0+1  0+1+2  0+1+2+3
```

Complete the function that takes an integer n and returns a list/array of length abs(n) + 1 of the arithmetic series explained above. Whenn < 0 return the sequence with negative terms.

#### EXAMPLES:
```javascript
 5  -->  [0,  1,  3,  6,  10,  15]
-5  -->  [0, -1, -3, -6, -10, -15]
 7  -->  [0,  1,  3,  6,  10,  15,  21,  28]
```

#### SOLUTION:
```javascript
solution here
```
***

#### NAME: Fun with ES6 Classes #3 - Cuboids, Cubes, and Getters
#### [LINK](https://www.codewars.com/kata/56fbdda707cff41b68000de2/train/javascript)
#### PROMPT: 
Define the following classes.

I. Cuboid
The object constructor for the class Cuboid should receive exactly three arguments in the following order: length, width, height and store these three values in this.length, this.width and this.height respectively.

The class Cuboid should then have a getter surfaceArea which returns the surface area of the cuboid and a getter volume which returns the volume of the cuboid.

II. Cube
class Cube is a subclass of class Cuboid. The constructor function of Cube should receive one argument only, its length, and use that value passed in to set this.length, this.width and this.height.

Hint: Make a call to super, passing in the correct arguments, to make life easier ;)

#### SOLUTION:
```javascript
solution here
```
***

#### NAME: Calculator: Coin Combination
#### [LINK](https://www.codewars.com/kata/564d0490e96393fc5c000029/train/javascript)
#### PROMPT: 
The function takes cents value (int) and needs to return the minimum number of coins combination of the same value.

The function should return an array where
coins[0] = pennies ==> $00.01
coins[1] = nickels ==> $00.05
coins[2] = dimes ==> $00.10
coins[3] = quarters ==> $00.25

#### EXAMPLE:
```javascript
coinCombo(6) --> [1, 1, 0, 0]
```

#### SOLUTION:
```javascript
solution here
```
***

#### NAME: 
#### [LINK]()
#### PROMPT: 


#### EXAMPLES:
```javascript
examples here
```

#### SOLUTION:
```javascript
solution here
```
***

#### NAME: 
#### [LINK]()
#### PROMPT: 


#### EXAMPLES:
```javascript
examples here
```

#### SOLUTION:
```javascript
solution here
```
***

#### NAME: 
#### [LINK]()
#### PROMPT: 


#### EXAMPLES:
```javascript
examples here
```

#### SOLUTION:
```javascript
solution here
```
***

## 6kyu
***

## 5kyu
***

## 4kyu
***

## 3kyu
***
