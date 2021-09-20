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

## Sample Guessing Game For/While imbedded loops

>function randomnumber(){<br>
    //100 is inclusive, 0 not inlcuded<br>
    let randomnum = Math.floor(Math.random()*100) + 1;<br>
    return "Your lucky number today is " + randomnum<br>
}

> function guessinggame(){<br>
    correctanswer = randomnumber();<br>
    console.log(randomnumber);<br>
    //console.log is for testing and double checking<br>
    let guesses = 3;<br>
    for(let i=0; i<guesses; i++){<br>
        //i++ add one each time<br>
        let guessesLeft = guesses - i;<br>
        let userGuess = parseInt(prompt('Please enter an integer between 1 and 100. You have '+ guessesLeft + ' tries left!'));<br>
        while(userGuess<1 || userGuess>100){<br>
            userGuess = parseInt(prompt('Try Again! Did you enter an integer between 1 and 100?'));<br>
        }<br>
        if(userGuess == correctanswer){<br>
            alert('WAHOO! YOU GOT IT RIGHT!!! CONFETTI TIME');<br>
            break;<br>
        } else {<br>
            alert('OOPS');<br>
        }<br>
    }<br>
}<br>
