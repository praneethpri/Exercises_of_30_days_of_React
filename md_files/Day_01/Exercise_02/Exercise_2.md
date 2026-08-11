---
title: Exercise 2
---

# Exercise

## Level 2

1.  Write a code which can give grades to students according to theirs
    scores:

    - 80 - 100 : A

    - 70 - 89 : B

    - 60 - 69 : C

    - 50 - 59 : D

    - 0 - 49 : F

      ``` javascript
      let score = 67

      if (score >= 80 && score <= 100) {
          console.log('A')
      }
      else if (score >= 70 && score <= 89) {
          console.log('B')
      }
      else if (score >= 60 && score <= 69) {
          console.log('C')
      }
      else if (score >= 50 && score <= 59) {
          console.log('D')
      }
      else if (score >= 0 && score <= 49) {
          console.log('F')
      }
      else {
          console.log('Not a valid score')
      }
      ```

2.  Check if the season is Autumn, Winter, Spring or Summer. If the user
    input is:

    - September, October or November, the season is Autumn.

    - December, January or February, the season is Winter.

    - March, April or May, the season is Spring.

    - June, July or August, the season is Summer.

      ``` javascript
      let month = 'March'

      switch (month) {
          case 'September' || 'October' || 'November':
              console.log('The season is Autumn')
              break;
          case 'December' || 'January' || 'February':
              console.log('The season is Winter')
              break;
          case 'March' || 'April' || 'May':
              console.log('The season is Spring')
              break;
          case 'June' || 'July' || 'August':
              console.log('The season is Summer')
              break;
          default:
              console.log('This is not a month')
              break;
      }
      ```

3.  Check if a day is weekend day or a working day. Your script will
    take day as an input.

    ``` javascript
    What is the day  today? Saturday
    Saturday is a weekend.

    What is the day today? saturDaY
    Saturday is a weekend.

    What is the day today? Friday
    Friday is a working day.

    What is the day today? FrIDAy
    Friday is a working day.
    ```

    ``` javascript
    let inputDay = 'Wednesday'

    switch (inputDay.toLowerCase()) {
        case 'monday':
            console.log('Monday is a working day.')
            break;
        case 'tuesday':
            console.log('Tuesday is a working day.')
            break;
        case 'wednesday':
            console.log('Wednesday is a working day')
            break;
        case 'thursday':
            console.log('Thursday is a working day')
            break;
        case 'friday':
            console.log('Friday is a working day')
            break;
        case 'saturday':
            console.log('Saturday is a weekend')
            break;
        case 'sunday':
            console.log('Sunday is a weekend')
            break;
        default:
            console.log('This is not a proper day')
    }
    ```
