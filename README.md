# Google-Developer-Challenge
On the way to greatness; year 2017; Udacity and Google announcing over 100k scholarships around the world.
<br>
I have accomplished the program and here to share the code, skipping all super trivial:
# Quiz: Even or Odd (3-2)
Directions:
Write an if...else statement that:

prints "even" if the number is an even number
prints "odd" if the number is an odd number
Hint: Use the % (modulo) operator to determine if a number is even or odd. The modulo operater takes two numbers and returns the remainder when the first number is divided by the second one:

console.log(12 % 3);
console.log(10 % 4);
Result: 
0 
2

The answer for 12 % 3 is 0 because twelve divided by three has no remainder. 10 % 4 is 2 because ten divided by 4 has a remainder of two.
Make sure to test your code with different values. For example:

If number equals 1, then odd should be printed to the console.
If number equals 12, then even should be printed to the console.

Your code:
```
/*
 * Programming Quiz: Even or Odd (3-2)
 *
 * Write an if...else statement that prints `even` if the 
 * number is even and prints `odd` if the number is odd.
 *
 * Note - make sure to print only the string "even" or the string "odd"
 */
 
// change the value of `number` to test your if...else statement
var number = 1;
var message;
if (number%2 === 0) {
    message = "even";
} else {
message = "odd";
}
console.log(message);
```
# Quiz: Musical Groups (3-3)
Musical groups have special names based on the number of people in the group.

For example, a "quartet" is a musical group with four musicians. Barbershop quartets were a popular type of quartet in the early 1900s and featured four singers made up of a lead, tenor, baritone, and bass.

Directions:
Write a series of conditional statements that:

prints "not a group" if musicians is less than or equal to 0
prints "solo" if musicians is equal to 1
prints "duet" if musicians is equal to 2
prints "trio" if musicians is equal to 3
prints "quartet" if musicians is equal to 4
prints "this is a large group" if musicians is greater than 4
TIP: Make sure to test your code with different values. For example,

If musicians equals 3, then trio should be printed to the console.
If musicians equals 20, then this is a large group should be printed to the console.
If musicians equals -1, then not a group should be printed to the console.

Your Code:
```
/*
 * Programming Quiz: Musical Groups (3-3)
 */
 
// change the value of `musicians` to test your conditional statements

var musicians = 20;
var message;
// your code goes here
if(musicians <= 0 ){
    message = "not a group"
}else if(musicians === 1){
    message ="solo";
}else if(musicians === 2){
    message ="duet";
}
else if(musicians === 3){
    message ="trio";
}
else if(musicians === 4){
    message ="quartet";
}else if(musicians > 4){
    message ="this is a large group";
}
console.log(message);
```
# Quiz: Murder Mystery (3-4)

Directions:
For this quiz, you're going to help solve a fictitious murder mystery that happened here at Udacity! A murder mystery is a game typically played at parties wherein one of the partygoers is secretly, and unknowingly, playing a murderer, and the other attendees must determine who among them is the criminal. It's a classic case of whodunnit.

Since this might be your first time playing a murder mystery, we've simplified things quite a bit to make it easier. Here's what we know! In this murder mystery there are:

four rooms: the ballroom, gallery, billiards room, and dining room,
four weapons: poison, a trophy, a pool stick, and a knife,
and four suspects: Mr. Parkes, Ms. Van Cleve, Mrs. Sparr, and Mr. Kalehoff.
We also know that each weapon corresponds to a particular room, so...

the poison belongs to the ballroom,
the trophy belongs to the gallery,
the pool stick belongs to the billiards room,
and the knife belongs to the dining room.
And we know that each suspect was located in a specific room at the time of the murder.

Mr. Parkes was located in the dining room.
Ms. Van Cleve was located in the gallery.
Mrs. Sparr was located in the billiards room.
Mr. Kalehoff was located in the ballroom.
To help solve this mystery, write a combination of conditional statements that:

sets the value of weapon based on the room and
sets the value of solved to true if the value of room matches the suspect's room
Afterwards, print the following to the console if the mystery was solved:

