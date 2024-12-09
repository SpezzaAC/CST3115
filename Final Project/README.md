# CST3115 - Final Project
# Spencer, Edward, Tim, Harryson

## Setup
### API Key:
The API key is from Google Cloud Console, and is **Not** included within the submission (for security purposes), as you must have an active Google Console account. To use this code, login/signup to Google Cloud Console, "get started" with Google Maps SDK, and enable (if not already) the "Static Maps API" feature.
<br>If enabled, copy the API key, and paste it into the "Map Activity", line "34" - replacing "API_KEY" with your actual key.
### Log Into App:
To log into the Noble Threads app, use the following credentials:
- **Username**: username
- **Password**: password

## App's Structure
The app structure is as follows:
- MainActivity:
  - Contains the NavController for application.
  - Contains variables that multiple activities need to access and modify.
- LoginActivity:
  - Allows the user to login after entering a correct username and password.
  - We defaulted this to ‘username’ and ‘password’.
- BrandActivity:
  - Acts almost as the “Main Menu” after the user logs in.
  - Shows all the available brands to the user.
  - Allows for navigation to any selected brand.
  - Checkout and favourites list are also accessible here.
  - Logout button to return to LoginActivity.
- ItemsActivity:
  - Displays the items that are relevant to the users selected brand.
  - Allows the user to navigate back to their cart.
  - Back button to the return to the BrandActivity.
- DetailsActivity:
  - Displays information relevant to the specific item selected.
  - Button to add to the users cart, navigate to cart.
  - Button to add to the favourites list.
  - Button to view store location on Google Maps as a Static Map.
  - Back button to return to the ItemsActivity.
- CartActivity:
  - Allows the user to see their selected items relevant to their cart.
  - This list is NOT saved after a user closes the application.
  - Allows the user to remove specific items from their cart.
  - Allows the user to checkout, navigating to CheckoutActivity and removes all items in the cart.
  - Back button to return to the BrandActivity.
- CheckoutActivity:
  - Displays some information regarding the action of a completed checkout.
  - Button to return to cart, returning to CartActivity.
  - Button to return to Brands, returning to BrandActivity.
  - Button to Log Out, returning to the LoginActivity.
- MapActivity:
  - Contains the Static Map regarding the store location.
  - Uses Google APIs to generate the Static Map (Key not included in submission).
  - Back button to return to the BrandActivity.
- FaveActivity:
  - Displays the list of favorited items that were saved and retrieved from the Room database.
  - Buttons to remove specific items from the list and the database.
  - Back button to return to the BrandActivity.
- AppDatabase:
  - Creates the database primarily used by the FaceActivity.
- Fave:
  - Data class containing all of the information regarding a save to the database for a new favorited item.
- FaveDao:
  - Fave Data Access Model - allows for database manipulation and data retrieval.
- FaveViewModel:
  - Contains the coroutines that allow parts of the program's favourite list database to run asynchronously.
- FaveViewModelFactory:
  - Helps to provide the FaveViewModel with the proper application context.

## Team Member Contributions
The overall team collaboration/contributions was good and even. In particular:
- **Spencer:** Map API implementation, project report, and presentation (lead).
- **Edward:** Primary developer (backend logic).
- **Harryson:** User interface (UI) implementation.
- **Tim:** Products (lists and details), testing and support.

