Project Title: Water Tracker App 💧
Objective
The primary objective of this project is to develop a simple Android application that helps users track their daily water intake. This app demonstrates core Android development concepts, including UI design, data persistence using 

SharedPreferences, and event handling. The project aims to provide a practical understanding of building a functional and user-friendly mobile application.

Features
Water Tracking: Users can track their water consumption by tapping a button to add a glass of water.

Progress Visualization: A circular progress bar visually represents the user's progress towards their daily goal of 8 glasses.

Customizable Glass Volume: Users can set a custom volume for a single glass of water in milliliters (ml).

Daily Goal Message: A congratulatory message appears once the daily goal is reached.

Data Persistence: The app saves the water count, total volume, and custom glass size using SharedPreferences, so the data is not lost when the app is closed.

Reset Functionality: A reset button allows users to clear their daily count and start over.

Challenges Faced and Solutions
Challenge: Implementing a dynamic progress bar that accurately reflects the water count.

Solution: By setting the progressBar.max to the dailyGoal variable and updating the progressBar.progress with the current waterCount in the updateUI() function, the progress bar now correctly visualizes the user's progress.

Challenge: Ensuring data is saved between app sessions.

Solution: We used SharedPreferences to store the waterCount, totalVolumeML, and volumePerGlassML in the onPause() lifecycle method. This allows the app to load the saved data when it is reopened, ensuring a continuous user experience.