__________ did it in the __________ with the __________!
Fill in the blanks with the name of the suspect, the room, and the weapon. For example,

Mr. Parkes did it in the dining room with the knife!
TIP: Make sure to test your code with different values. For example,

If room equals gallery and suspect equals Ms. Van Cleve, then Ms. Van Cleve did it in the gallery with the trophy! should be printed to the console.

Your Code:
```
/*
 * Programming Quiz: Murder Mystery (3-4)
 */

// change the value of `room` and `suspect` to test your code

var room = "dining room";
var suspect = "Mr. Parkes";

var weapon = "";
var solved = false;

if (room === "ballroom") {
    weapon = "poison"; solved = suspect === "Mr. Kalehoff";
} else if (room === "gallery") {
    weapon = "trophy"; solved = suspect === "Ms. Van Cleve";
} else if (room === "billiards room") {
    weapon = "pool stick"; solved = suspect === "Mrs. Sparr";
} else {
    weapon = "knife"; solved = suspect === "Mr. Parkes";
}

if (solved) {
    console.log(`${suspect} did it in the ${room} with the ${weapon}!`);
}
```
# Quiz: Checking your Balance (3-5)
Using the flowchart below, write the code to represent checking your balance at the ATM. The yellow diamonds represent conditional statements and the blue rectangles with rounded corners represent what should be printed to the console.
![atm-check-balance-cropped](https://user-images.githubusercontent.com/25347909/34531827-5730e222-f0bc-11e7-9af8-b6dc13398e5c.jpeg)
Use the following variables in your solution:

balance - the account balance
isActive - if account is active
checkBalance - if you want to check balance
Hint: The variable balance could be a value less than, greater than, or equal to 0. The variables isActive and checkBalance are booleans that can be set to true or false.

TIP: To print out the account balance with decimal points (i.e. 325.00), use the .toFixed() method and pass it the number of decimal points you want to use. For example, balance.toFixed(2) returns 325.00.
TIP: Make sure to test your code with different values. For example,

If checkBalance equals true and isActive equals false, then Your account is no longer active. should be printed to the console.

Your Code:
```
// change the values of balance, checkBalance, and isActive to test your code

var balance = -59.00;
var checkBalance = true;
var isActive = true;

// your code goes here

if (checkBalance === true && isActive === true && balance > 0) {
console.log("Your balance is $" + balance + ".");
} if (checkBalance === false){
console.log("Thank you. Have a nice day!");
} if (checkBalance === true && isActive === false){
console.log("Your account is no longer active.");
} if (checkBalance === true && (isActive === true && balance === 0)) {
console.log("Your account is empty.");
} else if (checkBalance === true && isActive === true && balance < 0) {
console.log("Your balance is negative. Please contact bank.");
}
```
# Quiz: Ice Cream (3-6)

Directions:
Ice cream is one of the most versatile desserts on the planet because it can be done up so many different ways. Using logical operators, write a series of complex logical expressions that prints only if the following conditions are true:

if flavor is set to vanilla or chocolate and
if vessel is set to cone or bowl and
if toppings is set to sprinkles or peanuts
If the above conditions are true, then print out:

I'd like two scoops of __________ ice cream in a __________ with __________.
Fill in the blanks with the flavor of the ice cream, vessel, and toppings. For example,

I'd like two scoops of vanilla ice cream in a cone with peanuts.
TIP: Make sure to test your code with different values. For example,

If flavor equals "chocolate", vessel equals "cone" and toppings equals "sprinkles", then "I'd like two scoops of chocolate ice cream in a cone with sprinkles." should be printed to the console.

Your Code:
```
/*
 * Programming Quiz: Ice Cream (3-6)
 *
 * Write a single if statement that logs out the message:
 * 
 * "I'd like two scoops of __________ ice cream in a __________ with __________."
 * 
 * ...only if:
 *   - flavor is "vanilla" or "chocolate"
 *   - vessel is "cone" or "bowl"
 *   - toppings is "sprinkles" or "peanuts"
 *
 * We're only testing the if statement and your boolean operators. 
 * It's okay if the output string doesn't match exactly.
 */

// change the values of `flavor`, `vessel`, and `toppings` to test your code

var flavor = "strawberry";
var vessel = "cone";
var toppings = "sprinkles";
// Add your code here

if(flavor === "vanilla" ||flavor === "chocolate" && (vessel === "cone" ||vessel === "bowl") && (toppings === "sprinkles" ||toppings === "peanuts")){
    console.log("I'd like two scoops of "+flavor+" ice cream in a "+vessel+" with "+toppings+".");
}
```
# Quiz: What do I Wear? (3-7)

If you're like me, finding the right size t-shirt can sometimes be a challenge. What size am I? What's the difference between S (small), M (medium), and L (large)? I usually wear L, but what if I need an XL (extra large)?

Thankfully, our friends at Teespring have got us covered because they've created a sizing chart to make things a lot easier.

![tshirt-guide](https://user-images.githubusercontent.com/25347909/34531980-fcd8dac2-f0bc-11e7-8ed3-84796316c593.png)

Directions:
Use the sizing chart above, create a series of logical expressions that prints the size of a t-shirt based on the measurements of shirtWidth, shirtLength, and shirtSleeve. Valid sizes include S, M, L, XL, 2XL, and 3XL.

For example, if...

var shirtWidth = 23; // size L (large)
var shirtLength = 30; // size L (large)
var shirtSleeve = 8.71; // size L (large)
Then print L to the console.

Hint: You will need to compare a range of values when checking for shirtWidth, shirtLength, and shirtSleeve. For example, if the shirt's width is at least 20", but no more than 22", then the t-shirt should be medium (M) — as long as the other values for the shirt's length and sleeve measurements match up.

If shirtWidth, shirtLength, and shirtSleeve don't fit within the range of acceptable values for a specific size, then print N/A to the console. For example, if...

var shirtWidth = 18; // size S (small)
var shirtLength = 29; // size M (medium)
var shirtSleeve = 8.47; // size M (medium)
Then print N/A to the console because the measurements don't all match up with one particular size.

TIP: Make sure to test your code with different values. For example,

If shirtWidth equals 19, shirtLength equals 28 and shirtSleeve equals 8.21, then S should be printed to the console.
If shirtWidth equals 26, shirtLength equals 33 and shirtSleeve equals 9.63, then 2XL should be printed to the console.
If shirtWidth equals 18, shirtLength equals 29 and shirtSleeve equals 8.47, then N/A should be printed to the console.

Your code:
```
   var shirtWidth = 18;
   var shirtLength = 29;
   var shirtSleeve = 8.47;

   // your code goes here
   
   if ((shirtWidth >= 18 && shirtWidth < 20) && 
   (shirtLength >= 28 && shirtLength < 29) &&
       (shirtSleeve >= 8.13 && shirtSleeve < 8.38)) {
       console.log ("S");
   } else if ((shirtWidth >= 20 && shirtWidth < 22) &&
              (shirtLength >= 29 && shirtLength < 30) &&
              (shirtSleeve >= 8.38 && shirtSleeve < 8.63)) {
       console.log ("M");
   } else if ((shirtWidth >= 22 && shirtWidth < 24) &&
              (shirtLength >= 30 && shirtLength < 31) &&
              (shirtSleeve >= 8.63 && shirtSleeve < 8.88)) {
       console.log ("L");
   } else if ((shirtWidth >= 24 && shirtWidth < 26) &&
              (shirtLength >= 31 && shirtLength < 33) &&
              (shirtSleeve >= 8.88 && shirtSleeve < 9.63)) {
       console.log ("XL");
   } else if ((shirtWidth >= 26 && shirtWidth < 28) && 
              (shirtLength >= 33 && shirtLength < 34) && 
              (shirtSleeve >= 9.63 && shirtSleeve < 10.13)) {
       console.log ("2XL");
   } else if (shirtWidth === 28 &&
              shirtLength === 34 &&
              shirtSleeve === 10.13) {
       console.log ("3XL");
   } else {
       console.log ("N\/A");
   }
```
   # Quiz: Back to School (3-9)
   
   In 2015, the U.S. Bureau of Labor Statistics conducted research to reveal how average salary is directly related to the number of years spent in school. In their findings, they found that people with:

no high school diploma earned an average of $25,636/year,
a high school diploma earned an average of $35,256/year,
an Associate's degree earned an average of $41,496/year,
a Bachelor's degree earned an average of $59,124/year,
a Master's degree earned an average of $69,732/year,
a Professional degree earned an average of $89,960/year,
and a Doctoral degree earned an average of $84,396/year.
NOTE: Wondering what the average salary would be for a person with a Nanodegree from Udacity? That's a hard question to answer, but that doesn't mean we haven't tried to quantify the value of our Nanodegrees. Click here to read more about Nanodegrees from resident Udacity writer Chris Watkins.
Directions:
Write a switch statement to set the average salary of a person based on their type of completed education.

Afterwards, print the following to the console.

In 2015, a person with __________ earned an average of __________/year.
Fill in the blanks with the type of education and the expected average salary. Make sure to use correct grammar in your printed statement. For help, refer to the findings above.

In 2015, a person with a Bachelor's degree earned an average of $59,124/year.
TIP: To print out the average salary with commas (i.e. 59,124), use the toLocaleString() method and pass it the locale "en-US". For example, salary.toLocaleString("en-US").
TIP: Make sure to test your code with different values. For example,

If education equals "an Associate's degree", then In 2015, a person with an Associate's degree earned an average of $41,496/year. should be printed to the console.

Your code:
```
/*
 * Programming Quiz: Back to School (3-9)
 */

// change the value of `education` to test your code

var education = "no high school diploma";

// set the value of this based on a person's education

var salary;

// your code goes here

switch(education){
case "no high school diploma":
    salary = "In 2015, a person with no high school diploma earned an average of $25,636/year."
    break;
    case "a high school diploma":
    salary = "In 2015, a person with a high school diploma earned an average of $35,256/year."
    break;
    case "an Associate's degree":
    salary = "In 2015, a person with an Associate's degree earned an average of $41,496/year."
    break;
    case "a Bachelor's degree":
    salary = "In 2015, a person with a Bachelor's degree earned an average of $59,124/year."
    break;
    case "a Master's degree":
    salary = "In 2015, a person with a Master's degree earned an average of $69,732/year."
    break;
    case "a Professional degree":
    salary = "In 2015, a person with a Professional degree earned an average of $89,960/year."
    break;
    case "a Doctoral degree":
    salary = "In 2015, a person with a Doctoral degree earned an average of $84,396/year."
    break;
}
console.log(salary);
```
# Quiz: JuliaJames (4-1)

"Fizzbuzz" is a famous interview question used in programming interviews. It goes something like this:

Loop through the numbers 1 to 100
If the number is divisible by 3, print "Fizz"
If the number is divisible by 5, print "Buzz"
If the number is divisible by both 3 and 5, print "FizzBuzz"
If the number is not divisible by 3 or 5, print the number
TIP: A number x is divisible by a number y if the answer to x / y has a remainder of 0. For example, 10 is divisible by 2 because 10 / 2 = 5 with no remainder. You can check if a number is divisible by another number by checking if x % y === 0.
We're going to have you program your own version of FizzBuzz called "JuliaJames" (yes, imaginative, right?) Keep in mind that in an interview, you would want to write efficient code with very little duplication. We don't want you to worry about that for this question. Just focus on practicing using loops.

Directions:
Write a while loop that:

Loop through the numbers 1 to 20
If the number is divisible by 3, print "Julia"
If the number is divisible by 5, print "James"
If the number is divisible by 3 and 5, print "JuliaJames"
If the number is not divisible by 3 or 5, print the number

Your code:
```
/*
 * Programming Quiz: JuliaJames (4-1)
 */
 
var x = 1;
while (x <= 20) {
    if(x % 3===0 && x%5===0){
        console.log("JuliaJames");
    }
    else if(x % 3 === 0){
        console.log("Julia");
        }else if(x % 5 === 0){
          console.log("James");  
        }
        else{
            console.log(x)
        }
    x++;
}
```
# Quiz: 99 Bottles of Juice (4-2)

Directions:
Write a loop that prints out the following song. Starting at 99, and ending at 1 bottle.

99 bottles of juice on the wall! 99 bottles of juice! Take one down, pass it around... 98 bottles of juice on the wall!
98 bottles of juice on the wall! 98 bottles of juice! Take one down, pass it around... 97 bottles of juice on the wall!
...
2 bottles of juice on the wall! 2 bottles of juice! Take one down, pass it around... 1 bottle of juice on the wall!
1 bottle of juice on the wall! 1 bottle of juice! Take one down, pass it around... 0 bottles of juice on the wall!
Some Notes:

Note the pluralization of the word "bottle" when you go from 2 bottles to 1 bottle.
Your text editor may try to autocorrect your ellipses ... to the ellipses character … Do not use the ellipses character for this quiz.

Your Code:
```
/*
 * Programming Quiz: 99 Bottles of Juice (4-2)
 *
 * Use the following `while` loop to write out the song "99 bottles of juice".
 * Log the your lyrics to the console.
 *
 * Note
 *   - Each line of the lyrics needs to be logged to the same line.
 *   - The pluralization of the word "bottle" changes from "2 bottles" to "1 bottle" to "0 bottles".
 */
 

var num = 99;
var message = "";
while (num>0) {
    if(num > 2){
        num;
        var message = num+" bottles of juice on the wall! "+num+" bottles of juice! Take one down, pass it around... "+(num-1)+" bottles of juice on the wall!";
        
    }else if(num===2){
        var message = num+" bottles of juice on the wall! "+num+" bottles of juice! Take one down, pass it around... "+(num-1)+" bottle of juice on the wall!";
        
    }else{
        var message = num+" bottle of juice on the wall! "+num+" bottle of juice! Take one down, pass it around... "+(num-1)+" bottles of juice on the wall!";
    }
    num--
    
    console.log(message);
        }
```

# Quiz: Countdown, Liftoff! (4-3)

NASA's countdown to launch includes checkpoints where NASA engineers complete certain technical tasks. During the final minute, NASA has 6 tasks to complete:

Orbiter transfers from ground to internal power (T-50 seconds)
Ground launch sequencer is go for auto sequence start (T-31 seconds)
Activate launch pad sound suppression system (T-16 seconds)
Activate main engine hydrogen burnoff system (T-10 seconds)
Main engine start (T-6 seconds)
Solid rocket booster ignition and liftoff! (T-0 seconds)
NOTE: "T-50 seconds" read as "T-minus 50 seconds".
Directions:
Write a while loop that counts down from 60 seconds and:

If there's a task being completed, it prints out the task
If there is no task being completed, it prints out the time as T-x seconds
Use the task and time descriptions described above.

Your Code:
Your output should look like the following:

T-60 seconds
T-59 seconds
T-58 seconds
...
T-51 seconds
Orbiter transfers from ground to internal power
T-49 seconds
...
T-3 seconds
T-2 seconds
T-1 seconds
Solid rocket booster ignition and liftoff!

Your code:
```
/*
 * Programming Quiz: Countdown, Liftoff! (4-3)
 * 
 * Using a while loop, print out the countdown output above.
 */
var sec = 60;
var message = "";
while(sec>=0){
  if(sec===50){
      message = "Orbiter transfers from ground to internal power";
  }else if(sec===31){
      message = "Ground launch sequencer is go for auto sequence start";
  }else if(sec===16){
      message = "Activate launch pad sound suppression system";
  }else if(sec===10){
      message = "Activate main engine hydrogen burnoff system";
  }else if(sec===6){
      message = "Main engine start";
  }else if(sec===0){
      message = "Solid rocket booster ignition and liftoff!";
  }else{
    message = "T-"+sec+" seconds";
}
sec--;
console.log(message);
}
```
# Quiz: Find my Seat (4-8)
Directions:
![3213163359-a4952f4f18-o](https://user-images.githubusercontent.com/25347909/34532822-4fa27530-f0c0-11e7-8b97-6e1b1c770f8b.jpg)
Theater seats often display a row and seat number to help theatergoers find their seats. If there are 26 rows (0 to 25) and 100 seats (0 to 99) in each row, write a nested for loop to print out all of the different seat combinations in the theater.

Example output for row-seat information: output each row and seat number on a separate line

0-0
0-1
0-2
...
25-97
25-98
25-99
Your Code:
```
/*
 * Programming Quiz: Find my Seat (4-8)
 * 
 * Write a nested for loop to print out all of the different seat combinations in the theater.
 * The first row-seat combination should be 0-0 
 * The last row-seat combination will be 25-99
 * 
 * Things to note: 
 *  - the row and seat numbers start at 0, not 1
 *  - the highest seat number is 99, not 100
 */
for(var x = 0;x < 26; x++){
      for(var y = 0; y < 100; y++){
       console.log(x+"-"+y);
    }
}
```

# Quiz: Build a Triangle (5-3)

Directions:
For this quiz, you're going to create a function called buildTriangle() that will accept an input (the triangle at its widest width) and will return the string representation of a triangle. See the example output below.
```
buildTriangle(10);
```
Returns:
```
* 
* * 
* * * 
* * * * 
* * * * * 
* * * * * * 
* * * * * * * 
* * * * * * * * 
* * * * * * * * * 
* * * * * * * * * *
```
We've given you one function makeLine() to start with. The function takes in a line length, and builds a line of asterisks and returns the line with a newline character.
```
function makeLine(length) {
  var line = "";
  for (var j = 1; j <= length; j++) {
    line += "* "
  }
  return line + "\n";
}
```
You will need to call this makeLine() function in buildTriangle().

This will be the most complicated program you've written yet, so take some time thinking through the problem before diving into the code. What tools will you need from your JavaScript tool belt? Professionals plan out their code before writing anything. Think through the steps your code will need to take and write them down in order. Then go through your list and convert each step into actual code. Good luck!

Your Code:
```

// creates a line of * for a given length
function makeLine(length) {
    var line = "";
    for (var j = 1; j <= length; j++) {
        line += "* ";
    }
    return line + "\n";
}

// your code goes here.  Make sure you call makeLine() in your own code.
function buildTriangle(n){
    var triangle = "";
    for (var i = 1; i <= n; i++) {
        triangle += makeLine(i);
    }
    return triangle
}

// test your code by uncommenting the following line
console.log(buildTriangle(100));
```
# Quiz: Inline (5-6)
Directions:
Call the emotions() function so that it prints the output you see below, but instead of passing the laugh() function as an argument, pass an inline function expression instead.

emotions("happy", laugh(2)); // you can use your laugh function from the previous quizzes
Prints: "I am happy, haha!"

Your Code:
```
/*
 * Programming Quiz: Inline Functions (5-6)
 */

// don't change this code
function emotions(myString, myFunc) {
    console.log("I am " + myString + ", " + myFunc(2));
}
emotions("happy", function laugh(lols){
    var laughs = "";
    for(var x = 1; x<=lols; x++){
        laughs += "ha";
    }
    return laughs + "!";
});
```
# Quiz: Colors of the Rainbow (6-4)
Directions:
James was creating an array with the colors of the rainbow, and he forgot some colors. The standard rainbow colors are usually listed in this order:

var rainbow = ["Red", "Orange", "Yellow", "Green", "Blue", "Purple"];
but James had this:

var rainbow = ["Red", "Orange", "Blackberry", "Blue"];
Using only the splice() method, insert the missing colors into the array, and remove the color "Blackberry" by following these steps:

Remove "Blackberry"
Add "Yellow" and "Green"
Add "Purple"

Your Code:
```
/*
 * Programming Quiz: Colors of the Rainbow (6-4)
 */

var rainbow = ["Red", "Orange", "Blackberry", "Blue"];
rainbow.splice(-2,2,"Yellow","Green","Blue","Purple");
console.log(rainbow);
```
# Quiz: Quidditch Cup (6-5)
Directions:
Create a function called hasEnoughPlayers() that takes the team array as an argument and returns true or false depending on if the array has at least seven players.

Your Code:
```
/*
 * Programming Quiz: Quidditch Cup (6-5)
 */

// your code goes here

var team = ["Oliver Wood", "Angelina Johnson", "Katie Bell", "Alicia Spinnet", "George Weasley", "Fred Weasley", "Harry Potter"];
function hasEnoughPlayers(team){
    var teamLength = team.length;
    if(teamLength >= 7){
        return true;
    }else{
        return false;
    }
}
console.log(hasEnoughPlayers(team));
```
# Quiz: Nested Numbers (6-10)
Directions:
Use a nested for loop to take the numbers array below and replace all of the values that are divisible by 2 (even numbers) with the string "even" and all other numbers with the string "odd".

Your Code:
```
/*
 * Programming Quiz: Nested Numbers (6-10)
 *
 *   - The `numbers` variable is an array of arrays.
 *   - Use a nested `for` loop to cycle through `numbers`.
 *   - Convert each even number to the string "even"
 *   - Convert each odd number to the string "odd"
 */

var numbers = [
    [243, 12, 23, 12, 45, 45, 78, 66, 223, 3],
    [34, 2, 1, 553, 23, 4, 66, 23, 4, 55],
    [67, 56, 45, 553, 44, 55, 5, 428, 452, 3],
    [12, 31, 55, 445, 79, 44, 674, 224, 4, 21],
    [4, 2, 3, 52, 13, 51, 44, 1, 67, 5],
    [5, 65, 4, 5, 5, 6, 5, 43, 23, 4424],
    [74, 532, 6, 7, 35, 17, 89, 43, 43, 66],
    [53, 6, 89, 10, 23, 52, 111, 44, 109, 80],
    [67, 6, 53, 537, 2, 168, 16, 2, 1, 8],
    [76, 7, 9, 6, 3, 73, 77, 100, 56, 100]
];

// your code goes here
    for(var row = 0; row < numbers.length; row++){
    for(var column = 0; column < numbers[row].length; column++){
        numbers[row][column] = numbers[row][column] % 2 === 0 ? "even" : "odd";
      }
}
console.log(numbers);
```
# Quiz: Umbrella (7-1)
Directions:
Using the umbrella example from the previous video, see if you can follow the example open() method and create the close() method. It's alright if you have trouble at first! We'll go into more detail later in this lesson.

var umbrella = { 
  color: "pink",
  isOpen: false,
  open: function() { 
    if (umbrella.isOpen === true) {
      return "The umbrella is already opened!";
    } else {
      umbrella.isOpen = true;
      return "Julia opens the umbrella!";
    }
   }
};
TIP: Remember to put all of your object's properties and methods inside curly braces: var myObject = { greeting: "hello", name: "Julia" };. Also, remember that an object is just another data type. Just like how you would put a semicolon after a string variable declaration var myString = "hello";, don't forget to put a semi-colon at the end of your object's declaration.

Your Code:
```
/*
 * Programming Quiz: Umbrella (7-1)
 */

var umbrella = {
    color: "pink",
    isOpen: true,
    open: function() {
        if (umbrella.isOpen === true) {
            return "The umbrella is already opened!";
        } else {
            umbrella.isOpen = true;
            return "Julia opens the umbrella!";
        }
    },
    close: function(){
        if (umbrella.isOpen === true){
            umbrella.isOpen = false;
            return "Closed"
            
        }
    }
};
```
# Quiz: Menu Items (7-2)

Directions:
Create a breakfast object to represent the following menu item:

The Lumberjack - $9.95
eggs, sausage, toast, hashbrowns, pancakes
The object should contain properties for the name, price, and ingredients.

Your Code:
```
/*
 * Programming Quiz: Menu Items (7-2)
 */
var breakfast = {
    name: "The Lumberjack",
    price: "$9.95",
    ingredients: ["eggs", "sausage", "toast", "hashbrowns", "pancakes"]
};
```
# Quiz: Bank Accounts 1 (7-3)
Directions:
Using the given object:
```
var savingsAccount = {
  balance: 1000,
  interestRatePercent: 1,
  deposit: function addMoney(amount) {
    if (amount > 0) {
      savingsAccount.balance += amount;
    }
  },
  withdraw: function removeMoney(amount) {
    var verifyBalance = savingsAccount.balance - amount;
    if (amount > 0 && verifyBalance >= 0) {
      savingsAccount.balance -= amount;
    }
  }
};
```
add a printAccountSummary() method that returns the following account message:

Welcome!
Your balance is currently $1000 and your interest rate is 1%.

Your Code:
```
/*
 * Programming Quiz: Bank Accounts 1 (7-3)
 */

var savingsAccount = {
    balance: 1000,
    interestRatePercent: 1,
    deposit: function addMoney(amount) {
        if (amount > 0) {
            savingsAccount.balance += amount;
        }
    },
    withdraw: function removeMoney(amount) {
        var verifyBalance = savingsAccount.balance - amount;
        if (amount > 0 && verifyBalance >= 0) {
            savingsAccount.balance -= amount;
        }
    },
    printAccountSummary: function printAccountSummary(){
        if(savingsAccount.balance === 1000){
            var message = "Welcome!"+"\n"+"Your balance is currently $"+savingsAccount.balance+" and your interest rate is "+savingsAccount.interestRatePercent+"%.";
            return message;
        }
    }
};

console.log(savingsAccount.printAccountSummary());
```
# Quiz: Facebook Friends (7-5)
Directions:
Create an object called facebookProfile. The object should have 3 properties:

your name
the number of friends you have, and
an array of messages you've posted (as strings)
The object should also have 4 methods:

postMessage(message) - adds a new message string to the array
deleteMessage(index) - removes the message corresponding to the index provided
addFriend() - increases the friend count by 1
removeFriend() - decreases the friend count by 1

Your Code:
```
/*
 * Programming Quiz: Facebook Friends (7-5)
 */
var facebookProfile = {
  name: "Erik",
  friends: 200,
  messages: ["what","the","heck"],
  postMessage: function postMessage(message){
      facebookProfile.messages.push(message);
  },
  deleteMessage: function deleteMessage(index){
      facebookProfile.messages.splice(index, 1);
  },
  addFriend: function addFriend(){
      facebookProfile.friends++;
  },
  removeFriend: function removeFriend(){
      facebookProfile.friends--;
  }
};
```
# Quiz: Donuts Revisited (7-6)
Here is an array of donut objects.
```
var donuts = [
  { type: "Jelly", cost: 1.22 },
  { type: "Chocolate", cost: 2.45 },
  { type: "Cider", cost: 1.59 },
  { type: "Boston Cream", cost: 5.99 }
];
```
Directions:
Use the forEach() method to loop over the array and print out the following donut summaries using console.log.

Jelly donuts cost $1.22 each
Chocolate donuts cost $2.45 each
Cider donuts cost $1.59 each
Boston Cream donuts cost $5.99 each

Your Code:
```
/*
 * Programming Quiz: Donuts Revisited (7-6)
 */

var donuts = [
    { type: "Jelly", cost: 1.22 },
    { type: "Chocolate", cost: 2.45 },
    { type: "Cider", cost: 1.59 },
    { type: "Boston Cream", cost: 5.99 }
];

donuts.forEach(function summary(donuts){
    console.log(donuts.type+" donuts cost $"+donuts.cost+" each");
});
```

The final project I have made during the program: https://github.com/erikfenriz/Pixel-Art-Maker
