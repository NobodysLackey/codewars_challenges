![Codewars](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fkhsmustangmonthly.com%2Fwp-content%2Fuploads%2F2020%2F05%2FInkBanner450x1000.jpg&f=1&nofb=1)

## Date: 5/4/2021

### By: Michael Lackey
#### [Website](https://michaellackey.com/) | [GitHub](https://github.com/mlackey9601) | [LinkedIn](https://www.linkedin.com/in/michaelglackey/)
***

### ***Description***

##### This is a repo for storing all [codewars](https://www.codewars.com/) challenges used over the course of General Assembly's Software Engineering Immersive.
***

<details><summary><strong>8kyu</strong></summary>

<ul type="none">

<li><details><summary><strong>Holiday VI - Shark Pontoon</strong></summary>

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

</details></li>

</details></ul>

____

<details><summary><strong>7kyu</strong></summary>

<ul type="none">

<li><details><summary><strong>Exes and Ohs</strong></summary>

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

</details></li>

<li><details><summary><strong>Merge Two Arrays</strong></summary>

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

</details></li>

<li><details><summary><strong>Basic Sequence Practice</strong></summary>

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
function sumOfN(n) {
  let sumArr = [];
  sumArr[0] = 0;
  for (let i = 1; i < Math.abs(n)+1; i++) {
    if(n > 0) {
      sumArr[i] = sumArr[i-1]+i;
    } else {
      sumArr[i] = sumArr[i-1]-i;
    }
  }
  return sumArr
}
```

</details></li>

<li><details><summary><strong>Fun with ES6 Classes #3 - Cuboids, Cubes, and Getters</strong></summary>

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

</details></li>

<li><details><summary><strong>Calculator: Coin Combination</strong></summary>

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

</details></li>

<li><details><summary><strong>Every Possible Sum of Two Digits</strong></summary>

#### [LINK](https://www.codewars.com/kata/5b4e474305f04bea11000148/train/javascript)
#### PROMPT: 
Given a long number, return all the possible sum of two digits of it.

#### EXAMPLE:
12345: all possible sum of two digits from that number are:
```javascript
[ 1 + 2, 1 + 3, 1 + 4, 1 + 5, 2 + 3, 2 + 4, 2 + 5, 3 + 4, 3 + 5, 4 + 5 ]
```
Therefore the result must be:
```javascript
[ 3, 4, 5, 6, 5, 6, 7, 7, 8, 9 ]
```

#### SOLUTION:
```javascript
solution here
```

</details></li>

<li><details><summary><strong>Simple Fun #136: Missing Values</strong></summary>

#### [LINK](https://www.codewars.com/kata/58a66c208b88b2de660000c3/train/javascript)
#### PROMPT: 
You are given a sequence of positive ints where every element appears three times, except one that appears only once (let's call it x) and one that appears only twice (let's call it y).

Your task is to find x * x * y.

Input/Output:

[input] integer array arr
an array contains positive integers.

[output] an integer
The value of x * x * y

#### EXAMPLES:
```javascript
arr = [1, 1, 1, 2, 2, 3] --> 18
//  3 x 3 x 2 = 18

