# Live Weather Dashboard with Fetch API

A weather website that fetches live data from the free Open-Meteo API.
Search any city to see the current conditions and a 5-day forecast.
Built with HTML, CSS and asynchronous JavaScript (fetch and async/await).

**Live app:** file:///C:/Users/ujosh/Downloads/Live%20Weather%20Dashboard%20(preview).html

## Features
- City search using the Open-Meteo Geocoding API (no API key needed)
- Current temperature, humidity, wind and weather icon
- 5-day forecast with daily high and low temperatures
- Input validation (empty, too short, invalid characters)
- Loading, empty, error and success states
- Remembers the last searched city using localStorage
- Responsive layout for phones, tablets and desktops

## How I handle errors
- Empty or invalid input is checked before any request is sent.
- `response.ok` is checked before reading the JSON.
- An unknown city shows "City not found", and a failed request shows a clear message.
- A network failure (a `TypeError` from `fetch`) shows "Network problem".
- The search button is disabled while loading, so requests are not repeated.
- User text is shown with `textContent`, never `innerHTML`.

## Files
- `index.html` - page structure
- `style.css` - styles and responsive layout
- `script.js` - API calls, rendering and state handling
