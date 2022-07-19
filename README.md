# HangMan-Game
I create the HangMan Game,to practice with functions. 
<!Doctype html>
<html>
<title>Hangman Game</title>
</head>
<body>
<h1> Let's play! </h1>
<script>
var words=["cloud", "winter", "javascript", "potato", "avocado", "ring"];
var word= words[Math.floor(Math.random()*words.length)];
var answerArray= [];
for(var i=0; i<word.length;i++){
anwerArray[i]= "_";
}
var remainingLetters=word.length;
var guesses=20;
while(remainingLetters > 0 && guesses > 0){
alert(answerArray.join(" "));
var guess= prompt("Guess a letter, or click cancel to stop playing.");
if(guess === null){
break;
} else if(guess.length !== 1){
alert("please enter a single letter.");
} else {
guesses--;
var guess = guess.ToLowerCase();
for (var j=0; j< word.length;j++){
if(word[j] === guess && answerArray[j] === "_")}
answerArray[j] = guess;
remainingLetters--;
    }
   }
  }
}
alert(answerArray.join(" "));
if(guesses > 0){
alert("Good job! The answer was " + word);
} else {
 alert("It´s a shame! But the way, the answer was " + word);
};  
</script>
</body>
