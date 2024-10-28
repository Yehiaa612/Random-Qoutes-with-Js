# Random Quotes Generator

A lightweight web-based application that displays random motivational or inspirational quotes on each click. Built with HTML, CSS, and JavaScript.

## Features
- **Random Quotes:** Displays a new quote with each interaction.
- **Dynamic Rendering:** Uses JavaScript to select and display quotes.
- **Array of Quotes:** Includes a predefined list of quotes with authors.

## Technologies Used
- **HTML5**  
- **CSS3**  
- **JavaScript**

## Usage
1. Clone the repository.
2. Open the `index.html` file in a web browser.
3. Click the button (if implemented) or refresh the page to see a new quote.

## Code Overview
- **`script.js`**: Contains the logic to fetch a random quote from an array and display it on the page.

### Example Code Snippet
```javascript
var qoute = [
    { qoute: "Do not take life too seriously. You will not get out alive.", Auther: "--Elbert Hubbard" },
    { qoute: "'The best revenge is massive success.'", Auther: "--Frank Sinatra" },
    { qoute: "'You miss 100% of the shots you don't take.'", Auther: "--Wayne Gretzky" }
];

function getQoutes() {
    var num = Math.floor(Math.random() * qoute.length);
    document.getElementById("quote").innerHTML = qoute[num].qoute;
    document.getElementById("auther").innerHTML = qoute[num].Auther;
}
