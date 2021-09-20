<== [HOME](README.md)

# WHILE loop
* run WHILE loop when you don't necessarily know how many loops we need to run
* have to set initial value first before entering the WHILE loop (e.g.'pls enter a number', see if >10)


* let userAnswer = 'no'
* while(userAnswer != 'yes'){
*       user Answer = prompt ('pls enter yes')}


# FOR loop
* for (var i=0; i<=12; i=i+1){
*   console.log(i * 8);
* }

## [Expressions and Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operatorsv)
>function randomnumber(){
    //100 is inclusive, 0 not inlcuded
    let randomnum = Math.floor(Math.random()*100) + 1;
    return "Your lucky number today is " + randomnum
}

function guessinggame(){
    correctanswer = randomnumber();
    console.log(randomnumber);
    //console.log is for testing and double checking
    let guesses = 3;
    for(let i=0; i<guesses; i++){
        //i++ add one each time
        let guessesLeft = guesses - i;
        let userGuess = parseInt(prompt('Please enter an integer between 1 and 100. You have '+ guessesLeft + ' tries left!'));
        while(userGuess<1 || userGuess>100){
            userGuess = parseInt(prompt('Try Again! Did you enter an integer between 1 and 100?'));
        }
        if(userGuess == correctanswer){
            alert('WAHOO! YOU GOT IT RIGHT!!! CONFETTI TIME');
            break;
        } else {
            alert('OOPS');
        }
    }
}
