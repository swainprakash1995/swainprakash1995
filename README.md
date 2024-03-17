//"confirm box" showing user for palying Quiz Game

const userConfirmation = confirm("Do you want to play the quiz?");

//math questions
const mathQuestionOne = "What is 1+5=? \n A. 2 \n B. 3 \n C. 4 \n D. 6";
const mathOneAnswer = "d";
const mathQuestionTwo = "What is 4-2=? \n A. 2 \n B. 3 \n C. 4 \n D. 5";
const mathTwoAnswer = "a";
const mathQuestionThree = "What is 1+1=? \n A. 2 \n B. 3 \n C. 4 \n D. 5";
const mathThreeAnswer = "a";
//Science questions
const scienceQuestionOne =
  "Where does the formation of Urea takes place in our body ? \n A. Pancreas \n B. Kidney \n C. Liver \n D. Lungs";
const sciOneAnswer = "c";

const scienceQuestionTwo =
  "What is the freezing point of water as per the Fahrenheit scale? \n A. 0° \n B. 32° \n C. 100° \n D. 212°";
const sciTwoAnswer = "b";

const scienceQuestionThree =
  "Which of the following scientific discoveries was made by C.V Raman? \n A. Inelastic scattering of light by molecules \n B. Super Conductivity \n C. Controlled nuclear fission \n D. Cyclotron";
const sciThreeAnswer = "a";

// //English questions
// const englishQuestionOne = "What is 1+5=? \n A. 2 \n B. 3 \n C. 4 \n D. 6";
// const englishQuestionTwo = "What is 4-2=? \n A. 2 \n B. 3 \n C. 4 \n D. 5";
// const englishQuestionThree = "What is 1+1=? \n A. 2 \n B. 3 \n C. 4 \n D. 5";

//history questions
const historyQuestionOne = "Who was the first Prime Minister of independent India? \n A. Mahatma Gandhi \n B. Jawaharlal Nehru \n C. Subhas Chandra Bose \n D. Atal bihari baachpai";
const historyQuestionTwo = "The Indian Constitution was adopted on: \n A. 15th August 1947 \n B. 26th January 1950 \n C. 2nd October 1947 \n D. 20th October 1947";
const historyQuestionThree = "Who was the first Emperor of the Maurya Dynasty? \n A. Samudragupta \n B. Ashoka \n C. Chandragupta Maurya \n D. Jahangir khan";

// //gepgraphy questions
// const gepgraphyQuestionOne = "What is 1+5=? \n A. 2 \n B. 3 \n C. 4 \n D. 6";
// const gepgraphyQuestionTwo = "What is 4-2=? \n A. 2 \n B. 3 \n C. 4 \n D. 5";
// const gepgraphyQuestionThree = "What is 1+1=? \n A. 2 \n B. 3 \n C. 4 \n D. 5";

// //gk questions
// const gkQuestionOne = "What is 1+5=? \n A. 2 \n B. 3 \n C. 4 \n D. 6";
// const gkQuestionTwo = "What is 4-2=? \n A. 2 \n B. 3 \n C. 4 \n D. 5";
// const gkQuestionThree = "What is 1+1=? \n A. 2 \n B. 3 \n C. 4 \n D. 5";

//ask user to select a subject

if (userConfirmation) {
  //adding while loop here for itaration if user choose wrong option
  while (userConfirmation) {
    var userInput = prompt(
      "Please select a subject choosing A to C \n \n A. Mathmatics \n B. Science \n C. History  \n"
    );
    var grandTotal = 9;
    {
      switch (
        userInput.toLowerCase() // here adding toLowerCase() method for lowercase
      ) {
        case "a":
          alert("You are choosing Mathematics");
         var correctAns=0;
         var Total=3
          //question number 1 start (Mathematics)
          var userMathQuestionOne = prompt(mathQuestionOne);
          if (userMathQuestionOne.toLowerCase() == "d") {
            alert("Your answer is Correct");
            correctAns +=1;
          } else {
            alert("Wrong Answer");
          }

          //question number 2 start (Mathematics)
          var userMathQuestionTwo = prompt(mathQuestionTwo);
          if (userMathQuestionTwo.toLowerCase() == "a") {
            alert("Your answer is Correct");
            correctAns +=1;
          } else {
            alert("Wrong Answer");
          }

          //question number 3 start (Mathematics)
          var userMathQuestionThree = prompt(mathQuestionThree);
          if (userMathQuestionThree.toLowerCase() == "a") {
            alert("Your answer is Correct");
            correctAns +=1;
          } else {
            alert("Wrong Answer");
          }

          if(correctAns == Total){
            alert("You know everything, plz choose another subject")
        }else{
            alert("You need more practice!!!")
        }

          // userConfirmation = true;
          break;
        case "b":
          alert("You are choosing Science");

          var correctAns2=0;
         var Total2=3

          //question number 1 start (Science)
          var userScienceQuestionOne = prompt(scienceQuestionOne);
          if (userScienceQuestionOne.toLowerCase() == sciOneAnswer) {
            alert("Your answer is Correct");
            correctAns2 +=1;
          } else {
            alert("Wrong Answer");
          }

          //question number 2 start (Science)
          var userScienceQuestionTwo = prompt(scienceQuestionTwo);
          if (userScienceQuestionTwo.toLowerCase() == sciTwoAnswer) {
            alert("Your answer is Correct");
            correctAns2 +=1;
          } else {
            alert("Wrong Answer");
          }

          //question number 3 start (Science)
          var userScienceQuestionThree = prompt(scienceQuestionThree);
          if (userScienceQuestionThree.toLowerCase() == sciThreeAnswer) {
            alert("Your answer is Correct");
            correctAns2 +=1;
          } else {
            alert("Wrong Answer");
          }
          
          if(correctAns2 == Total2){
            alert("You know everything, plz choose another subject")
        }else{
            alert("You need more practice!!!")
        }

          break;
        
        case "c":
          alert("You are choosing History");

          
          var correctAns3=0;
         var Total3=3

          //question number 1 start (history)
          prompt(historyQuestionOne);
          if (historyQuestionOne.toLowerCase() == "b") {
            alert("Your answer is Correct");
            correctAns3 +=1;
          } else {
            alert("Wrong Answer");
          }

          //question number 2 start (history)
          prompt(historyQuestionTwo);
          if (historyQuestionTwo.toLowerCase() == "b") {
            alert("Your answer is Correct");
            correctAns3 +=1;
          } else {
            alert("Wrong Answer");
          }

          //question number 3 start (history)
          prompt(historyQuestionThree);
          if (historyQuestionThree.toLowerCase() == "c") {
            alert("Your answer is Correct");
            correctAns3 +=1;
          } else {
            alert("Wrong Answer");
          }

          if(correctAns3 == Total3){
            alert("You know everything, plz choose another subject")
        }else{
            alert("You need more practice!!!")
        }
         
          break;

      
        default:
          alert("Please choose a correct option");
      }
    }
    if (grandTotal==Total+Total2+Total3){
      alert("you answered all subject correct")
    }else{
      alert("You need more practice!!!")
    }
  }
} else  {
  alert("No Problem See you on Next Time");
  }
