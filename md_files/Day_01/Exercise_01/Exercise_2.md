---
title: Exercise 2
---

# Exercise

## Level 2

1.  Create a separate countries.js file and store the countries array
    into this file, create a separate file web<sub>techs</sub>.js and
    store the webTechs array into this file. Access both file in main.js
    file

    [Countries.js File](Level_2_Exercise/countries.js)
    [Web<sub>Techs</sub>.js File](Level_2_Exercise/Web_Techs.js)
    [Main.js File](Level_2_Exercise/main.js)

    - countries.js file

      ``` javascript
      const countries = [
        'Albania',
        'Bolivia',
        'Canada',
        'Denmark',
        'Ethiopia',
        'Finland',
        'Germany',
        'Hungary',
        'Ireland',
        'Japan',
        'Kenya',
      ]

      module.exports = countries;
      ```

2.  web<sub>techs</sub>.js file

    ``` javascript
    const webTechs = [
      'HTML',
      'CSS',
      'JavaScript',
      'React',
      'Redux',
      'Node',
      'MongoDB',
    ]

    module.exports = webTechs;
    ```

    - main.js file

      ``` javascript
      const countries = require('./countries.js');
      const webTechs = require('./Web_Techs.js');

      console.log(countries);
      console.log(webTechs);
      ```

3.  First remove all the punctuations and change the string to array and
    count the number of words in the array.

    ``` javascript
    let text = 'I love teaching and empowering people. I teach HTML, CSS, JS, React, Python.'
    console.log(text.split(/[., ]+/))
    ```

4.  In the following shopping cart add, remove, edit items.

    ``` javascript
    const shoppingCart = ['Milk', 'Toffee', 'Tea', 'Honey']
    ```

    - add 'Meat' in the beginning of your shopping cart if it has not
      been already added

      ``` javascript
      const shoppingCart = ['Milk', 'Toffee', 'Tea', 'Honey']
      if (!shoppingCart.includes('Meat')) {
          shoppingCart.unshift('Meat')
      }
      ```

      ``` javascript
      const shoppingCart = ['Milk', 'Toffee', 'Tea', 'Honey']
      if (!shoppingCart.includes('Meat')) {
          shoppingCart.unshift('Meat')
      }
      console.log(shoppingCart)
      ```

    - add 'Sugar' at the end of your shopping cart if it has not been
      already added

      ``` javascript
      const shoppingCart = ['Milk', 'Toffee', 'Tea', 'Honey']
      if (!shoppingCart.includes('Meat')) {
          shoppingCart.unshift('Meat')
      }
      if (!shoppingCart.includes('Sugar')) {
          shoppingCart.push('Sugar')
      }
      ```

      ``` javascript
      const shoppingCart = ['Milk', 'Toffee', 'Tea', 'Honey']
      if (!shoppingCart.includes('Meat')) {
          shoppingCart.unshift('Meat')
      }
      if (!shoppingCart.includes('Sugar')) {
          shoppingCart.push('Sugar')
      }
      console.log(shoppingCart)
      ```

    - Remove Honey if you are allergic to honey

      ``` javascript
      const shoppingCart = ['Milk', 'Toffee', 'Tea', 'Honey']
      if (!shoppingCart.includes('Meat')) {
          shoppingCart.unshift('Meat')
      }
      if (!shoppingCart.includes('Sugar')) {
          shoppingCart.push('Sugar')
      }
      let allergy = true
      if (allergy) {
          let num = shoppingCart.indexOf('Honey')
          let sliced = shoppingCart.splice(num)
          sliced.shift()
          sliced.forEach((i) => shoppingCart.push(i))
      }
      ```

      ``` javascript
      const shoppingCart = ['Milk', 'Toffee', 'Tea', 'Honey']
      if (!shoppingCart.includes('Meat')) {
          shoppingCart.unshift('Meat')
      }
      if (!shoppingCart.includes('Sugar')) {
          shoppingCart.push('Sugar')
      }
      let allergy = true
      if (allergy) {
          let num = shoppingCart.indexOf('Honey')
          let sliced = shoppingCart.splice(num)
          sliced.shift()
          sliced.forEach((i) => shoppingCart.push(i))
      }
      console.log(shoppingCart)
      ```

    - Modify 'Tea' to 'Green Tea'

      ``` javascript
      const shoppingCart = ['Milk', 'Toffee', 'Tea', 'Honey']
      if (!shoppingCart.includes('Meat')) {
          shoppingCart.unshift('Meat')
      }
      if (!shoppingCart.includes('Sugar')) {
          shoppingCart.push('Sugar')
      }
      let allergy = true
      if (allergy) {
          let num = shoppingCart.indexOf('Honey')
          let sliced = shoppingCart.splice(num)
          sliced.shift()
          sliced.forEach((i) => shoppingCart.push(i))
      }
      let index = shoppingCart.indexOf('Tea')
      shoppingCart[index] = 'Green Tea'
      console.log(shoppingCart)
      ```

5.  In countries array check if 'Ethiopia' exists in the array if it
    exists print 'ETHIOPIA'. If it does not exist add to the countries
    list.

    ``` javascript

    const countries = [
      'Albania',
      'Bolivia',
      'Canada',
      'Denmark',
      'Ethiopia',
      'Finland',
      'Germany',
      'Hungary',
      'Ireland',
      'Japan',
      'Kenya',
    ]
    ```

    ``` javascript

    const countries = [
      'Albania',
      'Bolivia',
      'Canada',
      'Denmark',
      'Ethiopia',
      'Finland',
      'Germany',
      'Hungary',
      'Ireland',
      'Japan',
      'Kenya',
    ]

    if (countries.includes('Ethiopia')) {
        console.log(countries[countries.indexOf('Ethiopia')].toUpperCase())
    }
    else {
        countries.push('Ethiopia')
    }
    ```

6.  In the webTechs array check if Sass exists in the array and if it
    exists print 'Sass is a CSS preprocess'. If it does not exist add
    Sass to the array and print the array.

    ``` javascript
    const webTechs = [
      'HTML',
      'CSS',
      'JavaScript',
      'React',
      'Redux',
      'Node',
      'MongoDB',
    ]
    ```

    ``` javascript
    const webTechs = [
      'HTML',
      'CSS',
      'JavaScript',
      'React',
      'Redux',
      'Node',
      'MongoDB',
    ]
    if (webTechs.includes('Sass')) {
        console.log('Sass is a CSS preprocess')
    }
    else {
        webTechs.push('Sass')
    }
    console.log(webTechs)
    ```

7.  Concatenate the following two variables and store it in a fullstack
    variable

    ``` javascript
    const frontEnd = ['HTML', 'CSS', 'JS', 'React', 'Redux']
    const backEnd = ['Node', 'Express', 'MongoDB']

    let fullStack = frontEnd.concat(backEnd);
    console.log(fullStack)
    ```
