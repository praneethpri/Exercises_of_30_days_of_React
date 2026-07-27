---
title: Exercise 1
---

# Exercise

## Level 1

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

const webTechs = [
    'HTML',
    'CSS',
    'JavaScript',
    'React',
    'Redux',
    'Node',
    'MongoDB'
]
```

1.  Declare an empty array.

    ``` javascript
    let arr = Array()
    ```

2.  Declare an array with more than 5 number of elements.

    ``` javascript
    let fruits = ['banana', 'lemon', 'cherry', 'mango', 'orange']
    return fruits;
    ```

3.  Find the length of your array.

    ``` javascript
    console.log(fruits.length)
    ```

4.  Get the first item, the middle item and the last item of the array.

    ``` javascript
    console.log(fruits[0])
    console.log(fruits[Math.floor(fruits.length / 2)])
    console.log(fruits[fruits.length - 1])
    ```

5.  Declare an array called *mixedDataTypes*, put different data types
    in the array and find the length of the array. The array size should
    be greater than 5.

    ``` javascript
    let mixedDataTypes = [
        'Sri Lanka',
        1948,
        ['Sri Lanka', 'India', 'Pakistan', 'Bangladesh', 'Nepal', 'Maldives', 'Afganistan'],
        {country: 'Sri Lanka', region: 'South Asia'},
        {southAsianCountries: ['Sri Lanka', 'India', 'Pakistan', 'Bangladesh', 'Nepal', 'Maldives', 'Afganistan']},
        [{capital: 'Sri Jayawardhanapura Kotte'}, {mainCity: 'Colombo'}]
    ]

    console.log(mixedDataTypes.length)
    ```

6.  Declare an array variable name itCompanies and assign initial values
    Facebook, Google, Microsoft, Apple, IBM, Oracle and Amazon.

    ``` javascript
    let itCompanies = [
        'Facebook',
        'Google',
        'Microsoft',
        'Apple',
        'IBM',
        'Oracle',
        'Amazon'
    ]

    return itCompanies;
    ```

7.  Print the array using console.log.

    ``` javascript
    console.log(itCompanies)
    ```

8.  Print the number of companies in the array.

    ``` javascript
    console.log(itCompanies.length)
    ```

9.  Print the first company, middle and last company.

    ``` javascript
    console.log(itCompanies[0])
    console.log(itCompanies[Math.floor(itCompanies.length / 2)])
    console.log(itCompanies[itCompanies.length - 1])
    ```

10. Print out each company.

    ``` javascript
    for (let i = 0; i < itCompanies.length; i++) {
        console.log(itCompanies[i])
    }
    ```

11. Change each company name to uppercase one by one and print them out.

    ``` javascript
    for (let i in itCompanies) {
        console.log(itCompanies[i].toUpperCase())
    }
    ```

12. Print the array like a sentence: Facebook, Google, Microsoft, Apple,
    IBM, Oracle and Amazon are big IT companies.

    ``` javascript
    let arr = Array();
    for (let i = 0; i < itCompanies.length - 2; i++) {
     arr.push(itCompanies[i])
    }
    let string = arr.join(', ')

    let sentence = `${string}, ${itCompanies[itCompanies.length - 2]} and ${itCompanies[itCompanies.length -1]} are big IT companies.`
    console.log(sentence)
    ```

13. Check if a certain company exists in the itCompanies array. If it
    exist return the company or else return a company is not found.

    ``` javascript
    let checkCompany = 'Google'
    if (itCompanies.includes(checkCompany)) {
        console.log(checkCompany)
    }
    else {
        console.log('company is not found')
    }
    ```

14. Filter out companies which have more than one 'o' without the filter
    method.

    ``` javascript
    let companiesWithMoreThanOneO = Array();
    for (let j in itCompanies) {
        let splittedArr = itCompanies[j].split('')
        let countOfLetterO = 0;
        for (let k in splittedArr) {
            if (splittedArr[k] === 'o') {
                countOfLetterO++
            }
        }
        if (countOfLetterO > 1) {
            companiesWithMoreThanOneO.push(itCompanies[j])
        }
    }
    console.log(companiesWithMoreThanOneO)
    ```

15. Sort the array using the sort() method.

    ``` javascript
    console.log(itCompanies.sort())
    ```

16. Reverse the array using reverse() method.

    ``` javascript
    console.log(itCompanies.reverse())
    ```

17. Slice out the first 3 companies in the array.

    ``` javascript
    console.log(itCompanies.slice(3, itCompanies.length))
    ```

18. Slice out the last 3 companies from the array.

    ``` javascript
    console.log(itCompanies.slice(0, itCompanies.length - 3))
    ```

19. Slice out the middle IT company or companies from the array.

    ``` javascript
    let middleNumber = itCompanies.length / 2
    if (itCompanies.indexOf(middleNumber) !== -1) {
        let newArr = itCompanies.slice(Math.floor(middleNumber) - 1, Math.floor(middleNumber) + 1)
        console.log(newArr)
    }
    else {
        let newArr = itCompanies.slice(Math.floor(middleNumber), Math.floor(middleNumber) + 1)
        console.log(newArr)
    }
    ```

20. Remove the first IT company from the Array.

    ``` javascript
    let newArray = itCompanies.shift()
    console.log(itCompanies)
    ```

21. Remove the middle IT company or companies from the Array.

    ``` javascript
    let middleNumber = itCompanies.length / 2
    if (itCompanies.indexOf(middleNumber) !== -1) {
        let newArray = itCompanies.splice(Math.floor(middleNumber) - 1, 2)
    }
    else {
        let newArray = itCompanies.splice(Math.floor(middleNumber), 1)
    }
    console.log(itCompanies)
    ```

22. Remove the last IT company from the Array.

    ``` javascript
    let newArray = itCompanies.pop()
    console.log(itCompanies)
    ```

23. Remove all IT companies.

    ``` javascript
    let newArr = itCompanies.splice()
    console.log(newArr)
    ```
