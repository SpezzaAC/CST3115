# CST3115
# Spencer, Edward, Tim, Harryson

API key was gotten from https://www.weatherapi.com/

Key features that were implemented incude:
- Android project in Kotlin
- Main activity serves as app's entry point
- Two screens using Jetpack compose: Main and settings
- Main: Displays the daily weather for the selected city
- Settings: Allows the user to change their selected city using SharedPreferences
- Uses NavController for screen navigation
- Uses SharedPreferences to store the users city of choice
- Integrates a free weather API
- GET request to fetch current weather data for the selected city
- Parse JSON responses into Kotlin data classes
- Update's UI after each successful data fetch
- Uses coroutines for all network calls
- Basic error handling around API requests
- Displays appropriate weather icons
- Includes a simple loading indicator while fetching data
- Displays a basic error message if the API call fails

Limitations:
Proper integration of WorkManager and the 5 day forecast display is not seen on the application. While attempts were made to include these features within the application, not everything could be completed in-time and was therefore not included.

However, the code that we made to use as part of the integration of WorkManagwer and the 5 day forecast is still present within the application and can be found in the files, but none of it is in use. A refresh button was added in replacement of the WorkManager.
