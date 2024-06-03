# PRODIGY_WD_02
Project Description: 🚀
HTML:
Element separation for improved DOM manipulation. 🧩
CSS:
Utilizing box-sizing to include padding, margin, and border in height and width calculations. 📏
Using overflow: hidden to prevent scrolling and overflow to clip container content. 🚫
Responsive design with em, rem, vh, vw units. 📱
flex-wrap for responsive layout, flex-column for vertical alignment. 🌐
Media queries for max-width responsiveness. 🖥️
Animations for dynamic content transitions. 🔄
Additional Details:
box-sizing: border-box; ensures that padding and border are included in the element's total width and height. 📦
overflow: hidden; disables scrolling, and strategic use of overflow is employed to clip content. 🔒
Units like em, rem, vh, and vw are used for automatic responsiveness with width adjustments. 📐
flex-wrap is applied for elements to stack vertically instead of overlapping. 📏
Animations are used for smooth transitions, like animating the displayed time. 🎉
Media queries with max-width are used for responsiveness, setting maximum widths for layout adjustments. 📏
JavaScript:
QuerySelector for accessing HTML elements using class and ID. 🔍
EventListener for constructing events, passing functions without parentheses. 🎤
Functions:
Toggle Start:
Determines whether to start or stop the stopwatch based on the current state (isRunning). ⏯️
Calls the appropriate function accordingly. 📞
Start Stopwatch:
Sets the starttime value. ⏱️
Adjusts the start time if the stopwatch was paused (pausetime is not zero). ⏸️
Calls the updateStopWatchFunction to display and animate the stopwatch. 🔄
Pause Stopwatch:
Sets isRunning to false. ⏸️
Records the pause time (pausetime) as the current time minus the start time. ⏱️
Update Stopwatch:
Calculates the elapsed time by subtracting the start time from the current time. ⏳
Calls the formatTime function to convert the elapsed time into hours, minutes, and seconds. 🕰️
Calls the displayTime function to update the displayed time. 🔄
Initiates an animation for the displayed time. 🎉
Format Time:
Performs mathematical calculations to obtain hours, minutes, and seconds from the given time. 🧮
Ensures the formatted time values are limited to two digits. 🔢
Returns an object containing the formatted time values. 📊
Display Time:
Updates the HTML content for hours, minutes, and seconds with the values received in the object parameter. 📈
Resume Watch:
Sets isRunning to true. ▶️
Adjusts starttime based on the original start time and any pause time. 🔄
Resets pausetime to zero. 🔄
Calls the updateStopWatchFunction to display and animate the resumed stopwatch. 🔄
Reset Stopwatch:
Resets the stopwatch to its initial state. 🔄
Sets isRunning to false, pausetime to zero. ❌
Calls clearLaps to clear lap records. 🔄
Resets lap number to 1. 1️⃣
Updates the displayed time to zero. ⏰
Clear Laps:
Clears lap records by setting the innerHTML of the lap container to an empty string. 🧹
Resets the lap number to 1. 1️⃣
Record Laps:
Checks if the stopwatch is running before creating a lap record. 🏃
Calculates lap time using the formatTime function. ⏱️
Creates a new div element using createElement. 🆕
Applies CSS styling to the div using classList. 🎨
Updates the innerHTML of the div with lap details using template literals. 📝
Appends the div to the lap container using appendChild. ➕
General:
Dynamic use of backticks and ${} for string interpolation. 🔄
Consistent use of camelCase for function and variable names. 🐫
Careful handling of conditional operations based on isRunning state. ⚖️
Strategic use of createElement, classList, and appendChild for dynamic content manipulation. 🛠️
