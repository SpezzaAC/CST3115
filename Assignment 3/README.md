# CST3115
# Spencer, Edward, Tim, Harryson

## Setup
### API Key:
The API key is from Google Cloud Console, and is **Not** included within the submission (for security purposes), as you must have an active Google Console account. To use this code, login/signup to Google Cloud Console, "get started" with Google Maps SDK, and enable (if not already) the "Static Maps API" feature.
<br>If enabled, copy the API key, and paste it into the "StaticMapActivity", line 38 - replacing "YOUR_API_KEY" with your actual key.
### Log Into App:
To log into the TechFix app, use the following credentials:
- **Username**: username
- **Password**: password <br><br>
*Note*: Once you log into the app once, the app saves the login info in SharedPreferences.

## Key App Features
- Android project in Kotlin
- Login screen with hardcoded credentials
- Main Screen with button options for tasks, location, and logout.
- Location of user
- List of daily tasks (client name, address, and job description) with ability to mark as complete
- Google Maps SDK displaying a static map with predefined client locations
- SharedPreference to securely store login state

## App's Structure
The general app structure is as follows:
- mainActivity
  -  Acts as the NavController and stores necessary application data.
- menuActivity
  - Allows user to navigate between the different activities - also contains the logic for the current location button which utilizes staticMap.
- loginActivity
  - Allows the user to access the application after a successful username and password entry. The login state saves as a SharedPreference, meaning closing the application without logging out will leave you logged in.
- taskList
  - Displays a list of tasks, currently filled with hardcoded made-up data. Tasks can be marked as complete which removes them from the list, and each location for each task can be seen in the staticMap. 
- staticMap
  - Uses Google API's to display a static map based on the selected location from either the taskList or the current location selected in the menuActivity 

## Team Member Contributions
The overall team collaboration/contributions was good and even. In particular:
- Spencer: UI developer (Login screen + logic, main screen, etc.), + documentation
- Edward: Location Developer (Primary app logic, UI, testing, etc.) + documentation
- Tim: Co-Feature Developer (task list, etc.)
- Harryson: Co-Feature Developer (task list, etc.)
