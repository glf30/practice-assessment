# Practice Assessment

* Please include the correct number of parameters in each function!
* Make sure every function that is supposed to return something returns something
* You can console.log() the functions with test input to test your functions in the space provided
* Read each question carefully
* You are NOT forking this project.  Just a git clone will suffice!  Please submit your main.js file to populi
* Good luck!

## Methods you might need
* .toLowerCase()
* .toUpperCase()
* .concat()
* .indexOf()
* .includes()
* .push()
* .unshift()
* That's really all!  I think the only one that you'll NEED to use is .push(), the rest are optional/may possibly make your life easier.  
* You can use anything else we've formally covered.
* If we have not covered it, please ask to be sure that it's okay.

## Tasks

You can solve all of the following problems in the same file or separate files, up you.
## `sumOfOdds`

Write a function called `sumOfOdds` that takes in two numbers and returns the sum of all odd numbers between them, inclusive.

You can assume the second number will always be greater than the first and that the two numbers will not be the same.

**Test Cases**
```js
sumOfOdds(1, 5) // 9
sumOfOdds(4, 10) // 21
sumOfOdds(2, 4) // 3
```

## `arraySubtract`

Write a function called `arraySubtract` that takes in two arrays of numbers and subtracts each item in the second array from the corresponding item in the first array. Return a new array containing the results.

You can assume both arrays will have the same length.

**Test Cases**
```js
arraySubtract([7, 9], [2, 6]) // [5, 3]
arraySubtract([10, 20, 30], [1, 5, 10]) // [9, 15, 20]
arraySubtract([3, 4, 5], [5, 4, 3]) // [-2, 0, 2]
```

## `surroundArray`

Write a function called `surroundArray` that takes in three parameters in this order: an array, a string, and another string.

Add the first string to the beginning of the array and the second string to the end of the array. Return the modified array.

**Test Cases**
```js
surroundArray([1, 2, 3], "start", "end") // ["start", 1, 2, 3, "end"]
surroundArray(["apple", "banana"], "fruit", "basket") // ["fruit", "apple", "banana", "basket"]
surroundArray([], "first", "last") // ["first", "last"]
```

## `longestString`

Write a function called `longestString` that takes in an array of strings and returns the longest string in the array.

If the array is empty, return an empty string (`''`).

You can assume no two strings in the array will have the same length.

**Test Cases**
```js
longestString(["cat", "elephant", "dog"]) // "elephant"
longestString(["a", "abcd", "ab"]) // "abcd"
longestString([]) // ""
```

## `sToR`

Write a function called `sToR` that replaces every `s` character in a string with an `r` and every `r` character with an `s`.

If a letter in the original string is uppercase, the corresponding letter in the output must also be uppercase.

**Do not use `replaceAll()` or similar string methods.** If you are unsure what this means, ask before using a string method. `toUpperCase()` and `toLowerCase()` should be all you need, if anything.

**Test Cases**
```js
sToR("ssRR") // "rrSS"
sToR("Roses") // "Soser"
sToR("HELLO") // "HELLO"
```

## `divisibleBy4And7`

Write a function called `divisibleBy4And7` that takes in a number and returns `true` if it is divisible by both 4 and 7. Otherwise, return `false`.

**Test Cases**
```js
divisibleBy4And7(28) // true
divisibleBy4And7(8) // false
divisibleBy4And7(49) // false
```

## `exclamationAndQuestion`

Write a function called `exclamationAndQuestion` that takes in a string and returns `true` if it contains both an exclamation point (`!`) and a question mark (`?`). Otherwise, return `false`.

**Test Cases**
```js
exclamationAndQuestion("Really?!") // true
exclamationAndQuestion("Hello!") // false
exclamationAndQuestion("What? No way!") // true
```

## `countAB`

Write a function called `countAB` that takes in a string and returns an array of length two.

- The first item should be the count of all `A` and `a` characters.
- The second item should be the count of all `B` and `b` characters.

Return the two counts separately; do not add them together.

**Test Cases**
```js
countAB("ABBA") // [2, 2]
countAB("aAbBc") // [2, 2]
countAB("Hello") // [0, 0]
```

## `createCharacter`

Write a function called `createCharacter` that takes in three parameters in this order: a name (string), an attack stat (`atk`, number), and a defense stat (`def`, number).

Create and return an object containing these three properties.

**Test Cases**
```js
createCharacter("Noah", 10, 5) // { name: "Noah", atk: 10, def: 5 }
createCharacter("Mio", 15, 3) // { name: "Mio", atk: 15, def: 3 }
```

## `pairUp`

Write a function called `pairUp` that takes in two character objects. Each character has a `name` (string), `atk` (number), and `def` (number).

For each character, add the following properties:
- `pairUp`: a boolean set to `true`
- `pairPartner`: a string containing the other character's name

Finally, increase the `atk` of the first character by half the `atk` of the second character.

**Test Cases**
```js
const character1 = { name: "Noah", atk: 10, def: 5 };
const character2 = { name: "Mio", atk: 8, def: 3 };

pairUp(character1, character2);
// character1: { name: "Noah", atk: 14, def: 5, pairUp: true, pairPartner: "Mio" }
// character2: { name: "Mio", atk: 8, def: 3, pairUp: true, pairPartner: "Noah" }

const character3 = { name: "Chrom", atk: 12, def: 4 };
const character4 = { name: "Robin", atk: 6, def: 7 };

pairUp(character3, character4);
// character3: { name: "Chrom", atk: 15, def: 4, pairUp: true, pairPartner: "Robin" }
// character4: { name: "Robin", atk: 6, def: 7, pairUp: true, pairPartner: "Chrom" }
```
