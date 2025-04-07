# app-Next
app-Next

Explanation and Key Improvements:

React Structure: The code is now a React component, using useState for managing state and useEffect for handling side effects.
Functional Components: The quiz logic is organized within the PythonQuizApp functional component.
State Management:
current: Stores the index of the current question.
score: Stores the user's score.
timeLeft: Stores the remaining time for a question.
timer: Stores the timer ID.
quizStarted: Tracks whether the quiz has started.
selectedAnswer: Tracks the user's selected answer.
Effects:
The useEffect hook manages the timer. It starts when a question is displayed and is cleared when an answer is selected, the time runs out, or the component unmounts.
Another useEffect is used to control the flow of the quiz. It calls showQuestion when quizStarted changes or current changes, and calls showScore when all questions are answered.
UI Elements:
The question, options, timer, and score are displayed using React components.
The "Next" button is disabled until an answer is selected.
Event Handling:
startQuiz: Starts the quiz and resets the state.
checkAnswer: Handles the selection of an answer, updates the score, and stops the timer.
nextQuestion: Moves to the next question or ends the quiz.
showScore: Displays the final score and a restart button.
Styling: Uses inline styles and CSS classes. The styles from the original HTML are adapted for React. Tailwind CSS classes are used for more modern styling.
Animations: Uses framer-motion for animations.
Hooks: Uses useCallback to optimize functions that are passed as dependencies to other hooks.
Reusable Components: Uses Button from @/components/ui/button

