# Building a Gradebook whist reviewing Js fundamentals

## <ins>Objective :<ins>
### In this mini project, you will get to review JavaScript fundamentals like functions, variables, conditionals and more by building a gradebook app.

### This will give you an opportunity to solve small problems and get a better understanding of the basics.

## Javascript File
```js
function getAverage(scores) {
  let sum = 0;

  for (const score of scores) {
    sum += score;
  }

  return sum / scores.length;
}

function getGrade(score) {
  if (score === 100) {
    return "A++";
  } else if (score >= 90) {
    return "A";
  } else if (score >= 80) {
    return "B";
  } else if (score >= 70) {
    return "C";
  } else if (score >= 60) {
    return "D";
  } else {
    return "F";
  }
}

function hasPassingGrade(score) {
  return getGrade(score) !== "F";
}

function studentMsg(totalScores, studentScore) {
  let average = getAverage(totalScores);
  let grade = getGrade(studentScore);

  if (grade === "F"){
    return ("Class average: " + average+ ". Your grade: " + grade + ". You failed the course.")
  } else {
    return ("Class average: " + average+ ". Your grade: " + grade + ". You passed the course.")
  }
}
console.log(studentMsg([92, 88, 12, 77, 57, 100, 67, 38, 97, 89], 37));
```