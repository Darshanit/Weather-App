# Weather App README

## Overview

This is a simple weather application built using Python's Tkinter library. The app allows users to enter a city name and retrieve current weather conditions, including temperature, wind speed, humidity, atmospheric pressure, and a brief description of the weather. It also displays the local time for the specified city.

## Features

- **City-Based Weather Search:** Users can input any city name to get real-time weather data.
- **Temperature Display:** The app shows the current temperature in Celsius.
- **Weather Conditions:** Displays weather conditions like wind speed, humidity, pressure, and a brief description.
- **Time Zone Support:** The local time of the entered city is displayed.
- **User-Friendly Interface:** A clean and intuitive graphical user interface (GUI) for easy interaction.

## Requirements

- Python 3.x
- The following Python libraries:
  - `tkinter`
  - `geopy`
  - `timezonefinder`
  - `requests`
  - `pytz`

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/weather-app.git
   cd weather-app
   ```

2. **Install required libraries:**
   ```bash
   pip install geopy timezonefinder requests pytz
   ```

3. **Run the application:**
   ```bash
   python weather_app.py
   ```

## How to Use

1. **Enter a city name:** In the search box at the top of the window, enter the name of the city for which you want to check the weather.
2. **Get Weather Info:** Click on the search icon to fetch and display the weather details.
3. **View Results:** The app will display the current temperature, weather condition, wind speed, humidity, atmospheric pressure, and a brief description. The local time for the city will also be shown.

## Project Structure

- **`weather_app.py`**: The main Python file containing the application code.
- **`/assets`**: Folder containing image assets used in the app (search icon, logo, etc.).
  
  Ensure that the image paths used in the code are correctly mapped to the location of your images.

## API Usage

The app uses the OpenWeatherMap API to fetch weather data. You will need to replace the API key in the following line with your own:

```python
api="https://api.openweathermap.org/data/2.5/weather?q="+city+"&appid=your_api_key_here"
```

To get your API key, sign up at [OpenWeatherMap](https://home.openweathermap.org/users/sign_up).

## Customization

- **Change Units:** By default, the temperature is displayed in Celsius. You can change it to Fahrenheit by modifying the calculation in the `getWeather()` function.
- **Update UI:** Feel free to customize the appearance of the app by adjusting the Tkinter widgets (e.g., colors, fonts, positions).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Enjoy your weather app! If you encounter any issues, feel free to open an issue on the GitHub repository or contribute to the project.
