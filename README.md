<!-- AUTOGEN:STATS -->
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript) [![Terminal](https://img.shields.io/badge/mac%20terminal-000000?style=for-the-badge&logo=apple&logoColor=white&labelColor=000000)](https://support.apple.com/guide/terminal/welcome/mac) [![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)](https://code.visualstudio.com/) [![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/) [![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://www.figma.com/) 

[![📊 Views](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-03/main/assets/db/visitors-badge.json)](https://github.com/VuToV-Mykola/goit-js-hw-03/graphs/traffic)
[![⭐ Stars](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-03/main/assets/db/likes-badge.json)](https://github.com/VuToV-Mykola/goit-js-hw-03/actions/workflows/screenshot-and-visitor.yaml)
[![📦 Size](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-03/main/assets/db/repo-size.json)](https://github.com/VuToV-Mykola/goit-js-hw-03)
[![📄 License](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-03/main/assets/db/repo-license.json)](https://github.com/VuToV-Mykola/goit-js-hw-03/blob/main/LICENSE)

## 📸 Скріншот проекту
![Project Screenshot](./assets/screenshot.png)
<!-- END:AUTOGEN -->

## My Achievements

![Description](./assets/head.jpg) <!-- ![Description](./assets/hw-05.jpg) -->

## My Certificates - Completed Sololearn Course:

![Certification Badge](./assets/certificat.jpg)

[SOLOLEARN](https://www.sololearn.com/certificates/CT-VJXN3HQH)

# JavaScript Homework 03

## Task 1. Slug Generator

**File:** `task-1.js`

Before solving the task, let's define a new term!
The term slug is a human-readable unique identifier used in web development to create readable URLs.
For example, instead of a user seeing mysite.com/posts/1q8fh74tx in the address bar, you can create a slug from the article title. As a result, the address will be more pleasant to perceive: mysite.com/posts/arrays-for-beginners.

A slug is always a lowercase string with words separated by hyphens.
Got it? Now let's finally do the task!

Write a function `slugify(title)` that takes an article title, parameter `title`, and returns a slug created from this string.
The value of the `title` parameter will be strings whose words are separated only by spaces.
All slug characters must be lowercase.
All slug words must be separated by hyphens.

### Test Code

Add the following code after your function declaration to check its correctness. The console will display the results of its work.

```javascript
console.log(slugify("Arrays for beginners")); // "arrays-for-beginners"
console.log(slugify("English for developer")); // "english-for-developer"
console.log(slugify("Ten secrets of JavaScript")); // "ten-secrets-of-javascript"
console.log(slugify("How to become a JUNIOR developer in TWO WEEKS")); // "how-to-become-a-junior-developer-in-two-weeks"
```

Leave this code for mentor verification.

### Mentor Review Criteria

- Declared function `slugify(title)`
- Calling `slugify("Arrays for beginners")` returns `"arrays-for-beginners"`
- Calling `slugify("English for developer")` returns `"english-for-developer"`
- Calling `slugify("Ten secrets of JavaScript")` returns `"ten-secrets-of-javascript"`
- Calling `slugify("How to become a JUNIOR developer in TWO WEEKS")` returns `"how-to-become-a-junior-developer-in-two-weeks"`

## Task 2. Array Composition

**File:** `task-2.js`

Write a function called `makeArray` that takes three parameters: `firstArray` (array), `secondArray` (array), and `maxLength` (number). The function should create a new array that contains all elements from `firstArray`, and then all elements from `secondArray`.
If the number of elements in the new array exceeds `maxLength`, the function should return a copy of the array with `maxLength` elements.
Otherwise, the function should return the entire new array.

### Test Code

Add the following code after your function declaration to check its correctness. The console will display the results of its work.

```javascript
console.log(makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3)); // ["Mango", "Poly", "Ajax"]
console.log(makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4)); // ["Mango", "Poly", "Houston", "Ajax"]
console.log(makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3)); // ["Mango", "Ajax", "Chelsea"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2)); // ["Earth", "Jupiter"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4)); // ["Earth", "Jupiter", "Neptune", "Uranus"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0)); // []
```

Leave this code for mentor verification.

### Mentor Review Criteria

- Declared function `makeArray(firstArray, secondArray, maxLength)`
- Calling `makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3)` returns `["Mango", "Poly", "Ajax"]`
- Calling `makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4)` returns `["Mango", "Poly", "Houston", "Ajax"]`
- Calling `makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3)` returns `["Mango", "Ajax", "Chelsea"]`
- Calling `makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2)` returns `["Earth", "Jupiter"]`
- Calling `makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4)` returns `["Earth", "Jupiter", "Neptune", "Uranus"]`
- Calling `makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0)` returns `[]`
- Calling function `makeArray()` with random arrays and random number returns correct array

## Task 3. Number Array Filtering

**File:** `task-3.js`

Write a function `filterArray(numbers, value)` that takes an array of numbers (`numbers`) and a value (`value`) as parameters. The function should return a new array containing only those numbers from the `numbers` array that are greater than the `value`.

Inside the function:
- Create an empty array to which you will add suitable numbers.
- Use a loop to iterate through each element of the `numbers` array.
- Use the conditional operator `if` inside the loop to check each element and add it to your array.
- Return your new array with suitable numbers as a result.

### Test Code

Add the following code after your function declaration to check its correctness. The console will display the results of its work.

```javascript
console.log(filterArray([1, 2, 3, 4, 5], 3)); // [4, 5]
console.log(filterArray([1, 2, 3, 4, 5], 4)); // [5]
console.log(filterArray([1, 2, 3, 4, 5], 5)); // []
console.log(filterArray([12, 24, 8, 41, 76], 38)); // [41, 76]
console.log(filterArray([12, 24, 8, 41, 76], 20)); // [24, 41, 76]
```

Leave this code for mentor verification.

### Mentor Review Criteria

- Declared function `filterArray(numbers, value)`
- Calling function `filterArray([1, 2, 3, 4, 5], 3)` returns `[4, 5]`
- Calling function `filterArray([1, 2, 3, 4, 5], 4)` returns `[5]`
- Calling function `filterArray([1, 2, 3, 4, 5], 5)` returns `[]`
- Calling function `filterArray([12, 24, 8, 41, 76], 38)` returns `[41, 76]`
- Calling function `filterArray([12, 24, 8, 41, 76], 20)` returns `[24, 41, 76]`
- Calling function `filterArray()` with random array and number returns correct arrayost("Australia")); // "Shipping to Australia will cost 170 credits"
console.log(getShippingCost("Germany")); // "Sorry, there is no delivery to your country"
console.log(getShippingCost("China")); // "Shipping to China will cost 100 credits"
console.log(getShippingCost("Chile")); // "Shipping to Chile will cost 250 credits"
console.log(getShippingCost("Jamaica")); // "Shipping to Jamaica will cost 120 credits"
console.log(getShippingCost("Sweden")); // "Sorry, there is no delivery to your country"
```

### Mentor Review Criteria

- Declared function `getShippingCost(country)`
- The function body uses a `switch` statement
- Calling `getShippingCost("Australia")` returns `"Shipping to Australia will cost 170 credits"`
- Calling `getShippingCost("Germany")` returns `"Sorry, there is no delivery to your country"`
- Calling `getShippingCost("China")` returns `"Shipping to China will cost 100 credits"`
- Calling `getShippingCost("Chile")` returns `"Shipping to Chile will cost 250 credits"`
- Calling `getShippingCost("Jamaica")` returns `"Shipping to Jamaica will cost 120 credits"`
- Calling `getShippingCost("Sweden")` returns `"Sorry, there is no delivery to your country"`pingCost("Australia")); // "Shipping to Australia will cost 170 credits"
console.log(getShippingCost("Germany")); // "Sorry, there is no delivery to your country"
console.log(getShippingCost("China")); // "Shipping to China will cost 100 credits"
console.log(getShippingCost("Chile")); // "Shipping to Chile will cost 250 credits"
console.log(getShippingCost("Jamaica")); // "Shipping to Jamaica will cost 120 credits"
console.log(getShippingCost("Sweden")); // "Sorry, there is no delivery to your country"
```

### Mentor Review Criteria

- Declared function `getShippingCost(country)`
- The function body uses a `switch` statement
- Calling `getShippingCost("Australia")` returns `"Shipping to Australia will cost 170 credits"`
- Calling `getShippingCost("Germany")` returns `"Sorry, there is no delivery to your country"`
- Calling `getShippingCost("China")` returns `"Shipping to China will cost 100 credits"`
- Calling `getShippingCost("Chile")` returns `"Shipping to Chile will cost 250 credits"`
- Calling `getShippingCost("Jamaica")` returns `"Shipping to Jamaica will cost 120 credits"`
- Calling `getShippingCost("Sweden")` returns `"Sorry, there is no delivery to your country"`
