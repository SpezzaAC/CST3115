# CST3115
# Spencer, Edward, Tim, Harryson

## Setup
### API Key:
The API key is from Google Cloud Console, and is **Not** included within the submission (for security purposes), as you must have an active Google Console account. <br>To use this code, login/signup to Google Cloud Console, "get started" with Google Maps SDK, and enable (if not already) the "Static Maps API" feature.
If enabled, copy the API key, and paste it into Line... **(fill in code details)**.
### Log Into App:
To log into the TechFix app, use the following credentials:
- **Username**: username
- **Password**: password <br><br>
*Note*: Once you log into the app once, the app saves the login info in SharedPreferences.

## Key App Features
- Android project in Kotlin
- Login screen with hardcoded credentials
- Main Screen with button options for taks, location, and logout.
- Location of user
- List of daily tasks (client name, address, and job description) with ability to mark as complete
- Google Maps SDK displaying a static map with predefined client locations
- SharedPreference to securely store login state

## App's Structure
The general app structure is as follows:
- mainActivity
  -  (acts as the NavController)
- menuActivity
  - (includes logic for currentLocation)
- loginActivity
  - About
- taskList
  - About 
- staticMap
  - About 

## Team Member Contributions
The overall team collaboration/contributions was good and even. In particular:
- Spencer: UI developer (Login screen + logic, main screen, etc.), + documentation
- Edward: Location Developer (Primary app logic, UI, testing, etc.) + documentation
- Tim: Co-Feature Developer (task list, etc.)
- Harryson: Co-Feature Developer (task list, etc.)