arr = [6, 5, 4, 100, 6, 5, 4, 100, 6, 5, 4, 200] --> 4000000
//  200 x 200 x 100 = 4000000
```

#### SOLUTION:
```javascript
solution here
```

</details></li>

<li><details><summary><strong>Larger Product or Sum</strong></summary>

#### [LINK](https://www.codewars.com/kata/5c4cb8fc3cf185147a5bdd02/train/javascript)
#### PROMPT: 
For this Kata you will be given an array of numbers and another number n. You have to find the sum of the n largest numbers of the array and the product of the n smallest numbers of the array, and compare the two.

If the sum of the n largest numbers is higher, return "sum"
If the product of the n smallest numbers is higher, return "product"
If the 2 values are equal, return "same"

Note The array will never be empty and n will always be smaller than the length of the array.

#### EXAMPLE:
```javascript
sumOrProduct([10, 41, 8, 16, 20, 36, 9, 13, 20], 3) --> "product"
```

The sum of the 3 highest numbers is 41 + 36 + 20 = 97

The product of the lowest 3 numbers is 8 x 9 x 10 = 720

The product of the 3 lowest numbers is higher than the sum of the 3 highest numbers so the function returns "product"

#### SOLUTION:
```javascript
solution here
```

</details></li>

<li><details><summary><strong>Isograms</strong></summary>

#### [LINK](https://www.codewars.com/kata/54ba84be607a92aa900000f1/train/javascript)
#### PROMPT: 
An isogram is a word that has no repeating letters, consecutive or non-consecutive. Implement a function that determines whether a string that contains only letters is an isogram. Assume the empty string is an isogram. Ignore letter case.

#### EXAMPLES:
```javascript
isIsogram("Dermatoglyphics") --> true
isIsogram("aba") --> false
isIsogram("moOse") --> false // ignore letter case
```

#### SOLUTION:
```javascript
solution here
```

</details></li>

<li><details><summary><strong>Growth of a Population</strong></summary>

#### [LINK]()
#### PROMPT: 
In a small town the population is p0 = 1000 at the beginning of a year. The population regularly increases by 2 percent per year and moreover 50 new inhabitants per year come to live in the town. How many years does the town need to see its population greater or equal to p = 1200 inhabitants?

At the end of the first year there will be: 
1000 + 1000 * 0.02 + 50 => 1070 inhabitants

At the end of the 2nd year there will be: 
1070 + 1070 * 0.02 + 50 => 1141 inhabitants (** number of inhabitants is an integer **)

At the end of the 3rd year there will be:
1141 + 1141 * 0.02 + 50 => 1213

It will need 3 entire years.
More generally given parameters:

p0, percent, aug (inhabitants coming or leaving each year), p (population to surpass)

the function nb_year should return n number of entire years needed to get a population greater or equal to p.

aug is an integer, percent a positive or null floating number, p0 and p are positive integers (> 0)

#### EXAMPLES:
```javascript
nb_year(1500, 5, 100, 5000) --> 15
nb_year(1500000, 2.5, 10000, 2000000) --> 10
```

Note: Don't forget to convert the percent parameter as a percentage in the body of your function: if the parameter percent is 2 you have to convert it to 0.02.

#### SOLUTION:
```javascript
solution here
```

</details></li>

</details></ul>

____

<details><summary><strong>6kyu</strong></summary>

<ul type="none">

<li><details><summary><strong>Find the Odd Integer</strong></summary>

#### [LINK](https://www.codewars.com/kata/54da5a58ea159efa38000836/train/javascript)
#### PROMPT: 
Given an array of integers, find the one that appears an odd number of times.

There will always be only one integer that appears an odd number of times.

#### SOLUTION:
```javascript
solution here
```

</details></li>

<li><details><summary><strong>English Beggars</strong></summary>

#### [LINK](https://www.codewars.com/kata/59590976838112bfea0000fa/train/javascript)
#### PROMPT: 
Your task here is pretty simple: given an array of values and an amount of beggars, you are supposed to return an array with the sum of what each beggar brings home, assuming they all take regular turns, from the first to the last.

For example: [1,2,3,4,5] for 2 beggars will return a result of [9,6], as the first one takes [1,3,5], the second collects [2,4].

The same array with 3 beggars would have in turn have produced a better out come for the second beggar: [5,7,3], as they will respectively take [1,4], [2,5] and [3].

Also note that not all beggars have to take the same amount of "offers", meaning that the length of the array is not necessarily a multiple of n; length can be even shorter, in which case the last beggars will of course take nothing (0).

Note: in case you don't get why this kata is about English beggars, then you are not familiar on how religiously queues are taken in the kingdom ;)

Note 2: do not modify the input array.

#### SOLUTION:
```javascript
solution here
```

</details></li>

<li><details><summary><strong>Create Phone Number</strong></summary>

#### [LINK](https://www.codewars.com/kata/525f50e3b73515a6db000b83/train/javascript)
#### PROMPT:
Write a function that accepts an array of 10 integers (between 0 and 9), that returns a string of those numbers in the form of a phone number.

#### EXAMPLE:
```javascript
createPhoneNumber([1, 2, 3, 4, 5, 6, 7, 8, 9, 0]) --> "(123) 456-7890"
```

The returned format must be correct in order to complete this challenge.
Don't forget the space after the closing parentheses!

#### SOLUTION:
```javascript
solution here
```

</details></li>

<li><details><summary><strong>Who Likes It?</strong></summary>

#### [LINK](https://www.codewars.com/kata/5266876b8f4bf2da9b000362/train/javascript)
#### PROMPT: 
You probably know the "like" system from Facebook and other pages. People can "like" blog posts, pictures or other items. We want to create the text that should be displayed next to such an item.

Implement a function likes :: [String] -> String, which must take in input array, containing the names of people who like an item. It must return the display text.

#### EXAMPLES:
```javascript
likes [] --> "no one likes this"
likes ["Peter"] --> "Peter likes this"
likes ["Jacob", "Alex"] --> "Jacob and Alex like this"
likes ["Max", "John", "Mark"] --> "Max, John and Mark like this"
likes ["Alex", "Jacob", "Mark", "Max"] --> "Alex, Jacob and 2 others like this"
```

#### SOLUTION:
```javascript
solution here
```

</details></li>

<li><details><summary><strong>Split Strings</strong></summary>

#### [LINK](https://www.codewars.com/kata/515de9ae9dcfc28eb6000001/train/javascript)
#### PROMPT: 
Complete the solution so that it splits the string into pairs of two characters. If the string contains an odd number of characters then it should replace the missing second character of the final pair with an underscore ('_').

#### EXAMPLES:
```javascript
solution('abc') --> ['ab', 'c_']
solution('abcdef') --> ['ab', 'cd', 'ef']
```

#### SOLUTION:
```javascript
solution here
```

</details></li>

</details></ul>

____

<details><summary><strong>5kyu</strong></summary>

<ul type="none">

<li><details><summary><strong>NAME</strong></summary>

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

</details></li>

</details></ul>

____

<details><summary><strong>4kyu</strong></summary>

<ul type="none">

<li><details><summary><strong>NAME</strong></summary>

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

</details></li>

</details></ul>

____

<details><summary><strong>3kyu</strong></summary>

<ul type="none">

<li><details><summary><strong>NAME</strong></summary>

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

</details></li>

</details></ul>

____
