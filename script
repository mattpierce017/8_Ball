$(document).ready(function() {

  const magic8Ball = {};
  magic8Ball.listOfAnswers = ["If I Could Say Yes Twice... I Would", "Best Choice of Your Life!", "I Don't Think I Have Ever Been More Confident In a Yes...", "Of course!", "Indubitably", "How Could You Not?"];

  $("#answer").hide();

  magic8Ball.askQuestion = function(question) {
    $("#8ball").effect("shake");

    $("#8ball").attr("src", "https://s3.amazonaws.com/media.skillcrush.com/skillcrush/wp-content/uploads/2016/09/magic8ballAnswer.png");

    $("#answer").fadeIn(4000);

    const randomNumber = Math.random();

    let randomNumberForListOfAnswers = randomNumber * this.listOfAnswers.length;

    let randomIndex = Math.floor(randomNumberForListOfAnswers);

    let answer = this.listOfAnswers[randomIndex];

    $("#answer").text(answer);

    console.log(question);
    console.log(answer);
  };

  const onClick = function() {

    $("#answer").hide();

    $("#8ball").attr("src", "https://s3.amazonaws.com/media.skillcrush.com/skillcrush/wp-content/uploads/2016/09/magic8ballQuestion.png");


    setTimeout(function(){
      let question = prompt("PLEASE ASK A YES/NO QUESTION!");
      magic8Ball.askQuestion(question);
    }, 500);


  };

  $("#questionButton").click(onClick);

});