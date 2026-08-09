---
title: Exercise 3
---

# Exercise

## Level 3

1.  The following is an array of 10 students ages: js
    `const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]` - Sort the
    array and find the min and max age - Find the median age(one middle
    item or two middle items divided by two) - Find the average age(all
    items divided by number of items) - Find the range of the ages(max
    minus min) - Compare the value of (min - average) and (max -
    average), use abs() method

    ``` javascript
    const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
    ```

    - Finding minimum or maximum age

      ``` javascript
      const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
      let sorted = ages.sort((a, b) => a - b)
      ```

      ``` javascript
      const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
      let sorted = ages.sort((a, b) => a - b)
      console.log('Minimum Age : ' + sorted[0],'\n','Maximum Age : ' + sorted[sorted.length -1])
      ```

    - median age

      ``` javascript
      const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
      let sorted = ages.sort((a, b) => a - b)
      if (sorted.length % 2 !== 0) {
         let index = Math.floor(sorted.length / 2)
          console.log(sorted[index])
      }
      else {
          let lowerNum = Math.floor(sorted.length / 2)
          console.log((sorted[lowerNum] + sorted[lowerNum + 1]) / 2)
      }
      ```

    - Agerage age

      ``` javascript
      const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
      let sorted = ages.sort((a, b) => a - b)
      let total = 0;
      for (let i in ages) {
          total = total + ages[i]
      }
      let average = total / ages.length
      ```

      ``` javascript
      const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
      let sorted = ages.sort((a, b) => a - b)
      console.log(average)
      ```

    - Range of Age

      ``` javascript
      const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
      let sorted = ages.sort((a, b) => a - b)
      let range = sorted[sorted.length - 1] - sorted[0]
      console.log(range)
      ```

    - Compare Values

      - Minimum - Average

        ``` javascript
        const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
        let sorted = ages.sort((a, b) => a - b)
        let total = 0;
        for (let i in ages) {
            total = total + ages[i]
        }
        let average = total / ages.length
        let value = Math.abs(sorted[0] - average)
        console.log(value)
        ```

      - Maximux - Average

        ``` javascript
        const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
        let sorted = ages.sort((a, b) => a - b)
        let total = 0;
        for (let i in ages) {
            total = total + ages[i]
        }
        let average = total / ages.length
        let value = Math.abs(sorted[sorted.length - 1] - average)
        console.log(value)
        ```

2.  Slice the first ten countries in the countries array.

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
        'Kenya'
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
        'Kenya'
    ]
    console.log(countries.slice(0, 10))
    ```

3.  Find the middle countries in the countries array.

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
        'Kenya'
    ]
    let index = Math.floor(countries.length / 2)
    if (countries.length % 2 === 0) {
        console.log(countries[index], countries[index + 1])
    }
    else {
        console.log(countries[index])
    }
    ```

4.  Divide the countries array into two equal arrays if it is even. If
    country array is not even, one or more countries for the first half.

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
        'Kenya'
    ]
    let index = Math.floor(countries.length / 2)
    if (countries.length % 2 === 0) {
        let firstHalf = countries.splice(0, index)
        console.log(firstHalf, countries)
    }
    else {
        let firstHalf = countries.splice(0, index + 2)
        console.log(firstHalf, countries)
    }
    ```
