<!-- AUTOGEN:STATS -->
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript) [![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML) [![Terminal](https://img.shields.io/badge/mac%20terminal-000000?style=for-the-badge&logo=apple&logoColor=white&labelColor=000000)](https://support.apple.com/guide/terminal/welcome/mac) [![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)](https://code.visualstudio.com/) [![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/) [![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://www.figma.com/) 

[![📊 Views](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-02/main/assets/db/visitors-badge.json)](https://github.com/VuToV-Mykola/goit-js-hw-02/graphs/traffic)
[![⭐ Stars](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-02/main/assets/db/likes-badge.json)](https://github.com/VuToV-Mykola/goit-js-hw-02/actions/workflows/screenshot-and-visitor.yaml)
[![📦 Size](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-02/main/assets/db/repo-size.json)](https://github.com/VuToV-Mykola/goit-js-hw-02)
[![📄 License](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-02/main/assets/db/repo-license.json)](https://github.com/VuToV-Mykola/goit-js-hw-02/blob/main/LICENSE)

## 📸 Скріншот проекту
![Project Screenshot](./assets/screenshot.png)
<!-- END:AUTOGEN -->

## My Achievements

![Description](./assets/head.jpg) <!-- ![Description](./assets/hw-05.jpg) -->

## My Certificates - Completed Sololearn Course:

![Certification Badge](./assets/certificat.jpg)

[SOLOLEARN](https://www.sololearn.com/certificates/CT-VJXN3HQH)

# JavaScript Homework 02

## Task 1. Droid Orders

**File:** `task-1.js`

The repair droid sales station is ready to go, all that remains is to write the software for the sales department.

Declare the `makeTransaction(quantity, pricePerDroid, customerCredits)` function, which composes and returns a message about purchasing repair droids.

It declares three parameters, whose values will be set when calling it:
- `quantity` — number of ordered droids
- `pricePerDroid` — price of one droid
- `customerCredits` — amount of funds in the customer's account

Complete the function as follows:
- Declare a variable to store the total order amount (total cost of all ordered droids) and assign it an expression to calculate this amount.
- Add a check whether the customer can pay for the order:
  - if the amount to be paid exceeds the number of credits in the customer's account, the function should return the string `"Insufficient funds!"`
  - otherwise, the function should return the string `"You ordered <quantity> droids worth <totalPrice> credits!"`, where `<quantity>` is the number of ordered droids, and `<totalPrice>` is their total cost.

### Test Code

Add the following code after your function declaration to check its correctness:

```javascript
console.log(makeTransaction(5, 3000, 23000)); // "You ordered 5 droids worth 15000 credits!"
console.log(makeTransaction(3, 1000, 15000)); // "You ordered 3 droids worth 3000 credits!"
console.log(makeTransaction(10, 5000, 8000)); // "Insufficient funds!"
console.log(makeTransaction(8, 2000, 10000)); // "Insufficient funds!"
console.log(makeTransaction(10, 500, 5000)); // "You ordered 10 droids worth 5000 credits!"
```

### Mentor Review Criteria

- Declared function `makeTransaction(quantity, pricePerDroid, customerCredits)`
- Calling `makeTransaction(5, 3000, 23000)` returns `"You ordered 5 droids worth 15000 credits!"`
- Calling `makeTransaction(3, 1000, 15000)` returns `"You ordered 3 droids worth 3000 credits!"`
- Calling `makeTransaction(10, 5000, 8000)` returns `"Insufficient funds!"`
- Calling `makeTransaction(8, 2000, 10000)` returns `"Insufficient funds!"`
- Calling `makeTransaction(10, 500, 5000)` returns `"You ordered 10 droids worth 5000 credits!"`

## Task 2. Message Formatting

**File:** `task-2.js`

Declare the `formatMessage(message, maxLength)` function, which takes a string (parameter `message`) and checks its length according to the given maximum length (parameter `maxLength`).

Complete the function code so that:
- If the string length is equal to or less than `maxLength`, then the function returns the original string unchanged.
- If the length exceeds `maxLength`, then the function truncates the string to `maxLength` characters, adds ellipsis `"..."` at the end and returns the truncated version.

### Test Code

Add the following code after your function declaration to check its correctness:

```javascript
console.log(formatMessage("Curabitur ligula sapien", 16)); // "Curabitur ligula..."
console.log(formatMessage("Curabitur ligula sapien", 23)); // "Curabitur ligula sapien"
console.log(formatMessage("Vestibulum facilisis purus nec", 20)); // "Vestibulum facilisis..."
console.log(formatMessage("Vestibulum facilisis purus nec", 30)); // "Vestibulum facilisis purus nec"
console.log(formatMessage("Nunc sed turpis a felis in nunc fringilla", 15)); // "Nunc sed turpis..."
console.log(formatMessage("Nunc sed turpis a felis in nunc fringilla", 41)); // "Nunc sed turpis a felis in nunc fringilla"
```

### Mentor Review Criteria

- Declared function `formatMessage(message, maxLength)`
- Calling `formatMessage("Curabitur ligula sapien", 16)` returns `"Curabitur ligula..."`
- Calling `formatMessage("Curabitur ligula sapien", 23)` returns `"Curabitur ligula sapien"`
- Calling `formatMessage("Vestibulum facilisis purus nec", 20)` returns `"Vestibulum facilisis..."`
- Calling `formatMessage("Vestibulum facilisis purus nec", 30)` returns `"Vestibulum facilisis purus nec"`
- Calling `formatMessage("Nunc sed turpis a felis in nunc fringilla", 15)` returns `"Nunc sed turpis..."`
- Calling `formatMessage("Nunc sed turpis a felis in nunc fringilla", 41)` returns `"Nunc sed turpis a felis in nunc fringilla"`

## Task 3. Spam Check

**File:** `task-3.js`

The `checkForSpam(message)` function takes a string (parameter `message`), checks it for forbidden words `spam` and `sale`, and returns the check result. Words in the `message` parameter string can be in any case, for example `SPAM` or `sAlE`.

Complete the function code so that:
- If a forbidden word is found (`spam` or `sale`), then the function returns boolean `true`
- If there are no forbidden words in the string, the function returns boolean `false`

### Test Code

Add the following code after your function declaration to check its correctness:

```javascript
console.log(checkForSpam("Latest technology news")); // false
console.log(checkForSpam("JavaScript weekly newsletter")); // false
console.log(checkForSpam("Get best sale offers now!")); // true
console.log(checkForSpam("Amazing SalE, only tonight!")); // true
console.log(checkForSpam("Trust me, this is not a spam message")); // true
console.log(checkForSpam("Get rid of sPaM emails. Our book in on sale!")); // true
console.log(checkForSpam("[SPAM] How to earn fast money?")); // true
```

### Mentor Review Criteria

- Declared function `checkForSpam(message)`
- Calling `checkForSpam("Latest technology news")` returns `false`
- Calling `checkForSpam("JavaScript weekly newsletter")` returns `false`
- Calling `checkForSpam("Get best sale offers now!")` returns `true`
- Calling `checkForSpam("Amazing SalE, only tonight!")` returns `true`
- Calling `checkForSpam("Trust me, this is not a spam message")` returns `true`
- Calling `checkForSpam("Get rid of sPaM emails. Our book in on sale!")` returns `true`
- Calling `checkForSpam("[SPAM] How to earn fast money?")` returns `true`

## Task 4. Product Delivery

**File:** `task-4.js`

Declare the `getShippingCost(country)` function, which should check the possibility of delivering goods to the user's country (parameter `country`) and return a message about the result. Be sure to use the `switch` statement.

The format of the returned string is `"Shipping to <country> will cost <price> credits"`, where instead of `<country>` and `<price>` you need to substitute the corresponding values.

List of countries and delivery cost:
- China — 100 credits
- Chile — 250 credits
- Australia — 170 credits
- Jamaica — 120 credits

From the list you can see that delivery is not possible everywhere. If the specified country is not in the list, then the function should return the string `"Sorry, there is no delivery to your country"`.

### Test Code

Add the following code after your function declaration to check its correctness:

```javascript
console.log(getShippingCost("Australia")); // "Shipping to Australia will cost 170 credits"
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
