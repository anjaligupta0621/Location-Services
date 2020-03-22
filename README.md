# Location-Services

#### Implemented Option A of the Assessment

Application is written in Swift.
Backend Service is written in NodeJS hosted on Heroku with the Cloud Database Service mLAB for MongoDB

Write an iOS or Android location services app that returns a location based on geolocation. - **Used CLLocationManager in Swift to Fetch Current geolocation coordinates of the Mobile**

Record location in a NoSQL database such as Mongo. - **Each Get Location Tap makes a POST Request on the api to store the results in our cloud hosted Database in mLAB(MongoDB)**

Create a screen to query location history - **A Dropdown menu on the home screen to check the location history(https://location-history-server.herokuapp.com/location), choosing the timestamp will location the marker instantly on the google map**

Write a Rest API that implements a micro service to return location history. - **API endpoint - https://location-history-server.herokuapp.com/location**


The API must support at least two filters such as date range or last N locations - **API has two Different End point for applying the filter and fetch filtered results, Data Range(https://location-history-server.herokuapp.com/location/date/<start_date>/<end_date>) and Limit result to last 5 Locations visited(https://location-history-server.herokuapp.com/location/limit/5)**


Map location on a google map. Search is triggered by a button (Get Location). - **Google Maps SDK is used to Show the location chosen at all Times, User can Tap the Get Location Button to Fetch Current Location, which will simultaneously also added to Location History via API call.**


Share location with your friends list - **Implemented using uiactivityviewcontroller, user can share current location to his friends via the social apps installed or even normal message**


| Main Screen  | Date Range | Share Location |
| ------------- | ------------- | ------------- |
| ![alt text](https://github.com/anshulkapoor018/Location-Services/blob/master/Screenshots/Main%20Screen.png)  | ![alt text](https://github.com/anshulkapoor018/Location-Services/blob/master/Screenshots/Date%20Range.png)  | ![alt text](https://github.com/anshulkapoor018/Location-Services/blob/master/Screenshots/Share%20Location.png)  |


#### Configure the Team for each target within the project.

    1.Open the project in the Project navigator within Xcode and select each of the targets. Set the Team on the General tab to the team associated with your developer account.

    2.Change the Bundle Identifier.
        * With the project's General tab still open, update the Bundle Identifier value. The project's Lister target ships with the value: com.example.<Insert_Name_here>.Location-Services
        * You should modify the reverse DNS portion to match the format that you use:
            -> com.anshulkapoor018.Location-Services <This needs to be edited>
    3.Install Supporting Libraries
        * First, make sure you have Cocoapods installed. If not, Run the command below
            -> `sudo gem install cocoapods`
        * Second, navigate to ../Location-Services/Location Services Folder via Terminal and Run the Below command
            -> `pod install`

##### Open the Project workspace File(_Location Services.xcworkspace_) for Testing the Application

This application is written in Swift.
Location-Services design and controller interactions are implemented in a Storyboard. A storyboard makes it easy to visualize the relationships between view controllers and to lay out the user interface of the app. Location-Services also takes advantage of Auto Layout to fluidly resize the interface as the user resizes the window. If you're opening the project for the first time, the Main.storyboard file is a good place to understand how the app works.
