---
title: Exercise 3
---

# Exercise

### Level 3

1.  Write a program which tells the number of days in a month.

    ``` javascript
    Enter a month: January
    January has 31 days.

    Enter a month: JANUARY
    January has 31 day

    Enter a month: February
    February has 28 days.

    Enter a month: FEbruary
    February has 28 days.
    ```

    ``` javascript
    let insertMonth = 'September'

    switch (insertMonth) {
        case 'january':
            console.log('January has 31 days.')
            break;
        case 'february':
            console.log('February has 28 days.')
            break;
        case 'march':
            console.log('March has 31 days.')
            break;
        case 'april':
            console.log('April has 30 days.')
            break;
        case 'june':
            console.log('June has 30 days.')
            break;
        case 'july':
            console.log('July has 31 days.')
            break;
        case 'august':
            console.log('August has 31 days.')
            break;
        case 'september':
            console.log('September has 30 days.')
            break;
        case 'october':
            console.log('October has 31 days.')
            break;
        case 'november':
            console.log('November has 30 days.')
            break;
        case 'december':
            console.log('December has 31 days.')
            break;
        default:
            console.log('This is not a month.')
            break;
    }
    ```

2.  Write a program which tells the number of days in a month, now
    consider leap year.

    ``` javascript
    let year = 2024
    let insertMonth = 'February'

    switch (insertMonth.toLowerCase()) {
        case 'january':
            console.log('January has 31 days.')
            break;
        case 'february':
            if (year % 4 === 0) {
                console.log('February has 29 days.')
            }
            else {
                console.log('February has 28 days.')
            }
            break;
        case 'march':
            console.log('March has 31 days.')
            break;
        case 'april':
            console.log('April has 30 days.')
            break;
        case 'june':
            console.log('June has 30 days.')
            break;
        case 'july':
            console.log('July has 31 days.')
            break;
        case 'august':
            console.log('August has 31 days.')
            break;
        case 'september':
            console.log('September has 30 days.')
            break;
        case 'october':
            console.log('October has 31 days.')
            break;
        case 'november':
            console.log('November has 30 days.')
            break;
        case 'december':
            console.log('December has 31 days.')
            break;
        default:
            console.log('This is not a month.')
            break;
    }
    ```
