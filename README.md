Simple Weather App A lightweight web application that fetches real-time weather data for any city using the OpenWeatherMap API. Built with JavaScript, HTML, and styled with Tailwind CSS, this app provides a responsive and user-friendly interface to check temperature, weather conditions, humidity, and wind speed. Features

Search weather by city name (e.g., "London,UK"). Displays temperature (°C), weather description, humidity, and wind speed. Responsive design for mobile and desktop. Error handling for invalid city names or API issues. Weather icon display for current conditions.

Demo Check out the live app hosted on GitHub Pages (replace with your actual URL after setting up). Prerequisites

An OpenWeatherMap API key. Sign up for a free account to obtain one. A modern web browser (Chrome, Firefox, Safari, etc.).

Setup Instructions

Clone the Repository: git clone https://github.com/your-username/weather-app.git cd weather-app

Get an API Key:

Sign up at OpenWeatherMap and navigate to the "API keys" section in your account. Copy your API key.

Configure the API Key:

Open index.html in a text editor. Find the line in the <script> section:const apiKey = 'YOUR_API_KEY';

Replace 'YOUR_API_KEY' with your actual OpenWeatherMap API key.

Run the App:

Option 1: Open index.html directly in a browser (note: may encounter CORS issues). Option 2: Use a local server for development:npx http-server

Or use VS Code’s Live Server extension. Access the app at http://localhost:8080 (or the provided port).

Deploy to GitHub Pages (Optional):

Push your code to a GitHub repository. Go to the repository’s "Settings" > "Pages." Set the source to the main branch and / (root) folder. Your app will be live at https://your-username.github.io/weather-app.

Usage

Enter a city name in the input field (e.g., "London,UK" or "New York,US"). Click the "Get Weather" button. View the weather details, including temperature, description, humidity, and wind speed. For ambiguous city names, include the country code (e.g., "Springfield,US").

Technologies Used

HTML5: Structure of the web app. JavaScript: Fetching and processing API data. Tailwind CSS: Responsive and modern styling. OpenWeatherMap API: Weather data source.

Notes

The API uses metric units (°C). To use Fahrenheit, modify the API URL in index.html by changing units=metric to units=imperial. The free OpenWeatherMap API tier is sufficient, with limits of 60 calls/minute and 1,000,000 calls/month. Avoid hardcoding your API key in a public repository. Consider using environment variables or a backend proxy for production.

Troubleshooting

"Invalid API key": Ensure your API key is correct and active. Wait 10-30 minutes for new keys to activate. "City not found": Check spelling or include the country code (e.g., "Paris,FR"). Test with major cities like "Tokyo,JP". **CORS issuesස

Contributing Contributions are welcome! Feel free to submit issues or pull requests for improvements. License This project is licensed under the MIT License. Acknowledgments

OpenWeatherMap for providing the weather API. Tailwind CSS for styling.
