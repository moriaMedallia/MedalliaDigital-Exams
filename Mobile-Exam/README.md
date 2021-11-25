# Button to Action app
## Medallia Digital - Mobile exam
### In this exam, you are asked to write the "Button to Action" ReactNative or Flutter

* This app has only 1 button
* Tapping on this button will show an alert
* You can choose how to implement the alert component
* There is a configuration file with list of possible values for the alert data
* The app should calculate which context to show and show it accordinaly


#### Pre Conditions
* Start a new project on your machine
* Read the implementation guidelines section
* Implement :)
* Create a project on Github 
* Send us the repo link when you finish :) 

### Implementation guidelines

#### Guidelines

* Keep in mind that in the future, the app should be able to support more types, other than alert.

- When the user tap the button, one action should be chosen by the actions settigns.

##### Configuration 

Fetch the configuration from the file https://raw.githubusercontent.com/moriaMedallia/MedalliaDigital-Exams/master/Mobile-Exam/actionConfiguration.json 

The way an action is chosen is according to the configuration values retrieved from the configuration json above.
The configuration values:

* id (String)
    * Component id 
* type (String)
    * Describe the compomenent type (Right now only Alert supported)
* enabled (boolean)
    * a disabled action can never be chosen
* title
    * The component should present the title text 
* body
    * The component should present the body text 
* priority (int)
    * if action X has a higher priority than action Y, action X will be selected
    * If two actions have the same priority, choose one at random.
* valid days (days array)
    * valid days to choose the action
    * for example, we can set the “Animation action” action to be choosable only on Monday­Thursday
* cool down period (long) in milliseconds
    * cool down period between choosing an action that was already chosen
    * for example, if an action has a 3 day (1000*60*60*24*3) cool down period, it can’t be chosen for 3 days after it was shown to the user
    * this should persist across app runs
 

### Notes
* Use proper OOP design
* Address edge cases
* When done, send the github link to our email


# Good Luck
