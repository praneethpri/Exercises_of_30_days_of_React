---
title: Exercise 1
---

# Exercise

### Level 1

1.  Get user input using prompt(“Enter your age:”). If user is 18 or
    older , give feedback:'You are old enough to drive' but if not 18
    give another feedback stating to wait for the number of years he
    needs to turn 18.

    ``` javascript
    Enter your age: 30
    You are old enough to drive.

    Enter your age:15
    You are left with 3 years to drive.
    ```

    ``` javascript
    let enteredAge = 30

    if (enteredAge >= 18) {
        console.log('You are old enough to drive.')
    }
    else {
        let leftAge = 18 - enteredAge
        console.log(`You are left with ${leftAge} years to drive`)
    }
    ```

2.  Compare the values of myAge and yourAge using if … else. Based on
    the comparison and log the result to console stating who is older
    (me or you). Use prompt(“Enter your age:”) to get the age as input.

    ``` javascript
    Enter your age: 30
    You are 5 years older than me.
    ```

    ``` javascript
    const myAge = 28

    let yourAge = 45

    if (yourAge > myAge) {
        let difference = yourAge - myAge
        console.log(`You are ${difference} years older than me.`)
    }
    else if (yourAge === myAge) {
        console.log('You are same age as me.')
    }
    else {
        let difference = myAge - yourAge
        console.log(`You are ${difference} year younger than me.`)
    }
    ```

3.  If a is greater than b return 'a is greater than b' else 'a is less
    than b'. Try to implement it in two ways

    ``` javascript
    let a = 4
    let b = 3
    ```

    - using if else

      ``` javascript
      let a = 4
      let b = 3
      if (a > b) {
          console.log(`${a} is greater than ${b}`)
      }
      else {
          console.log(`${b} is greater than ${a}`)
      }
      ```

    - using ternary operators

      ``` javascript
      let a = 4
      let b = 3
      a > b ? console.log(`${a} is greater than ${b}`) : console.log(`${b} is greater than ${a}`)
      ```

4.  Even numbers are divisible by 2 and the remainder is zero. How do
    you check, if a number is even or not using JavaScript?

    ``` javascript
    Enter a number: 2
    2 is an even number

    Enter a number: 9
    9 is is an odd number.
    ```

    ``` javascript
    let num = 2
    if (num % 2 === 0) {
        console.log(`${num} is an even number`)
    }
    else {
        console.log(`${num} is an odd number`)
    }
    ```

    ``` javascript
    let num = 9
    num % 2 === 0 ? console.log(`${num} is an even number`) : console.log(`${num} is an odd number`)
    ```
