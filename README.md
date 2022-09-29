# FB11615066

UIMenuBuilder does not show key commands on app launch
----

- Product: UIKit
- Classification: Incorrect/Unexpected Behaviour
- Status: Open
- Product Version: 16.0
- Date Originated: 2022-09-29

----

On iPadOS 15.5 and above, building with the iOS 16 SDK, the app does not immediately show the key commands setup by the app from `func buildMenu(with builder: UIMenuBuilder)` from its `AppDelegate`. 

After interacting with any view in the app that can become a first responder, the app immediately begins to display key commands setup by it. 

The app instead presents key commands from Springboard (Homescreen). 

Apps built with prior versions of the SDK (15.5) exhibit the correct behaviour. 

Sample code and screenshot attached (https://github.com/dezinezync/FB11615066)

Xcode Version: 14.0.1 (14A400)

