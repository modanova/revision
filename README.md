# Revision

## Git

- [x] Why do we use Git? - To organise versions of and simultaniously work on projects together
- [x] What’s the difference between Git and GitHub? - git is the app for the local computer and github is a web based platform
- [x] What happens when you clone a repository? - You download it to your local machine and can edit and update it online
- [x] What happens when we do git pull origin main - you download the most recent main branch of a repository with all the branches that stem from it as they appear on github
- [x] How do we create a new branch on our local machine? git checkout -b <name>
- [x] How do we control which changes will be included in the next commit? - by staging only the files we want to include in the next commit
- [x] When might git add . be inappropriate? - When one might just like to update one or a couple of files but not all of the files of the repository
- [x] How do we make sure our local changes don’t conflict with main? - We git pull first and create new branch from the main. Conflicts despite this can be reviewed and edited manually from GitHub
- [x] What does git push origin [branch-name] do? - When pushing a new branch to Github it usually asks you for a confirmation that this is the correct repository you'd like to add it to
- [x] Why do we make pull requests instead of just changing main directly? - The larger the project, the more dependencies there are, the more people work on them. For a team, pull requests helps organising the project, ensures new changes don't overwrite other people's work and updates them on the incomming changes. For a standalone project, it keeps your current project safe from mistakes that might break everything. Also it keeps a history of the project.
- [x] Why should you review your teammates’ pull requests? - To ensure the incomming changes have not interfered with the state of the current project, to keep track of their work, to close issues and open new ones

## HTML

- [x] Why is accessibility important? - To ensure your web app is accessible to people with various needs and ensure as many people can access it as realistically possibe
- [x] How can you quickly find simple accessibility problems? - Lighthouse, manually going through the accessibility checklist
- [x] What is semantic HTML? - Creating HTML using descriptive tags that somewhat give a sense of the expected purpose of the given web container
- [x] Why is it important to use the “correct” semantic element? - Some semantic elements come with their own functionality which is useful and saves the developer some time if they were to create another element manually. To give other developers a better code readability
- [x] What is the <form> element used for? - to collect user's input

## CSS

- [x] How would you use CSS variables to make a reusable colour palette? - store the chosen coloures into variables and refer to them when selecting colours using var(e.g. --prime-color);
- [x] How would you use flexbox to make elements sit on a single line? - by making the parent container's display set to flex
- [x] How would you use grid to make a layout that automatically adds columns as the screen gets wider? - by using grid-template-columns and set it to the amount and size of columns expected to see
- [x] Why is it important to create a responsive design? - To ensure our content can be accessed and readible on all devices possible
- [x] How would you structure your CSS to make it “mobile-first”? - Start adding styles for a small screen and add media queries for larger screens later on

## Javascript

- [x] Why should we avoid using var to define variables? - because of its scope. Var creates a variable that is accessible globally throughout the JS file. This can interfere with functions that only aim to use a varible inside their scope and forget about it after the function has executed
- [x] How might you make a long, complex chunk of code easier to read? - By breaking it down and going through the code line by line, e.g. giving a variable a value and seeing how it will get amended through a functon
- [x] What is a “callback”? - an existing function that is passed as an argument and used by another function

### Array methods

- [x] How would you use array.map() to create a new array with transformed values?- take an array and apply a callback function inside the map to every argument of that array using this methos, e.g. .map( x => x+1) to return all numbers in an array increased by 1

- [x] How would you use array.filter() to create a new array with certain values removed? - apply .filter() with a callback function as a test to pass which only returns the elements of the array that pass that test
      filter()How would you use array.find() to get a single value from an array? - By giving passing a callback function as an argument to find to search for an alement that passes the test in the callback

### Promises & fetch

- [x] What is a promise? - a JS object that takes an asynchronous code and "promises" an answer or a failure
- [x] How do promises help manage asynchronous code? - it allows asychronous code to run in a given order
- [x] What does a promise’s .then method return? - returns a value that was received from a promise
- [x] How could you chain promises together to avoid “callback hell”? - chain their responces using .then or use asynchronous functions
- [x] How would you handle a fetch request that failed to get a response from the server? - using .catch at the end of .then chains
- [x] How would you handle a fetch request that received a 404 response from the server? - Ensure you've used a valid link for example

## HTTP

- [x] What is an HTTP request? - a request fromt the local browser to a server to exchange information
- [x] What kind of request is sent when you click a link in your browser? - a get request - information is requested from the server
- [x] What kind of request is sent when you submit a form in your browser? - a post request, sending user input to the server
- [x] What is an HTTP response? - the encoded information that the server sends back as a response
- [x] What does the status code of an HTTP response tell us? - What error has occured or whether the information exchange was completed successfully
- [x] What are some common status codes? - 404, 200
- [x] What are HTTP methods for? - to specify the type of exchange to take place
- [x] What kind of request should have a GET method? - that handles the data received
- [x] What kind of request should have a POST method? - sending an object of user's information to the server
- [x] What kind of request should have a PUT method? - Not sure
- [x] What kind of request should have a DELETE method? - specify what to delete
- [x] What is the “body” of an HTTP request for? - this is where the information sent contained

## DOM

- [x] How would you get a reference to a DOM element in your JS? - by storing the element into an object variable, using document. and selecting the relevant tag, class, id, etc. then addind an event listener to it
- [x] How would you get references to multiple DOM elements at once in your JS? - querySelectorAll to select all elements of the given tag or class in an array
- [x] How would you update properties of a DOM element? - by selecting it with JS and storing it into an object, then refering to it's properties as any object's keys e.g. element.value = 0;
- [x] What’s the difference between a “property” and an “attribute”? - Didn't know this, found the answer: "An attribute is the initial state when rendered in the DOM. A property is the current state". To research!
- [x] What are some different ways to add content inside a DOM element? - createElement(), append(), cloneNode()
- [x] When might the <template> element be useful? - to copy a ready made, often complicated, and styled element quickly into another element
- [x] What are the different ways to add event handlers to elements? - as properties in the HTML directly or by storing elements into variables and adding event listeners to them
- [x] Why is addEventListener the safest way to add an event handler? - HTML code might get deleted
- [x] - [x] How can you access submitted form values in your JS? - attaching a JS onto the form and usign a callbackfunction that receives the form's input as argument, preventDefault and element.target etc.

## Testing

- [x] Why are tests useful? - To discover if dependencies work and the desired responses are received, information is communicated between function as expected. Also to test all edge cases
- [x] What is the difference between unit and integration tests? - unit tests only work on one function where as integration tests check if a group of functions correspond together as desired
- [x] What kind of code is easier to test? - one function not depending on other function's returned values
- [x] Why should your tests be isolated from each other? - so we achieve a clean and complete test that checks if the functions work seamlessly from all perspectives
- [x] What is Test Driven Development (TDD)? - Writing code simultaniously with writing a test for the given code, it facilitates writing working functions by breaking the functions down into a step by step process
- [x] When might TDD be a useful process to follow? -

## Debugging

What process would you take to find out why your code isn’t working?
What tools do JS/dev tools have to help debug your code?
At what point should you ask for someone else’s help?
