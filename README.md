# Weather-Forecast-Web-page
A simple weather web page using Html, CSS, Java script and Python

Hello group members! For our first group project we will be coding a weather forecast web page. The group will be split into 2 teams, frontend and backend. Marvin will also assist the frontend or help guide them with his experience on frontend. The deadline will be set after we have a meeting to discuss how we will fit these group projects to our schedules in order to not let them interrupt our other work commitments. For now read up and get all the information you need to tackle this project.

Frontend Team:
Thando
Luyanda
Phezile

Frontend Team Steps:
The frontend is responsible for how the app looks and how users interact with it. This will involve setting up the user interface, handling user input, and displaying data received from the backend.

1. Project Setup
Set up a basic project structure, including creating a folder for your frontend (frontend/) and initializing the necessary files (index.html, styles.css, app.js).
2. Design the User Interface (UI)
Header: Add a title or logo for your weather forecast app.
Search Bar: Include an input field where users can type in the name of a city.
Submit Button: Add a button next to the input field that the user can click to trigger the search.
Weather Information Display: Create a section where the weather details will be displayed (temperature, weather condition, etc.).
Error Handling: Plan for an error message that will be shown if the user enters an invalid city or if there's an issue fetching the weather data.
3. Style the UI
Use CSS to make the layout visually appealing and user-friendly.
Ensure the page is responsive (works well on both mobile and desktop).
4. Handle User Input
Create a function to capture the city name entered by the user.
Attach an event listener to the submit button so that when it’s clicked, it triggers the action to fetch weather data.
5. Fetch Data from Backend
Implement a function to send a request to the backend (using fetch() or XMLHttpRequest).
Pass the city name as a query parameter in the request.
When the backend responds, display the weather information (e.g., city, temperature, weather condition) in the UI.
If there’s an error, show an appropriate error message in the UI.
6. Test and Integrate
After completing the interface and data fetching logic, test the app with multiple cities and ensure data is displayed correctly.
Ensure proper error handling is in place (e.g., city not found or bad API response).
Refine the UI based on feedback or any issues encountered during testing.


Backend Team:
Marvin
Vercus
Sane
Ntshuxeko

Backend Team Steps:
The backend will be responsible for handling requests from the frontend, fetching data from an external weather API, and returning the relevant data.

1. Set Up Server
Set up a backend framework (like Express in Node.js) to handle incoming HTTP requests from the frontend.
Ensure the server can handle API routes for weather data, such as /weather.
2. Connect to Weather API
Choose a weather API service (such as OpenWeatherMap, AccuWeather, etc.).
Register for an API key from the chosen weather service.
Set up an API request to fetch weather data based on the city name passed as a query parameter.
3. Handle API Request
Receive the city name from the frontend through a GET request (e.g., /weather?city=London).
Use the weather API to fetch the weather details for the requested city (temperature, conditions, etc.).
Parse the API response and extract the necessary weather details.
4. Error Handling
Handle errors like invalid city names, no response from the weather API, or network issues.
Return a meaningful error message (e.g., "City not found") if an error occurs during the API request.
5. Send Data Back to Frontend
Once you have the weather data (or an error message), send the response back to the frontend in JSON format.
Ensure the response contains all the necessary data (city name, temperature, weather condition) or an error message.
6. Set Up CORS (Cross-Origin Resource Sharing)
If your frontend and backend are running on different domains or ports during development, you’ll need to enable CORS to allow the frontend to make requests to the backend.
7. Test API
Test the API route to make sure the server is correctly fetching weather data.
You can use tools like Postman or cURL to test the backend API independently before integrating it with the frontend.


Integration and Final Steps:
1. Integrate Frontend and Backend
Ensure the frontend is sending requests to the backend correctly and receiving the weather data.
Display the weather data from the backend on the frontend UI.
Make sure the user can input a city, click the "Get Weather" button, and see the correct weather details displayed.
2. Test the Full Application
Test the entire flow from start to finish:
Enter a valid city, see the weather data.
Enter an invalid city, see an error message.
Handle edge cases like network failures or invalid input.
3. Refine and Optimize
Optimize the UI for better user experience (e.g., loading indicators while waiting for data).
Ensure the code is clean, readable, and well-documented.
4. Deploy
Once everything is working well locally, deploy the backend (e.g., on Heroku or another cloud platform) and the frontend (e.g., on Netlify, Vercel, or GitHub Pages).
Ensure both the frontend and backend are connected after deployment.

