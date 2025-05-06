# Weather Window Project

## Overview
Weather Window is an interactive web application that transforms weather data into a dynamic visual experience. Instead of traditional weather icons, it renders a real-time animated window view that changes based on current weather conditions, time of day, and location.

## Features
- Real-time Weather Visualization:
  - Sunny, cloudy, rainy, and clear night scenes
  - Dawn/dusk transitions with appropriate lighting
  - Animated rain, clouds, and stars

- Location-Based:
  - Automatic geolocation detection
  - Search for any city worldwide
  - Timezone-aware time displays

- Technical Highlights:
  - Uses Open-Meteo Weather API
  - Pure CSS animations
  - Responsive design
  - No external libraries (vanilla JavaScript)

## Installation
No installation required - runs directly in modern browsers:
1. Clone the repository
2. Open index.html in any modern browser
Or access the live version at: [Live Demo URL]

## Usage
- On Load:
  - The app will request location permission to show local weather
  - If denied, defaults to New York weather

- Search:
  - Type any city name in the search bar
  - Select from dropdown results

- Information Display:
  - Current temperature (Fahrenheit with Celsius small)
  - "Feels like" temperature
  - Wind speed and humidity
  - Local time

## API Used
Open-Meteo Weather API:
- Free weather API with generous limits
- Provides:
  - Current temperature
  - Weather codes
  - Humidity
  - Wind speed
  - Timezone data

## Customization
To modify the visual effects:
- Change Colors:
  - Edit the gradient backgrounds in setScene() function
  - Example: bg = 'linear-gradient(to top, #87CEEB, #ffffff)'

- Adjust Animations:
  - Modify CSS @keyframes in the style section
  - Example: Change @keyframes rainFall for different rain speeds

- Add New Weather Types:
  - Extend the setScene() switch statement
  - Add new condition checks and corresponding visual elements

## Troubleshooting
Issue: Location not loading
Fix:
- Check browser permissions
- Verify internet connection
- Console log any API errors

Issue: Time displays incorrectly
Fix:
- Verify the timezone returned from API
- Check updateTime() function calculations

## Future Enhancements
- Add snowfall for winter conditions
- Implement weather forecasts
- Add day/night cycle transitions
- Mobile app version

## Credits
- Weather data by Open-Meteo
- Inspired by lo-fi aesthetic designs
- Developed by Deceli Soto

## License
MIT License - Free for personal and commercial use
