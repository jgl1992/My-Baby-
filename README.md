RE:
A public GitHub repository containing your project: https://github.com/users/jgl1992/projects/1/views/3
An HTML document for the page: 
<!DOCTYPE html>
<html lang ="en">
<head>
<meta charset = UTF>
<title> weather API </title>
<style>
body {
font-family: arial
margin: 2em;
    }
.endpoint{
padding: 1 em;'
}
</style>
</head>
<body>
<h1> weather API </h1>
<p> Tina Lin's API will give you data on the temperature (too hot to handle) for HIS "condition"; thank God we are NOT like him </p>
<div class "endpoint">
<h2> /api/weather/temperature </h2>
<p> desc </strong> return temp </p>
    <ul> 
<li> location: string, LISLE </li>
    </ul>
"temperature": {
"value": 70"
  }
}</pre>
  </div>
</body>
</html>
A CSS document to style the HTML page:

/justina.css/
body{
font-family: tahoma, geneva;
background linear-gradient
color: #444;
text-align: center;
}

/* hot-weather.css */

body {
font-family: tahoma, geneva;
background: linear-gradient
color: #333;
text-align:center;
}
  
h1 {
font-size: 2em;
Color: #ff3c00;
}

.weather-icon {
font-size: 5em;
color: #ffca3a;
}

footer {
margin-top: 3em;
color:#444;
}
A JavaScript file that retrieves data from one of several public API sources to display the data on your HTML page/ 
For the Star Wars API, have a page that shows character information and a page that shows film information.

Here is my starwars.js file!
//fetch and display star wars characters and film info from SWAPI
const characterContainer = document.getElementByID("character");
const filmContainer = document.getElementById("film");
// fetch character data (Bix Caleen id 2)
fetch("https://swapi.dev/api/people/2")
.then(response => response.json())
.then(Data =: {
characterContainer.innerHTML =
<H2> Bix's character info: fearless and bold </h2>
<p><strong> name:</strong> ${data.name}</p>
<p><strong>eye color: </strong> ${data.eye_color}</p>
      `;
    })
.catch(error => {
characterContainer.innerHTML = <p> error fetching </p>'
}];

    .catch(error => {
      characterContainer.innerHTML = `<p>Error fetching character data.</p>`;
      console.error(error);
    });

 
A README file that includes the instructions for running the webpage
#🌦️ Tina Lin's Hot Weather API

Welcome to my pleasant, robust, and productive API for accessing real-time weather data before your hiking adventure! You will know if it's sunny or rainy.
In the file I am including **temperature** and **conditions** such as sunny or rainy. 



CONTENT:
Display the data for at least 2 of the end-points in the API
Examples: If you choose the use the Weather API, use temperature and condition (rainy/sunny/etc) end-points. For the Star Wars API, use characters and film title end-points.
Include navigation from each end-point’s page to the other end-points that are displayed
Example: If you choose to use the Weather API, be able to click between a page that shows temperatures and a page that shows conditions. For the Star Wars API, have a page that shows character information and a page that shows film information.
Issue new GET requests for the linked data to display in the linked pages.
FUNCTIONALITY:
Be sure that we can get the code to run without issues by following the instructions in the README file
Be sure navigation between the different end-points behaves properly and is not slowed down by requesting more data than needs to be displayed
Be sure your code is readable and well structured
If including a user-interactive feature like a search field, be sure that you appropriately handle error cases
Be thoughtful about what typ
