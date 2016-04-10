# basil-front-end
This is a Python Flask application. It displays a recipe on screen.
The front-end is linked with Alexa. Users can speak voice commands like
"Alexa, tell Basil to move to the next step" to read the recipe instructions.

Technology flow:
 - The page is rendered using HTML/CSS/Javascript. The only front-end framework used is jQuery.
 - Users speak commands into Amazon Echo.
 - We built an Alexa Skill to understand commands related to this app.
 - When the skill is invoked, an Amazon Lambda java function is called.
 - The Amazon Lambda function updates data in Firebase as needed.
 - Changes the Firebase DB then synchronizes to the web page, which updates the screen.

The back-end Lambda application and skills files are in https://github.com/Team-Basil/basil.
