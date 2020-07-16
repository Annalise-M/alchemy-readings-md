Class 07 Readings/ Notes:
___
    Domain Modeling:
    https://github.com/codefellows/domain_modeling#domain-modeling

    HTML: chpt. 6 - Tables

    JavaScript: chpt. 3 - Functions, Methods & Objects

---
    Tables:
        table structures | <table> | <tr> | <td>
        
        table headings | <th>

        long tables | <thead> | <tbody> | <tfoot>

    old code: width, spacing, border, background - pg. 137 - 138
---
    Functions, Methods & Objects:
-
    global objects: number objects | pg. 132

        isNan() | checks if the value is not a number
        toFixed() | rounds to specified number of decimal places - returns a string
        toPrecision() | rounds to total number of places - returns a string
        toExponential() | returns a string representing the number in exponential notation
-
    global objects: math object  | pg. 134

        Property | Description
        Math.PI | returns pi - approximately 3.14159265359

        Method | Description
        Math.round() | rounds number to the nearest integer
        Math.sqrt(n) | returns square root of positive number, e.g., Math.sqrt(9) returns3
        Math.cell() | rounds number up to the nearest integer
        Math.floor() | rounds number down to the nearest integer
        Math.random() | generates a random number between 0 -inclusive- and 1 -not inclusive-
-
    global objects: date object -and time- | pg. 137

        Method | Description
        getDate() / setDate() | returns/ sets the day of the month 1-31
        getDay() | returns teh day of the week 0-6
        getFullYear() / setFullYear() | returns/ sets the year -4 digits-
        getHours() / setHours() | returns/ sets the hours
        getMilliseconds() / setMilliseconds() | returns/ sets the milliseconds 0-999
        getMinutes() / setMinutes() | returns/ sets minutes 0-59
        getMonth() / setMonth() | returns/ sets month 0-11
        getSeconds() / getSeconds() | returns/ sets seconds 0-59
        getTime() / setTime() | number of milliseconds since January 1, 1970, 00:00:00 UTC -coordinated universal time- and a negative number for any time before
        getTimezoneOffset() | returns time zone offset in mins for locale
        toDateString() | returns 'date' as a human-readable string
        toTimeString() | returns 'time' as a human-readable string
        toString() | returns a string representing the specified date
