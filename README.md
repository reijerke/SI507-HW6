# JavaScript assignment

## Some useful resources
* Some [JavaScript tutorials](https://www.htmldog.com/guides/javascript/)
* The complicated [resources in the You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) series, including [your reading last week](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md)
* [A resource for CSS/style/colors](https://htmlcolorcodes.com/)  
* [An excerpt from a specific workshop site](https://witny-summer-guild-2018.github.io/day_4_exercise_2.html) (for a different audience than yourselves) which addresses some common questions about jQuery
* [The simple JSFiddle example from class](https://jsfiddle.net/2of65j8q/)
* A [W3Schools resource on JavaScript output](https://www.w3schools.com/js/js_output.asp)
* Google, Piazza, your classmates, office hours, lab time!

## Included files
* This `README.md`, which you should edit with answers to the questions
* `jsPracticeLab.html`, which you'll need to edit and try out
* `jquerylib_submit_example.html`, which you'll need to edit and try out

## Your goals for this lab

### Broadly
The aim for this lab is to practice adapting to and understanding code in a new-to-you (or not) language and its own libraries/packages -- JavaScript, in this case.

The programming skills you have built up till now are useful for *Python programming*, but, more than that, they extend to fundamentals of many kinds of programming.

This experience is *not in any way* about becoming an expert JavaScript programmer. Instead, it is about using what you *do* have experience with -- and your skills in *learning new things* that relate to programming -- in order to make educated judgments about some brand new-to-you code, even if you haven't learned in detail about it yet. That's part of what being in technology -- or even technology-adjacent -- will often mean.

### Specifically

Below are a bunch of questions and indications of things to do. For each indication of something to do with code, there is also an accompanying question to answer or brief explanation to give.

**To complete and submit this assignment, you should:**

* Fork (and clone) this repository
* Add our instructional team as a collaborator to your fork (see instructions for adding collaborators on Canvas)
* Edit this `README.md` file with answers to the questions/prompts, briefly, using Markdown formatting so that the questions appear in bulletpoints and the answers appear clearly below each respective question, *not* as bulletpoints.
* Add all names of those who worked on this (as indicated below)
* Make the changes that are indicated below to each of the `.html` files with JavaScript programs provided. (You'll probably do this concurrently with answering questions)
* Commit (as you go) and push your changes to all three files to your GitHub forked repository.
* Submit a link to your repository on Canvas. (This HW doesn't have an autograder -- it will be graded by hand/by humans this time.)

### Important notes
* You are *more than* welcome to work together on this, but **you must <u>each</u> submit a repo to be graded on it**, so if you do work together, you should do the following:
	* Make sure each one of you understands all the work -- YOU are responsible for using and knowing this information
	* Write each person's name & uniqname who worked on the assignment together on your submitted `README.md` file (you'll see a space for this below)

* In answering questions, please make sure the formatting is clear to read and that you have updated the names of everyone who worked with you, with your name first (see below).

* In answering questions, assume all of the questions include a *explain briefly* note -- you do NOT have to, and should not, write extended paragraphs. Be as concise as you can and explain in your own words. Don't worry about "whether it's enough" -- just worry about conveying your understanding so you can read it later, or even give it to someone else, and the answers will help/make sense.

* It is not acceptable to copy and paste answers from the internet and submit them as your own. If you cite things, make sure you provide a citation, including to links. If you get information from a resource and rephrase it so you're basically explaining an idea, that's just fine for an explanatory purpose in this assignment, but you *must* cite any quotes or examples that aren't yours.

* **For grading:** we are grading on...
	* Following the instructions
	* Approximate correctness of the code edits
	* Careful & clear answers to the questions
	* Correct answers to the questions
	* Slightly more than half the 1000 points will come from answering the questions. The rest will come from your edits to the code.

### Names of people you have worked with on this assignment
* List everyone's names and uniqnames who have worked on this assignment with you, **including your own name, but make sure YOUR name is first and bold**
* **Dana Reijerkerk (reijerke)**
* Zinnia Khan (zinniak)
* Madel Leal (madeleal)

## Questions & code instructions

### The first questions address the `jsPracticeLab.html` file.

* **This is just an example question.**

This is what an example answer should look like. If you want to include some code, which you probably don't have to do, you can, like this:

```js
Some JavaScript code
```

* **What does a code comment look like in JavaScript? What character/s do you have to put before a comment?**

Comments begin with two // symbols. It looks like this:

```
//
```

* **Explain what needs to happen to get a JavaScript program to "run", given the JavaScript you've seen in this assignment.**

The <script> tag tells the browser you are running JavaScript code (Citing from https://www.htmldog.com/guides/javascript/beginner/makingstuffhappen/). To run the entire program you open it in your browser (I just click on the file and it does so automatically).

* **What functions in JavaScript seem to be similar in function to the `print` function in Python? (There are two.) Why might you use one and not the other? Explain briefly.**

The console.log() and alert() functions display data (this is seen in lines 12-13 of `jsPracticeLab.html`). The alert() function displays a pop-up box with the text inside the function as the message (https://www.w3schools.com/jsref/met_win_alert.asp). Console.log() outputs a message to the console, which may be more useful to debugging the console than a pop-up.   

* **What code would have to comment out to get rid of the pop-up box when you load the page? (Related to the last question.) Do that in the code file, and then, add code so that a text box will appear that contains the current date and time! *HINT:* Look through the rest of the code first...**

Line 12 `alert("hello")` if commented out gets rid of the pop-up. I changed the code to say `alert(new Date());` to get the current date and time to appear.

* **How can you put your own name at the top where it currently says "A name"? Explain very briefly how to do so, and replace `A name` in the web page with your own name.**

I changed line 17 that said `document.querySelector('h1').innerHTML = "A name";`. Instead of `"A name"` I wrote `"Dana"`.

* **What does the word `document` represent in this code? Explain briefly.**

Document represents the webpage and allows me to access the elements on the page (Citing from https://www.w3schools.com/js/js_htmldom_document.asp).

* **What is happening in line 12 (
		`document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length`
)? Explain, briefly (<= 2 sentences).**

Look at the elements that have the tag name `<li>` and count how many there are. Assign that number to the span tag that has `id = "items"` in it.

* **What color would the background of this page be <u>if there were no JavaScript in this page</u>?**

White, which is the default color.

* **Why are there a couple of gray boxes on the screen with a different colored border? How could you edit this code to make them a different color? Explain briefly. Then edit the code to make those boxes some shade of blue, of your choosing.**

The gray boxes from code written in the `<style>` tag, which is CSS. I edited background-color in the paragraph (`<p>` tag) using a code for light blue from https://www.w3schools.com/colors/colors_picker.asp.

* **Edit the code so that, if you highlight `McGill University` and copy it, you see the text `O Canada` near the bottom of the page. Briefly explain why you made the edits that you did -- how did you know/figure out what to do?**

I noticed when you copied `Univeristy of Michigan` on the webpage the words `Go Blue!` appear. So I changed the phrase `Go Blue!` in `function copyFunction()` to say `O Canada` and also moved the line `oncopy="copyFunction()"`inside the `<li>` tag for `McGill University`.

* **In the original code, when you click the button that says `Wow`, you see a text box! Wow. Explain briefly in your own words why the following code causes that to happen:**

```js
function handleClick(){
	alert("hello");
}
```
**and**

```js
<button onclick=handleClick() id="wow-button">Wow</button>
```

`button onclick=handleClick() id="wow-button">Wow</button>` says that when the button with the id `wow-button` is clicked it invokes the function `handleClick`. `function handleClick(){alert("hello")}` is indicating that when the function called `handleClick()` is invoked the web page displays `hello` in a pop-up window.


* **Knowing what you learned from the previous question, add code/markup to the `jsPracticeLab.html` file *so that* there is a button with the text `Spring Equinox 2019` on it somewhere on the page, and when that button is clicked, a text box containing the text `March 20, 2019` appears. (There's no function -- that I am aware of -- to automatically get this info, you've got to type it yourself.)**

### The next few questions address the `jquerylib_submit_example.html` file.

* **Check out the file `jquerylib_submit_example.html`. This is an example of code that uses a package called `jQuery` (and this will need you to have an internet connection to run it properly, although the other file does not). Check out resources above for more on jQuery!**

* **When you enter input that isn't valid, you see an error that is red. Why is the error in red? Why is the response for valid inputs blue?**

This is because of the `if...else` statement in lines 20-26 which reference the `<style>` tags in lines 7-13. The element with `class="error"` is styled under the `<style>` tag as `red` and element with `class="good"` is styled as `blue`.

* **What is this line `var regex = /^[a-zA-Z]+$/;` helping with? And if you googled something to figure that out, what did you google, and what, briefly, did you learn? (If you didn't need to google, you can leave that out, but explain briefly what that line is helping the program do, anyway.)**

The line `var regex = /^[a-zA-Z]+$/;` helps improve performance because the literal pattern is only compiled once in the JavaScript code (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions).

I googled `/^[a-zA-Z]+$/` and learned that it is a regular expression in JavaScript that is defined by character encoding like in cataloging (e.g. the `/` marks the beginning and end of the expression, if `^` is before or after the `[]` it means something different, etc.). I also learned that the `a-zA-z` is saying make sure the text is the letters A-Z. The capital and lowercase letters ensure the expression catches the variant spelling; in programming a different case is considered a different variable altogether.

* **What's different about the syntax of conditional statements in JavaScript, compared to Python?**

In python there is `elif` but in JavaScript you use `else if` to indicate if the first thing I said wasn't true then do this thing. The formatting is also a little different. The if/else in python is indented on the same line of code and there is a colon after the conditional statement. In python you would construct an if/else statement like this:

```
	if (condition):
		//block of code if true
	else:
		//block of code if false
```

In JavaScript the code uses `{}` to indicate what comes after is the code if true/false and the `else {}` line is not flush with the `if {}` line. In JavaScript the code would look like this:

```
	if (condition) {
		//block of code if true
	} else {
		//block of code if false
	}
```

* **What do you think the `10000` refers to in the code `.fadeOut(10000)`?**

This refers to how quickly the text in the console disappears once the function is executed. The higher the number the quicker it disappears (https://www.w3schools.com/jquery/eff_fadeout.asp).  

* **What do you think is going on with the following code at the beginning of the program? Note that the most important thing to do for answering this question is to be thoughtful and clear, not to be absolutely correct:**


```
js
$(document).ready(function(){
    $("form").submit(function(event){
```

The `$(document).ready()` is a jQuery `event method` that lets you execute the function only after the document (the entire webpage you created) is loaded. In the next line `$("form").submit()` means when I submit a form do this. The function inside `submit()` I think then means then do this thing to my submitted form. I'm not sure what `event` is for. Maybe it's what action should happen? Like this thing I call event should happen when I submit a form.

* **Add some code to the `jquerylib_submit_example.html` file so that, if the input is valid and is specifically the text `hello`, rather than the visible output being `Nice!` in blue, the visible output should be `Hello to you too!`, also in blue, just like `Nice!` is.**
	* *HINT:* You'll have to make some changes to the conditional statement, and possibly look up some JavaScript conditional syntax. You'll also need to look carefully at what generates visible output right now.
