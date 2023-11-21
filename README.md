# Weather-App-pro3
this a web Weather App pro3
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Weather App</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }

        #weather-container {
            margin-top: 50px;
        }

        #temperature {
            font-size: 2em;
            margin-bottom: 10px;
        }

        #description {
            font-size: 1.2em;
            color: #666;
        }

        #location {
            font-size: 1.5em;
            margin-top: 10px;
        }

        #input-container {
            margin-top: 20px;
        }

        #cityInput {
            padding: 5px;
            font-size: 1em;
        }

        #getWeatherBtn {
            padding: 5px 10px;
            font-size: 1em;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Weather App</h1>
    
    <div id="input-container">
        <label for="cityInput">Enter City:</label>
        <input type="text" id="cityInput" placeholder="Enter city name">
        <button id="getWeatherBtn" onclick="getWeather()">Get Weather</button>
    </div>

    <div id="weather-container">
        <div id="temperature"></div>
        <div id="description"></div>
        <div id="location"></div>
    </div>

    <script>
        function getWeather() {
            // This is a placeholder. In a real-world scenario, you would use a weather API.
            // Replace the following lines with code to fetch real-time weather data.

            var temperature = Math.floor(Math.random() * 30) + 1; // Random temperature for demonstration
            var description = "Partly Cloudy"; // Random description for demonstration
            var city = document.getElementById('cityInput').value;

            document.getElementById('temperature').innerText = temperature + "°C";
            document.getElementById('description').innerText = description;
            document.getElementById('location').innerText = "Weather in " + city;
        }
    </script>
</body>
</html>
