# Google-Developer-Challenge
On the way to greatness; year 2017; Udacity and Google announcing over 100k scholarships around the world.
<br>
I have accomplished the program and here to share the code is the code, starting with something not super trivial:
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
        var message = num+" bottles of juice on the wall! "+num+" bottles of juice! Take one down, pass it around... "+(num-1)+" bottles of juice on the wall!"
        
    }else if(num===2){
        var message = num+" bottles of juice on the wall! "+num+" bottles of juice! Take one down, pass it around... "+(num-1)+" bottle of juice on the wall!"
        
    }else{
        var message = num+" bottle of juice on the wall! "+num+" bottle of juice! Take one down, pass it around... "+(num-1)+" bottles of juice on the wall!"
    }
    num--
    
    console.log(message);
        }
