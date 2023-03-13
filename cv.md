# ***Pavel Hvan***

### Junior Frontend Developer

______
 
## Contact information:

***Phone***: +996 555 960 890

***Email***: pavel.hvan@keiin.kg

***[LinkedIn](https://www.linkedin.com/in/pkhvan/)***

***Discord:*** Nazzemax #8716
  ____
  
### About myself:
Good afternoon, I am Hvan Pavel, and I would like to share some information about myself.My goal is to get a job in IT field where I can apply my knowledge and skills to the fullest extent and develop professionally.My priorities are to continually learn and improve my skills to be the best in my field. I strive to learn new things and develop in my profession to achieve my goals.My strengths are ability to learn quickly, creativity, responsibility, teamwork skills, organizational skills. I do not have commercial experience yet, but I am confident that I can learn quickly and put my knowledge and skills into practice. I have experience in participation in projects, courses, internships.I work mostly on my own projects. 
I am constantly learning new technologies and ways of working to keep abreast of the latest trends in my field. I am willing to apply my knowledge and experience to achieve my goals and become a professional in my industry. Thank you for your attention to my resume, and I look forward to the opportunity to showcase my skills in future jobs.

## Skills:

- HTML5, CSS3, SASS

- Javascript, React, Node JS

- Git, Github

- Figma

## Code example:
**parseInt() reloaded KATA from CODEWARS:**  Convert string representing numbers in words to integers. Valid numbers range from "zero" to 1 million. Optional "and" in some cases. All input numbers are valid. Examples: "one" => 1, "twenty" => 20, "two hundred forty-six" => 246, "seven hundred eighty-three thousand nine hundred and nineteen" => 783919.

```
function parseInt(s) {
  // Map English words for numbers to their corresponding values
  const numberWords = {
    zero: 0,
    one: 1,
    two: 2,
    three: 3,
    four: 4,
    five: 5,
    six: 6,
    seven: 7,
    eight: 8,
    nine: 9,
    ten: 10,
    eleven: 11,
    twelve: 12,
    thirteen: 13,
    fourteen: 14,
    fifteen: 15,
    sixteen: 16,
    seventeen: 17,
    eighteen: 18,
    nineteen: 19,
    twenty: 20,
    thirty: 30,
    forty: 40,
    fifty: 50,
    sixty: 60,
    seventy: 70,
    eighty: 80,
    ninety: 90,
    hundred: 100,
    thousand: 1000,
    million: 1000000
  };

  // Split input string into an array of words
  const words = s.match(/\w+/g);

  // Check if the number is negative
  const isNegative = words[0] === 'minus';

  // Accumulate values for each "block" of numbers
  let subtotal = 0;
  let total = 0;

  // Loop over words in the input string
  words.reduce((previous, word) => {
    // Skip the word "and"
    if (word === 'and') {
      return previous;
    }

    // Check if the word is a valid number word
    if (!numberWords.hasOwnProperty(word)) {
      throw new Error(`Invalid word: ${word}`);
    }

    const value = numberWords[word];

    // Handle "hundred", "thousand", and "million"
    if (value >= 1000) {
      total += subtotal * value;
      subtotal = 0;
    }
    // Handle numbers between 100 and 999
    else if (value >= 100) {
      subtotal *= value;
    }
    // Handle numbers less than 100
    else {
      subtotal += value;
    }

    return word;
  }, '');

  // Add the final subtotal to the total
  total += subtotal;

  // Handle negative numbers
  if (isNegative) {
    total *= -1;
  }

  return total;
}
```

## Experience:

- **Keiin International University 2018-2022**

Project [Mogo](https://github.com/Nazzemax/Mogo) used technologies HTML, CSS, Jquery

Project [Blitz](https://github.com/Nazzemax/blitzWebsite) used technologies HTML, CSS, Jquery

Project [Simple clock](https://github.com/Nazzemax/simpleClock) used technologies HTML, CSS, Javascript

## Languages:

- ***English:*** - Upper-Intermediate according to the online test at EF SET [www.efset.org](https://www.efset.org/cert/pEfc8q)

- ***Russian:*** - Native

- **Korean:** - Elementary
