# CODTECH-Task1
Name: THUMUGANTI LAHARI

Company: CODTECH IT SOLUTIONS

ID: CT8WD1420

Domain: WEB DEVELOPMENT

Duartion: JUNE 25th 2024 TO AUGUST 25TH 2024

**OVERVIEW OF THE PROJECT**

Project: WEATHER FORECAST APP

Objective:
To create a user-friendly web application that allows users to quickly and easily search for weather information based on a specific location. By providing a simple interface with a search bar, the app enables users to input their desired location and receive relevant weather data, including temperature, weather description, and a corresponding icon. The app aims to streamline the process of accessing weather forecasts, making it a convenient tool for individuals who want to stay informed about the weather conditions in their chosen locations.

It builds a simple weather forecast app using HTML, CSS, and JavaScript. Here's a breakdown of each part:

**HTML (index.html):**

-Defines the basic structure of the web page.

-Links the CSS file (style.css) for styling and the JavaScript file (app.js) for functionality.

-Creates a form (#form) with a search bar (#search) for users to input the location they want weather for.

-Includes a main section (#main) where the weather information will be displayed.

**CSS (style.css):**

-Sets up a basic foundation for styling using box-sizing: border-box; for consistent element sizing.

-Defines styles for the entire body element:

  *Centered content using justify-content: center; and align-items: center;*

  *Minimum height (min-height: 100vh;) to cover the viewport*

  *Background color and font family*

-Styles the search bar input:

  *Rounded corners (border-radius: 25px;)*
  
  *Padding and background color*

  *Basic shadow effect (box-shadow)*

  *Minimum width (min-width: 300px;)*

  *Removes outline on focus*

-Defines styles for the .weather class, likely used for the weather information section after user input.

  *Centered text (text-align: center;)*

  *Font size (font-size: 2rem;)*

  *Styles for the h2 element within .weather*

  Removes bottom margin (margin-bottom: 0;)

Centers content horizontally (display: flex; align-items: center;)

**JavaScript (app.js):**

-Defines the API key (apiKey) used to access weather data from OpenWeatherMap.

-Selects elements from the HTML:

*main section*

*Search form (#form)*

*Search input field (#search)*

-Creates a function url(city) to construct the API request URL based on the provided city name.

-Defines an asynchronous function getWeatherByLocation(city):

*Fetches weather data from the OpenWeatherMap API using the constructed URL.*

*Parses the response into JSON format (respData).*

*Calls addWeatherToPage(respData) to display the weather information.*

-Defines a function addWeatherToPage(data):

*Converts temperature from Kelvin to Celsius using Ktoc(data.main.temp).*

*Creates a new div element with the class weather.*

*Sets the inner HTML of the div to display:*

*1.The temperature in Celsius with an icon from OpenWeatherMap*

*2.A description of the weather*

*Clears the main section content and adds the new weather information.*

-Defines a function Ktoc(K) to convert Kelvin (K) temperature to Celsius (°C).

-Attaches an event listener to the form's submit event:

*Prevents default form submission behavior (e.preventDefault();).*

*Retrieves the entered city name from the search input field (search.value).*

*If a city is entered, calls getWeatherByLocation(city) to fetch and display the weather data.*

**Overall functionality:**

1.User enters a city name in the search bar.

2.Upon form submission, the JavaScript code retrieves weather data from OpenWeatherMap based on the entered city.

3.The retrieved data (temperature in Kelvin, weather description, and icon) is converted and displayed on the page within the main section.

*This is a basic implementation and can be further enhanced to display additional weather information (e.g., humidity, wind speed).*

*Error handling can be added to handle cases where the user enters an invalid city name or no city name at all.*

*You might need to create an account with OpenWeatherMap to obtain a valid API key.*
