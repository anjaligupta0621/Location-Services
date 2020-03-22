# Location-Services

iOS Application Backed by a NodeJS Server Hosted on Heroku with the Cloud Database Service mLAB for MongoDB

Configure the Team for each target within the project.

Open the project in the Project navigator within Xcode and select each of the targets. Set the Team on the General tab to the team associated with your developer account.

Change the Bundle Identifier.
With the project's General tab still open, update the Bundle Identifier value. The project's Lister target ships with the value:

com.example.<Insert_Name_here>.Location-Services

You should modify the reverse DNS portion to match the format that you use:

com.anshulkapoor018.Location-Services <This needs to be edited>

Written in Swift
This application is written in Swift.
Location-Services design and controller interactions are implemented in a Storyboard. A storyboard makes it easy to visualize the relationships between view controllers and to lay out the user interface of the app. Location-Services also takes advantage of Auto Layout to fluidly resize the interface as the user resizes the window. If you're opening the project for the first time, the Main.storyboard file is a good place to understand how the app works.
