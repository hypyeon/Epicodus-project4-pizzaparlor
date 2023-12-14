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
https://hypyeon.github.io/Epicodus-project4-pizzaparlor/

## Tests
```
Describe: Order()
 
Test: "It should return an Order object with five properties for: order name, size of pizza, an array of selected $2 toppings, an array of selected $3 toppings, and order receive method."
Code: const orderMinsu = new Order("Minsu", "large", ["olive", "mushroom"], ["pepperoni"], "pickup");
Expected: Order { orderName: "Minsu", size: "large", firstToppings: ["olive", "mushroom"], secondToppings: ["pepperoni"], method: "pickup" }

Describe: Order.prototype.getToppingNames()
 
Test: "It should return all of selected topping names."
Code: 
    const orderMinsu = new Order("Minsu", "large", ["olive", "mushroom"], ["pepperoni"], "pickup");
    orderMinsu.getToppingNames();
Expected: "Olive, Mushroom, Pepperoni"

Describe: Order.prototype.getTotalPrice()
 
Test: "It should return a total price for the order, fixed to 2 decimals. Base price differs by pizza size and there are $2 and $3 worth of toppings whose price will be added to the base price if selected."
Code: 
    const orderMinsu = new Order("Minsu", "large", ["olive", "mushroom"], ["pepperoni"], "delivery");
    orderMinsu.getTotalPrice();
Expected: 23.25

Test: "If "pickup" is selected, there will be 5% discount applied to the total price."
Code: 
    const orderJulie = new Order("Julie", "large", ["olive", "mushroom"], ["pepperoni"], "pickup");
    orderJulie.getTotalPrice();
Expected: 22.09

Describe: Order.prototype.discountEligibility()
 
Test: "It should return 'Yes' if "pickup" is selected for delivery method."
Code: 
    const orderJulie = new Order("Julie", "large", ["olive", "mushroom"], ["pepperoni"], "pickup");
    orderJulie.discountEligibility();
Expected: "Yes"

Test: "It should return 'No' if "delivery" is selected for delivery method."
Code: 
    const orderMinsu = new Order("Minsu", "large", ["olive", "mushroom"], ["pepperoni"], "delivery");
    orderMinsu.discountEligibility();
Expected: "No"

Describe: formatName()
 
Test: "It should return a name with the first letter in upper case and the rest in lower cases."
Code: formatName("elsa");
Expected: "Elsa"

Test: "It should return a name with the first letter in upper case and the rest in lower cases."
Code: formatName("ELSA");
Expected: "Elsa"
```
## Known Bugs
- No bugs detected currently. Feel free to reach out to the [author](mailto:hayeong.pyeon@gmail.com) if find any. 
- Last updated: December 13, 2023

## License
[MIT](/LICENSE.txt) Copyright © 2023 Hayeong Pyeon  
Icons used for background is downloaded from [Icons8](https://icons8.com/icon/7DNAxn61w5zi/pizza)