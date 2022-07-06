# Debugging Activity
/**
 * Description: This program is locked into an infinite loop. Your task is to run and debug the program. 
 * 
 * TODO: The program should exit the loop after counting down from 5 to 1. You should check to make sure the boolean statement
 * is being updated.
 */

function checkPoint1() {
    alert1();
    
    let array = [];
    let x = 0;

    // TODO: Remove the bugs from the code below.
    function getMultiples() {
        while (x <= 50, x++){
            array.push(x * 2);
        }
        return array;
    }
    console.log(getMultiples()); 

    // DO NOT CHANGE THE CODE BELOW
    alert2();
}


/************************************************ DONT CHANGE THE CODE BELOW ******************************************************/
function alert1() {
    alert("Oh no! It looks like you are trapped in an infinite loop. Go to the example1.js file and work on checkpoint 1.");
}

function alert2(){
    alert("Congratulations! You have passed checkpoint 1!");
}

/**
 * Description: This program is assigning student IDs to 5 new students but there is a bug in the code preventing the code to run 
 * as expected. Your task is to run and debug the program using breakpoints.
 * 
 * TODO: The program has error message in the console. You should read the message and debug accordingly. The final 
 * goal is to print out a student ID for each student to the console. The ID numbers should be from 0 to 4.
 */

function checkPoint2(){
    alert3();

    // TODO: Remove the bugs from the code below.
    const friends = ["Rei", "Miya", "Alexis", "Ethan", "Anna"];
    const studentID = [];

    for (var i = 0; i < friends.length; i++){
        studentID.push("JSMIT" + i);
    }
    console.log(studentID);

    // DO NOT CHANGE THE CODE BELOW
    alerts(studentID);
}


/************************************************ DONT CHANGE THE CODE BELOW ******************************************************/
function alert3() {
    alert("All students need to get their student IDs, but it seems like the system is down. Can you help debug the system? Go to the example2.js file and work on checkpoint 2.");
}

function alerts(studentID) {
    if (studentID.length == 5) {
        alert("Yay! You got the system running!");
    }
    else {
        alert("Hmmm! It seems like Rei hasn't received his ID. Keep debugging!");
    }
}

/**
 * Description: This program is calculating the amount of change given to the customer after buying groceries but there is a bug 
 * in the code preventing the code to run as expected. Your task is to run and debug the program using the console to print 
 * statements.
 * 
 * TODO: The program currently displays NaN in the console as the returned change. You should check and make sure the function 
 * is reading the passed parameters.
 */

function checkPoint3(){
    alert4();

    // TODO: Remove the bugs from the code below.
    function superMarket(cash) {
        let milk = 4.99;
        let vegetables = 15.99;
        let bread = 2.99;

        let total = milk + vegetables + bread; 
        cash = cash - total;

        return cash;
    }

    function main(cash) {
        let moneySpent = superMarket(cash);
        return moneySpent;
    }

    let totalCash = 50.00;
    console.log("Total Cash: $" + totalCash);
    console.log("Change Return = $" + main(totalCash));


    // DO NOT CHANGE THE CODE BELOW
    if (main(totalCash) < 50) {
        alert("Awesome work! You got the system running!");
    }
}


/************************************************ DONT CHANGE THE CODE BELOW ******************************************************/
function alert4() {
    alert("The system at the supermarket doesn't seem to be working. Can you help debug the system to help calculate the total change return to the customer? Go to the example3.js file and work on checkpoint 3.");
}

/**
 * Description: This program is asking the user to create a new password for their account but there is a bug 
 * in the code preventing the code to run as expected. Your task is to run and debug the program by reading the error message.
 * 
 * TODO: The program has an error message in the console. You should read the message and debug accordingly.
 */

function checkPoint4() {
    // TODO: Remove the bugs from the code below.
    let password = ""
    while (password.length != 10) {
        password = prompt("New password must be 10 characters: "); 
    }
    alert("Your new password: " + password);
}