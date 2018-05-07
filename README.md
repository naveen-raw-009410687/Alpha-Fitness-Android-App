# FitnessApp
CS 175 - Programming Assignment #2

An Android Fitness Application that tracks the users activities and promotes their wellness by using Google Maps API to track their location and movements

CS 175, Spring 2018
Programming Assignment #2 Advanced Android Programming Programming Assignment – 50 points
Naveen Rawat sjsu id: 009410687
YouTube link: https://youtu.be/oNsQGc6c6UI
Also GitHub source code link:
https://github.com/naveen-raw-009410687/Alpha-Fitness-Android-App
Design Feature Highlights:
Alpha Fitness Android App:
Android phone application that keep tracks of user's workout activity
Features:
• Real-time update of workout steps walked distance
• Real-time update of workout time
• Real-time update of step counts
• Calorie counter
• Use of fragment concepts
• Orientation sensor (landscape or portrait)
• Geolocation with Google maps API
• Data saved to database with SQLite
• Real-time graph plotting of calories & step counts

A) User Interface (20 Points):
I) The Record Workout Screen: (7 points)
• Contain a button to activate the Profile screen - 1 point Done

• When changing to landscape mode, the Workout Details screen will be shown - 1 point  Done
• When changing back to portrait mode, the Record Workout Screen will be shown - 1 point Done

• Show distance with real-time update - 1 point  Done
• Show duration with real-time update - 1 point  Done
• Fragment is used in the design - 1 point  Done

<FrameLayout android:name="edu.sjsu.nrawat.alphafitness.PortraitFragment" android:id="@+id/portrait_fragment" android:layout_weight="1"
android:layout_width="0dp" android:layout_height="match_parent" />
<FrameLayout android:name="edu.sjsu.nrawat.alphafitness.WorkoutDetailsLandscape"
android:id="@+id/landscape_fragment" android:layout_weight="1" android:layout_width="0dp" android:layout_height="match_parent" />
\
private Fragment fragment;
private final String RECORD_WORKOUT = "RecordWorkoutFragment"; private final String WORKOUT_DETAILS = "WorkDetailsFragment";
• Has a Start Workout button to control the start/stop of the workout - 1 point Done

II) The Workout Details Screen: (6 points)
• Contain all UI elements:AVG, MAX, MIN, and Chart -4 points
Done
• Real-time update of AVG, MAX, MIN info - 2 points Done


III) Profile Screen: (7 Points)
• All elements are present: Name, User Info, AVG/Weekly, All Time -
2 points Done
• Able to modify User name and User Info - 2 points  Done

• Statistics can be updated in real-time (not fixed) - 2 points  Done
• Able to go back to the previous screen (Record Workout) - 1 point
Done

B) Remote Service and Content Provider (10 Points):
• A remote service keeps recording the workout data in the
background. - 4 points Done
• Workout session data is saved to SQLite database - 3 points  Done

• Content Provider is used - 3 points Done
C) GPS and Google Map (10 Points):
• Google Map service is used properly - 4 points  Done

• Google Map is centered - 1 point  Done
• The path of user’s workout session is shown - 5 points Done Blue line tracking run.
D) Rubric for Estimating Calories and Distance from Step Counts (10 Points):
• Calories is estimated from Step Counts - 2 points  Done
• Distance is estimated from Step Counts - 2 points  Done

• Real-time plotting of Calories and Step Counts are provided - 6 points Done

