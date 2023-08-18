---
title: "Weather App using only HTML CSS and JavaScript"
datePublished: Fri Aug 18 2023 18:25:33 GMT+0000 (Coordinated Universal Time)
cuid: cllgx7yzp000k09l42ueefny1
slug: weather-app-using-only-html-css-and-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1692384114417/08c2916f-0acb-4ead-b6eb-608f13489896.jpeg
tags: javascript, apis, web-development-project-ideas, weatherapp, javascript-projects

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1692383075797/cee4f0d9-02b8-449f-8d9e-f596c69a4c3c.png align="center")

Here's how you can create a weather app just by using HTML CSS and Javascript:  
In the modern digital age, convenience and information are at our fingertips. Weather is no exception – imagine being able to access real-time weather forecasts right from your web browser! In this blog post, we're about to demystify the inner workings of a weather web app. By merging HTML, CSS, and JavaScript, we'll create a stylish and functional weather app that displays weather details for a specific city. Let's embark on this coding journey together.

Setting the Scene

Our web app adventure begins with structuring the HTML. This foundational markup provides the canvas upon which our weather app comes to life.

```python
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Weather App</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="card">
        <div class="search">
            <input type="text" id="cityName" spellcheck="true"> 
            <button> <img src="/Website/Assets/images/search.png" alt=""></button>
        </div>
        <div class="weather">
            <img src="/Website/Assets/images/rain.png" class="weather-icon">
            <h1 class="temp">22°C</h1>
            <h2 class="city">Radha Valley</h2>
            <div class="details">
                <div class="col">
                    <img src="/Website/Assets/images/humidity.png" alt="">
                    <div>
                        <p class="humidity">50%</p>
                        <p>humidity</p>
                    </div>
                </div>
                <div class="col">
                    <img src="/Website/Assets/images/wind.png" alt="">
                    <div>
                        <p class="wind">15km/ph</p>
                        <p>wind-Speed</p>
                    </div>
                </div>
            </div>
        </div> 
    </div>

    <script src="weather.js"></script>
</body>
</html>
```

Breaking Down the HTML

1. The standard HTML structure sets the tone for the page.
    
2. The `<link>` tag links an external stylesheet (style.css) for styling our app.
    
3. Within the `<body>`, we've laid out a structure comprising a search bar, weather display, and placeholder images/icons.
    
4. An `<input>` field is provided for users to enter the desired city name.
    
5. A `<button>` element adorned with a search icon offers a visual cue to initiate the search.
    
6. The weather display area includes a weather icon, temperature, city name, and additional weather details.
    
7. Icons for humidity and wind are included, along with labels and placeholders for actual data.
    

Styling with CSS

To give our weather app a polished and visually appealing look, we use CSS to style the elements according to our design preferences.

Title: Mastering CSS: A Deep Dive into Styling a Weather App

Introduction

In the realm of web development, styling is the brush that paints the canvas of user interfaces. Cascading Style Sheets (CSS) hold the power to transform a mere collection of elements into a visually appealing and functional web application. In this blog post, we'll embark on an exciting journey through the lines of CSS code that bring life to a weather app. From defining the layout to crafting colors and alignments, you'll witness the magic that CSS can bestow upon a user interface.

CSS as the Artist's Palette

Our weather app's visual appeal begins with a global reset, ensuring a consistent starting point across browsers and devices.

```css
*{
    margin: 0;
    padding: 0;
    font-family: sans-serif;
    box-sizing: border-box;
}
```

1. The universal selector `*` selects all HTML elements and applies uniform styling.
    
2. `margin: 0; padding: 0;` resets margins and padding to eliminate default spacing.
    
3. `font-family: sans-serif;` ensures a readable font.
    
4. `box-sizing: border-box;` alters the box model to include padding and border within the element's total width and height.
    

Setting the Stage: Background and Card Styling

```css
body{
    background-color: #222;
}
.card{
    /* Styling for the card container */
}
```

1. `background-color: #222;` sets the backdrop to a dark shade, creating a dramatic ambiance.
    

Card Design and Layout

```scss
.card{
    /* ... */
    width: 90%;
    max-width: 470px;
    background: linear-gradient(50deg, #54b8d1, #503eb8);
    color: #fff;
    margin-top: 100px;
    margin-left: 480px;
    border-radius: 25px;
    padding: 40px 35px;
    text-align: center;
}
```

1. `width: 90%; max-width: 470px;` ensures the card remains responsive, adapting to various screen sizes.
    
