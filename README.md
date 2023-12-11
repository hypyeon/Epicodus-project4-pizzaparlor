# Pizza Parlor 🍕
by [Hayeong Pyeon](https://www.hayeong.website)

## Table of Contents

1. [Technologies Used](#technologies-used)
2. [Description](#description)
3. [Setup Requirements](#setup-requirements)
4. [Link](#link)
5. [Tests](#tests)
6. [Known Bugs](#known-bugs)
7. [License](#license)

## Technologies used
- HTML5
- SCSS
- JavaScript
- Test Driven Development

## Description
- This is an independent project assigned by Epicodus. 
- This project is part of 'Object-oriented JS' course. 
- On the webpage, you can make up to 3 different pizza orders by customizing each one. Each order will be added to the right section which users have access to see order details upon clicking 'order detail' button. 
- TDD included in this file.

## Setup Requirements
1. Clone this repository to your desktop.
2. Navigate to the top level of the directory. 
3. Open `index.html` in your browser. 

## Link
https://hypyeon.github.io/pizza-parlor/

## Tests
```
Describe: Order()
 
Test: "It should return an Order object with five properties for: order name, size of pizza, an array of selected $2 toppings, an array of selected $3 toppings, and food receive method."
Code: const firstPizza = new Order("Minsu", "large", ["olive", "mushroom"], ["pepperoni"], "pickup");
Expected: Order { orderName: "Minsu", size: "large", firstToppings: ["olive", "mushroom"], secondToppings: ["pepperoni"], method: "pickup" }

Describe: Order.prototype.getToppingNames()
 
Test: "It should return all of selected topping names."
Code: firstPizza.getNumOfToppings();
Expected: "olive, mushroom, pepperoni"

Describe: Order.prototype.getTotalPrice()
 
Test: "It should return a total price for the order, rounded to 2 decimals."
Code: firstPizza.getTotalPrice();
Expected: 22.09

Describe: Order.prototype.discountEligibility()
 
Test: "It should return 'Yes' or 'No', depending on the order receive method users choose."
Code: firstPizza.discountEligibility();
Expected: "Yes"

Describe: formatName()
 
Test: "It should return a name with the first letter in upper case and the rest in lower cases."
Code: formatName("elsa");
Expected: "Elsa"
```
## Known Bugs
- No bugs detected currently. Feel free to reach out to the [author](mailto:hayeong.pyeon@gmail.com) if find any. 
- Last updated: December 10, 2023

## License
[MIT](/LICENSE.txt) Copyright © 2023 Hayeong Pyeon  
Icons used for background is downloaded from [Icons8](https://icons8.com/icon/7DNAxn61w5zi/pizza)