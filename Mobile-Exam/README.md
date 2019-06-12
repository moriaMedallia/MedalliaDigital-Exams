# Button to Action app
## Medallia Digital - Mobile exam
### In this exam, you are asked to write the "Button to Action" Android or iOS app.

* This app has only 1 button
* Tapping on this button performs one of the [actions](#actions) below
* Each tap on the button will trigger a random action


#### Pre Conditions
* Start a new project on your machine
* Read the implementation guidelines section
* Implement :)
* Create a project on Github 
* Send us the repo link when you finish :) 

### Implementation guidelines
#### Actions
The app should support the following actions:
1. Alert
2. Screen
3. Action Sheet

#### Guidelines

* Keep in mind that in the future, the app should be able to support actions that are more complex than the actions above.

- When the user tap the button, one action should be chosen by the actions settigns.

##### Configuration 

Fetch the configuration from:
https://raw.githubusercontent.com/medallia-digital/Exams-Data/master/mobileData.json

The way an action is chosen is according to the configuration values retrieved from the configuration json above.
The configuration values:

* id (String)
    * Component id 
* type (String)
    * Describe the compomenent type (Alert, Screen,BottomSheet)
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
* cool down period (long)
    * cool down period between choosing an action that was already chosen
    * for example, if an action has a 3 day (1000*60*60*24*3) cool down period, it can’t be chosen for 3 days after it was shown to the user
    * this should persist across app runs

#### Componenets 
1. Alert - 
    * Android - AlertDialog 
    * iOS - UIAlertController
2. Screen - 
    * Android - Activity 
    * iOS - UIViewController
3. Action Sheet - 
    * Android - BottomSheetDialog
    * iOS - UIActionSheet
 

### Notes
* Use proper OOP design
* Address edge cases
* When done, send the github link to our email


# Good Luck
