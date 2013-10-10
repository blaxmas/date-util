## Date-Util: Prototype utils for date object

- Date format function
- strtotime

### Using with Node.js
    $ npm install date-util
    
    require('date-util');

### Date Format

Flags:
- d:    Day of the month without leading zeros  
- dd:   Day of the month, 2 digits with leading zeros  
- ddd:  A textual representation of a day, three letters  
- dddd: A full textual representation of the day of the week  
- m:    Numeric representation of a month, without leading zeros  
- mm:   Numeric representation of a month, with leading zeros  
- mmm:  A short textual representation of a month, three letters  
- mmmm: A full textual representation of a month, such as January or March  
- yy:   A two digit representation of a year  
- yyyy: A full numeric representation of a year, 4 digits  
- h:    12-hour format of an hour without leading zeros  
- hh:   12-hour format of an hour with leading zeros  
- H:    12-hour format of an hour without leading zeros  
- HH:   24-hour format of an hour with leading zeros  
- M:    Minutes without leading zeros  
- MM:   Minutes with leading zeros  
- s:    Seconds, without leading zeros  
- ss:   Seconds, with leading zeros   
- l:    Milliseconds, 3 digits  
- L:    Milliseconds without leading zeros  
- t:    Lowercase Ante meridiem and Post meridiem, 1 digit  
- tt:   Lowercase Ante meridiem and Post meridiem, 2 digits  
- T:    Uppercase Ante meridiem and Post meridiem, 1 digit  
- TT:   Uppercase Ante meridiem and Post meridiem, 2 digits  
- Z:    Difference to Greenwich time (GMT) in hours, with "GMT" word  
- o:    Difference to Greenwich time (GMT) in hours, without "GMT" word  
- S:    English ordinal suffix for the day of the month, 2 characters  
	
####Examples
	new Date().format("yyyy/mm/dd");  

### strtotime
Parse about any English textual datetime description  
####Examples
	new Date().strtotime("+1 day");  
	new Date().strtotime("next month +1 day");  
	new Date().strtotime("last sunday");  

####Example with format
	new Date().strtotime("last sunday").format("yyyy/mm/dd");  
