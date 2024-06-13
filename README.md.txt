MULTITHREDED APPLICATION

DESCRIPTION:
                         Given code is in python language and about Multithreded application. The GUI of given code also developed which displays the temprature and weather of mentioned cities.
 
1. There are 6 threds and 3 functions in  givem code. 
2. One function is used to  fetch temprature weather and a random city. 
3. 2nd function is used to change the city name. 
4 3rd function is used to display or for GUI. 
5. There is no sensitivity between temprature, weather and city name.  It display a random city. 
6. Given cide is very simple and easy to understand and to change. 

.................................................................................... GROUP MEMBERS....................................................................................
SECTION BSIT 4th (ss2).
1. Muhammad Zeeshna Sabir(BSIT51F22S073).
2. Fawad(BSIT51F22S068).
3. Jawad Jamshed(BSIT51F22S074).
4. Habib Ullah Ahsan(BSIT51F22S070).

..........................................................................FROM UNOVERSITY OF SARGODHA.......................................................................

Sure, here is a step-by-step summary of the provided code:

# Imports and Setup

1. Imports:
   - The code imports necessary modules: `threading`, `time`, `random`, `tkinter` and `ttk` from `tkinter`.

2. Mock Function:
   - `fetch_weather(city)`: Simulates fetching weather data by introducing a random delay and returning random weather information for the given city.

### Functions

3. Update City Weather:
   - `update_city_weather(city, label)`: This function continuously fetches and updates the weather data for a specific city. It updates the label with new weather data every 5 seconds.

4. Periodic Weather Update:
   - `update_weather_periodically(city_labels)`: This function fetches and updates the weather data for all cities at regular intervals (every 60 seconds).

# City List

5. Cities:
   - A list of cities (`cities`) is defined: 'New York', 'London', 'Paris', 'Tokyo', 'Sydney'.

# Tkinter Application

6. **Main Window**:
   - `root = tk.Tk()`: Initializes the main application window with the title "Weather Application" and background color `#2E4053`.

7. **Styles Configuration**:
   - Configures styles for frames and labels using `ttk.Style`.

# Creating City Frames and Labels

8. City Frames and Labels:
   - A loop iterates over the list of cities. For each city:
     - A `ttk.Frame` is created and styled, and added to the main window grid.
     - A `ttk.Label` is created within each frame to display weather data.
     - Each label initially displays "Fetching..." until updated.
     - The labels are stored in a dictionary (`city_labels`).

#Threads for Updating Weather Data

9. Update Threads:
   - For each city, a thread is started that continuously updates the city's weather data using the `update_city_weather` function.
   - An additional thread is started to periodically update the weather data for all cities using the `update_weather_periodically` function.

### Main Loop

10. **Main Application Loop**:
    - `root.mainloop()`: Starts the Tkinter main loop to keep the application running and responsive.

In summary, this code creates a Tkinter application that displays weather information for a list of cities. Each city's weather data is fetched and updated in real-time using separate threads to ensure the GUI remains responsive. The weather information is simulated with random values and updated at regular intervals.
