# What is a Widget?
- UI components, such as TextView, Buttons, etc.
- `View` object.

# What is a Layout?
- Containers controlling how their child views are positioned.
- `ViewGroup` object.

# Describe the relationship between `ViewGroups` and `View`
![Relationship between ViewGroups and Views](https://developer.android.com/images/viewgroup_2x.png)

# What is `ConstraintView`?
Defines position of each view based on sibling and parent view constraints. This is the preferred method for creating responsive views.

# What is a constraint?
Every widget is placed relatively to the layout and other widgets.

# What is a string resource file?
Contains all your UI strings. File is called strings.xml.

# What is a chain?
A linear group of views with bidirection constraint. You can use it to evenly space views out.

# What does match constraints mean?
The width of a view expands to meet the definition of the horizontal constraints. The width of the textbox fills the horizontal space after all margins are accounted for.

# Activity: Create a UI that contains a text box and a button. When the user clicks the button, the text box string must be displayed on the next page. Code a back button on the next page. The following rules apply:
- Must use `ConstraintLayout`.
- The top margin must be 16 DP. The left margin of the text box and the space between the text box and the button must be 16 DP. The left margin of the button must be 16 DP.
- Constrain the text box and button widgets in a horizontal alignment (Hint: use baselines).
- Make the text box responsive to the width of different screen sizes (Hint: use chaining).
- The text view in the second activity must be centralized.
- Assign a string value to the text box and button via the string resource file.

# What is an Intent?
- A message that activates broadcast receivers, activities and services.
- Binds individual components to each other at runtime.
- For activities and services - Intent defines the action to be performed. Eg. View or send something.
- Broadcast receivers - Defines announcement being broadcast.

# Name the four app components and briefly explain them.
- Activity - Entry point for interacting with the user. Eg. A screen with a UI.
- Services - Keeps an app running in the background for all kinds of reasons. Eg. An app that fetches data over the network without blocking user interaction. There are 2 types of services: Started and Bound services.
- Broadcast receivers - Delivers events to the app, outside of a regular user flow. System can deliver broadcasts, even if app is not running. Eg. An app can schedule an alarm to post a notification. The app does not have to be running.
- Content providers - manages a <i>shared set of app data</i> that you can <i>store</i> in the <i>file system</i>, SQLLite, web or persistant location. Eg. The system provides a content provider for managing contact information. Any app with proper permission can access the content provider.

# How can you use the camera app (App A) from another separate app (App B)?
- Instead of developing a camera app, you can use the component of the Android's built-in camera app.
- From App B, you can start the activity from App A.
- When completed, the photo is returned to App B.

# What is the purpose of the AndroidManifest.xml?
- Declares all components.
- <activity> - Elements for activities.
- <service> - Elements for services.
- <receiver> - Elements for broadcast receivers.
- <provider> - Elements for content providers.