2. `background: linear-gradient(50deg, #54b8d1, #503eb8);` crafts a gradient background that adds vibrancy.
    
3. `color: #fff;` sets the text color to white for high contrast.
    
4. `margin-top: 100px;` pushes the card down from the top.
    
5. `margin-left: 480px;` centers the card horizontally.
    
6. `border-radius: 25px;` provides a subtle rounded corner effect.
    
7. `padding: 40px 35px;` offers ample padding inside the card.
    
8. `text-align: center;` centers the content within the card.
    

Search Bar Styling

```css
.search{
    /* ... */
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.search input{
    /* ... */
    border: 0;
    outline: 0;
    background: #ebfffc;
    color: #555;
    /* ... */
    border-radius: 30px;
}
.search button{
    /* ... */
    border: 0;
    outline: 0;
    background: #ebfffc;
    border-radius: 50%;
    /* ... */
}
```

1. `display: flex; align-items: center; justify-content: space-between;` arranges the input and button side by side.
    
2. Input styling includes removing borders, setting background color, and providing a subtle text color.
    
3. `border-radius: 30px;` curves the input edges.
    
4. Button styling eliminates borders, adds a background, and gives it a rounded appearance.
    
5. `border-radius: 50%;` transforms the button into a circular shape.
    

Visual Elements and Details

```css
.weather-icon{
    /* ... */
    width: 170px;
    margin-top: 30px;
}
.weather-h1{
    /* ... */
    font-size: 80px;
    font-weight: 500;
}
.weather-h2{
    /* ... */
    font-size: 45px;
    font-weight: 400;
    margin-top: -10px;
}
.details{
    /* ... */
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0px 20px;
    margin-top: 50px;
}
```

1. `width: 170px; margin-top: 30px;` adjusts the weather icon size and provides spacing.
    
2. `font-size: 80px; font-weight: 500;` increases the font size and emphasizes the temperature.
    
3. `font-size: 45px; font-weight: 400;` defines the font size and weight for the city name.
    
4. `margin-top: -10px;` shifts the city name slightly upwards.
    
5. `display: flex; align-items: center; justify-content: space-between;` arranges the humidity and wind elements side by side.
    
6. `padding: 0px 20px;` offers padding to the weather details.
    
7. `margin-top: 50px;` provides spacing from the temperature and city name.
    

Fetching and Displaying Weather Data

Now, let's dive into the JavaScript code that fetches and displays weather data from the OpenWeatherMap API.

```javascript
// API key provided by OpenWeatherMap
const apiKey = "YOUR_API_KEY";

// Selecting HTML elements
const searchBox = document.querySelector('.search input');
const searchBtn = document.querySelector('.search button');
const apiUrl = `https://api.openweathermap.org/data/2.5/weather?&units=metric&q=`;

// Function to fetch and display weather data
async function checkWeather(city) {
    const response = await fetch(apiUrl + city + `&appid=${apiKey}`);
    const data = await response.json();

    // Display weather information
    document.querySelector(".city").innerHTML = data.name;
    document.querySelector(".temp").innerHTML = Math.round(data.main.temp) + "°C";
    document.querySelector(".humidity").innerHTML = data.main.humidity + "%";
    document.querySelector(".wind").innerHTML = Math.round(data.wind.speed) + " km/h";
}

// Event listener for search button
function searching() {
    searchBtn.addEventListener('click', () => {
        checkWeather(searchBox.value);
    });
}
searching();
```

Understanding the Code

1. The provided API key is stored securely in the `apiKey` variable.
    
2. HTML elements for the search box and search button are selected using the `querySelector` method.
    
3. The OpenWeatherMap API URL is structured in the `apiUrl` variable, incorporating query parameters for units and city name.
    
4. The `checkWeather` function asynchronously fetches weather data by combining the API URL, city name, and API key. The fetched JSON data is then displayed in designated HTML elements.
    
5. The `searching` function adds an event listener to the search button. When clicked, it triggers the `checkWeather` function with the value from the search input.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1692383066647/bbf43063-1843-4e17-a15b-3bc1c791dd08.png align="center")

**Conclusion**

By following this tutorial, you've crafted a fully functional weather app that harnesses the power of JavaScript and the OpenWeatherMap API. This project demonstrates the potential of dynamic web development and the integration of APIs to enrich user experiences. Remember that this app can serve as a starting point for further expansion—whether you're interested in refining the user interface, integrating additional features, or exploring other APIs. Through the creative fusion of code and data, you've built a tool that empowers users to access crucial weather information with just a few clicks. Happy coding and exploring the world of web development!