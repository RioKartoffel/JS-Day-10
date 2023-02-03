# JS-Day-10
Dad Jokes

HTML:
The first line <!DOCTYPE html> declares the type of document.
The <html> tag defines the start of the HTML document and specifies the language as English with lang="en".
The <head> tag contains information about the document that is not displayed on the page, such as the title of the page, which is set to "Dad Jokes".
The <meta> tag sets the character encoding of the document to UTF-8 and the viewport width to the width of the device.
The <link> tag imports a stylesheet named "style.css" which contains the styles for the page.
The <body> tag contains the content that is displayed on the page. The <div> with class "container" contains a heading with text "Don't Laugh Challenge" and a div with id "joke" which will display the joke, and a button with id "jokeBtn" and text "Get Another Joke".
The <script> tag imports the JavaScript file "script.js" which contains the code to fetch and display the jokes on the page.
CSS:
The first line imports a font named "Roboto" from Google Fonts.
The rest of the styles define the look of the page, including setting the background color, font family, size, and spacing of the text, and styling the button.
JavaScript:
The code first selects the elements on the page by their id using document.getElementById(). It stores the joke div and the jokeBtn button in variables jokeEl and jokeBtn respectively.
The jokeBtn button has a click event listener attached to it that calls the generateJoke() function whenever the button is clicked.
The generateJoke() function makes a GET request to the https://icanhazdadjoke.com/ API to retrieve a joke. The response from the API is in the form of a JSON object, which is then parsed and displayed in the joke div. The function uses either the async/await or .then() syntax to handle the asynchronous API call. The async/await syntax is used in the first implementation of the function, while the .then() syntax is used in the second implementation of the function.
In summary, the code creates a simple web page that displays a random "Dad Joke" by making a request to an API and updating the page with the joke retrieved from the API.



