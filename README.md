# Google-Developer-Challenge
On the way to greatness; year 2017; Udacity and Google announcing over 100k scholarships around the world
<br>
Here is the code, starting with something not super trivial:
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
///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
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


