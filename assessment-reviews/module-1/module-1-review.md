# Module 1 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

## HTML

### Questions

1. What is HTML and what is it used for? Answer: HTML (Hyper Text Markup Language) is a computer language used in building websites.  In HTML, "tags" are used to organize text and images into different headers and categories. 
2. What is the difference between an ID and a class? A: In CSS, the computer language used to add style and form to the HTML structure, an ID is generally used to differentiate/manipulate ONE element of the HTML, whereas, a class is generally used to differentiate/manipulate a whole segment/category of HTML. 
3. What does it mean to write "semantic" HTML? A: Writing semantic HTML is use use HTML in ways that augment its meaning, as opposed to merely adding to its style and presentation.  This can be done by, fornexample, organizing a group of text under a certain header, or using the <em> emphasis tag on a word or phrase.</em>

### Exercises

1. Write a paragraph tag with a class of "highlight" and content "Watch out!". <p><mark>"Watch out!"</mark></p>
2. Write an HTML image tag to show an image called `profile-picture.jpg`. <img src = 'profile-picture.jpg'>
3. Write a link tag that links to http://google.com. <a href = "http://google.com">Link to google here.</a>
5. Write an complete standard HTML document outline (including a DOCTYPE, and `<html>`, `<head>`, and `<body>` tags).
<!DOCTYPE html>
<html>
  <head>
    <link type='text/css' rel='stylesheet' href='main.css'>
    <script type='text/javascript' src='main.js'></script>
  </head>
  <body>
  <h1> ... </h1>
  <h2> ... </h2>
  <h3> ... </h3>
    <ul>
      <li> ... </li>
      <li> ... </li>
      </ul>
  </body>
6. Inside of the code for the previous exercise, write the appropriate tag to link to a script file called `main.js`.
7. Inside of the code for the previous exercise, write the appropriate tag to link to a stylesheet file called `main.css`.
8. Write a numbered list in HTML and list three of your favorite books.
<ol>
  <li><i> Ragtime </i></li>
  <li><i> Goodnight Me, Goodnight You </i></li>
  <li><i> Where the Wild Things Are </i></li>
</ol>  
9. Fix the indentation of the following HTML sample:

  ```html
  <div>
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
  </ul>
  </div>
  ```

## CSS

### Questions

1. What is CSS and what is it used for?
2. What is the CSS box model?
3. What's the difference between margin and padding?

### Exercises

1. Write a CSS rule to make the text of all `h1` tags red.
2. Write a CSS rule to make the background color of the link with `class="btn"` blue:

  ```html
  <a href="#" class="btn">Learn more</a>
  ```

3. Write a CSS rule to give the first paragraph in the following HTML a font size of `20px`, but not the second paragraph.

  ```html
  <header class="jumbotron">
    <p>Hello, World!</p>
  </header>

  <p>Welcome to this awesome website!</p>
  ```

## JavaScript

### Questions

1. What is a function? What are they used for? A: A function is a particular type of code that executes whatever action is specified in the body of the code.  Functions are used for iterating a simple or complex task multiple times; functions eliminate errors and reduce the energy and time used by people and computers.
2. What is the difference between `==` and `===`? A: Both symbols mean "are the same thing as". '===' differs from '==' in JavaScript code in that '===' acts as an assimilator between strings and numbers, allowing more efficient interpretation of code. For example: the string "23"===23 the number.
3. What is the difference between global and local scope variables? A: With regard to functions, variables of global scope retain their value both outside and inside the function.  They are established in the first lines of code, before the function is written and indentations are made.  Local variables are contained within a particular function and their value pertains only to the particular function in which they are contained.
4. What is a boolean value? True and False are the common boolean values.  Along with other types of values, they are implicitly used in "if", "else/if", and "while" functions to direct the flow of the function.  
5. What is an array? An array is a group of values - usually strings and/or numbers. for example: var array = [1, red, 2, blue]

### Exercises

1. Write a line that declares a variable called `myName` and set its value to your name.
var myName = Tim
2. Write a loop that logs the numbers 1 through 10 to the console.
var number = 1
while(number<11){
  console.log(number);
  number++;
}  
3. Translate the following pseudocode into JavaScript: if `score` is greater than `3` and `lives` is greater than `0`, alert "You win!".
if(var score>3){
  if(var lives>0){
  alert("You win!");
  }
}
4. Write a function `sayHello` that takes one argument, a name, and logs "Hello, <name>!" to the console. Then, call the function below the function definition and pass in your name as the argument.
function sayHello(name){
  return console.log("Hello, " + name + "!");
}
sayHello(Tim);

5. What would the following script log to the console?

  ```javascript
  var currentSong = "Call Me Maybe";

  function setSong(song) {
    currentSong = song;
  }

  setSong("Friday, Friday");

   console.log(currentSong);
  ```
A: This would log "Friday, Friday" to the console.  
6. What would the following script log to the console?

  ```javascript
  var add = function(a, b) {
    return a + b;
  }

  var result = add(3, 7);

  console.log(result);
  ```
A: add(3, 7)
7. What would the following script log to the console?

  ```javascript
  var helloGoodbye = function(name) {
    return sayHello(name) + " " + sayGoodbye(name);
  }

  var sayHello = function(name) {
    return "Hello " + name " !";
  }

  var sayGoodbye = function(name) {
    return "Goodbye " + name " !";
  }

  console.log(helloGoodbye("Sarah"));
  ```

8. Write a function `findLongestWord()` that takes an array of words and returns the length of the longest one.
var word = [scooby, shaggy, fred, swampmonster]
var i = 0
findLongestWord(word){
  if (word.length[i] > word.length[i++]){
    word.pop[i++];}
    else if (word.length[i] < word.length[i++]){
      word.pop[i];}
    elso if (word.length[i] = word.length[i++]){
      word.pop[i];}
  else(if word[i++]=undefined){
    return word[i]}
}    
      
      

9. Define a function `sum()` that sums all the numbers in an array of numbers. For example, `sum([1,2,3,4])` should return 10.
var numbers = [1,2,3,4]
function sum(number

10. Write a function that takes a character (i.e. a string of length 1) and returns true if it is a vowel, false otherwise.
11. Write the correct line to make `"Woof!"` show up in the console based on this script:

  ```javascript
  var pet = {
    name: "Charles",
    goodDog: true,
    speak: function() {
      console.log("Woof!");
    }
  };
  ```

12. Using the same script as above, write the correct line to log the dog's name to the console.

## Command Line

### Questions

1. What is the command line and what is it used for?
2. What does the command `ls` do?
3. What does the command `pwd` do?
4. What does the following command do: `cd my-cool-project`

### Exercises

1. Write the command to make a new directory called "my-cool-project".
2. Write the command to create a file called "index.html".
3. Write the command to delete a file called "main.css".

## Git

### Questions

1. What is Git and what is it used for?
2. What's the difference between a local repository and a remote repository?

### Exercises

1. Write the command that you would use to create a new local Git repository.
2. Write the command to stage a file called `index.html` to be committed.
3. Write the command to view the current status of the git repository.
