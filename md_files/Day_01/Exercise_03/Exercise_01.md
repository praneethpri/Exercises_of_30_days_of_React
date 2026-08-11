---
title: Exercise 01
---

# Exercise

## Level 1

1.  Create an empty object called dog.

    ``` javascript
    const dog = {}
    ```

2.  Print the dog object on the console.

    ``` javascript
    const dog = {}
    console.log(dog)
    ```

3.  Add name, legs, color, age and bark properties for the dog object.
    The bark property is a method which return woof woof

    ``` javascript
    const dog = {}
    dog.name = 'Lassie'
    dog.leg = 4
    dog.color = 'Brown'
    dog.bark = 'woof woof'
    ```

    ``` javascript
    console.log(dog)
    ```

4.  Get name, legs, color, age and bark value from the dog object

    ``` javascript
    const dog = {}
    dog.name = 'Lassie'
    dog.leg = 4
    dog.color = 'Brown'
    dog.bark = 'woof woof'
    console.log(dog.name, dog.leg, dog.color, dog.bark)
    ```

5.  Set new properties the dog object: breed, getDogInfo

    ``` javascript
    const dog = {}
    dog.name = 'Lassie'
    dog.leg = 4
    dog.color = 'Brown'
    dog.bark = 'woof woof'
    dog.getDogInfo = function () {
        return `This dog's name is ${this.name} and she has ${this.leg} legs, with ${this.color} color wool and a lovely ${this.bark} sound.`
    }
    console.log(dog.getDogInfo())
    ```
