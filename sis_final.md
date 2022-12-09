
# Overview

The purpose of the Software Requirement Specification is to define assumptions and requirements for the product. The goal is to provide a high level of understanding of the System "The Cook Book", a modern recipe-sharing website, which aims to provide users with a variety of food recipes and be the starting point of development. 

# Software Requirements

This section provides a comprehensive understanding of the system’s underlying features and functionalities i.e what the system can do and the non-functional requirements which gives an insight into the system behavior and ensures the usability and effectiveness of the system. As it provides a high level of understanding of the application it is useful for developers to implement the system, testers to test the functionality, and end users and admins who would be using the application.

## Functional Requirements

### Sign Up
| ID | Requirement |
| -------------| ---------- |
| FR1 | The system shall provide an user, with a signup option that opens a signup form. |
| FR2 | The system shall register the new user when the user fills out the signup form with valid details. |
| FR3 | The system shall validate the user does not use an invalid or existing email address. |
| FR4 | The system shall validate the user a secured password meeting standard secured password criteria. |
| FR5 | The system shall display appropriate validation messages when the user enters invalid data. |
| FR6 | The system shall display a welcome message to the user after successful signup. |
| FR7 | The system shall redirect the new user to the home screen after successful signup. |
| FR8 | The system shall allow the user to cancel the signup. |

### Log In
| ID | Requirement |
| -------------| ---------- |
| FR9 | The system shall allow an user to enter his username and password on the login screen of the website. |
| FR10 | The system shall validate the email input fields and display the appropriate validation message. |
| FR11 | The system shall verify user login data entered on the login screen of the website. |
| FR12 | The system shall display appropriate error messages if an user enters an invalid username or password. |
| FR13 | The system shall allow an user to reset his password by clicking on forgot password. |
| FR14 | The system shall allow the user to provide their registered email for password recovery. |
| FR15 | The system shall redirect the signed-in user to the home screen after successful login. |

### Manage Account
| ID | Requirement |
| -------------| ---------- |
| FR16 | The system shall allow the registered user to update their personal information except for email. |
| FR17 | The system shall allow the user to upload a new/change an existing profile picture. |
| FR18 | The system shall allow the registered user to change the password. |
| FR19 | The system shall prompt the user for the existing password along with the new password when changing the password. |
| FR20 | The system shall validate the new password as per the secured password criteria. |
| FR21 | The system shall persist the new updated information in the database for the signed-in user. |


### Search and View Recipe
| ID | Requirement |
| -------------|---------- |
| FR22 | The system shall allow any user to search and view recipe(s). |
| FR23 | The system shall allow an user to search for recipes by name. |
| FR24 | The system shall allow an user to search for recipes based on ingredients. |
| FR25 | The system shall use pagination to fetch the recipe list. |
| FR26 | The system shall allow an user to select a recipe from the search list result. |
| FR27 | The system shall allow an user to view the recipe selected.|

### Upload a Recipe
| ID | Requirement |
| -------------| ---------- | 
| FR28 | The system shall allow only logged-in users to upload recipes. |
| FR29 | The system shall allow a logged-in user to upload one recipe at a time. |
| FR30 | The system shall provide a form to upload the recipe details. |
| FR31 | The system shall allow a logged-in user to attach an image to the recipe being uploaded. |
| FR32 | The system shall validate the upload recipe form data and display the appropriate validation message. |
| FR33 | The system shall persist the uploaded recipe in the database after successful validation. |
| FR34 | The system shall close the upload recipe form and redirect the logged-in user to the home screen after upload. |

### Add a Review Comment
| ID | Requirement |
| -------------| ---------- | 
| FR35 | The system shall allow the logged-in user to add one or more review comments on a recipe. |
| FR36 | The system shall persist the comment added in the database. |
| FR37 | The system shall allow the logged-in user to view all review comments on a recipe. |
| FR38 | The system shall allow the logged-in user to edit their review comment. |
| FR39 | The system shall allow the logged-in user to delete their review comment. |
| FR40 | The system shall update/delete the review comment in the database based on the user's action. |

### Like a Recipe
| ID | Requirement |
| -------------| ---------- | 
| FR41 | The system shall display the count of total likes on a given recipe. |
| FR42 | The system shall allow a logged-in user to like a recipe. |
| FR43 | The system shall persist the like action by a logged-in user for a recipe in the database. |
| FR44 | The system shall allow a logged-in user to, unlike a recipe. |
| FR45 | The system shall delete the like record for the logged-in user for the recipe in the database. |
| FR46 | he system shall refresh the total like count on the screen when a like or unlike action is performed by the logged-in user. |

### Log Out
| ID | Requirement |
| -------------| ---------- | 
| FR47 | The system shall allow the logged-in user to log out. |
| FR48 | The system shall redirect to the home page after the registered user logs out successfully. |

    
## Non-Functional Requirements
### Performance:
| ID | Requirement |
| -------------| ---------- |
| NFR1 | Application shall handle maximum number of 30K users at a time.|
| NFR2 | Performace of the application shall be monitored using AWS cloudwatch.|
| NFR3 | After clicking onto reset password button temporary password shall be sent with a latency of no greater than 1 hour.|
| NFR4 | Each login and registration request shall be processed in maximum of 10 seconds.|
| NFR5 | Application shall take no longer than 3 seconds to load when user tries to open it.|
| NFR6 | All the drawer navigation shall load their respective screens in less 3 seconds.|

### Availability:
| ID | Requirement |
| -------------| ---------- |
| NFR7 | Application shall be up and running 24*7 all the days.|
| NFR8 | Recent or only upcoming posts shall be available for avoiding storage of large data on database.|
| NFR9 | Customer support shall be provided if user faces any issue accessing the application.|
| NFR10 | Temporary password sent to user shall be valid for 4 hours for successful login.|
| NFR11 | After successful login, users email address shall be stored in AsyncStorage.|

### Usability:
| ID | Requirement |
| -------------| ---------- |
| NFR12 | Each application UI screen shall be user friendly and in easily understanble format or readable formate.|
| NFR13 | The user shall experience an aesthetic and minimal design.|
| NFR14 | The application shall consist of standard visual experience for all users.|
| NFR15 | The ride booking shall follow first in first out method.|
| NFR16 | User from any age group shall access app easily.|

### Operational Requirement:
| ID | Requirement |
| -------------| ---------- |
| NFR17 | Application shall be installed or run on both operating systems - Android and iOS.|
| NFR18 |The system front end UI shall be created using react-native.|
| NFR19 | System shall be build using expo CLI.|
| NFR20 | The backend logic shall be implemented using python flask framework.|
| NFR21 | Application shall run on device regardless of OS update or on switching mobile with new operating system.|
| NFR22 | Application shall store all of its users and posts/comments data in NoSQL format in DynamicDB of AWS.|
| NFR23 | Google maps shall be used for entering accurate location while posting a ride detail.|
| NFR24 | CI/CD pipeline shall be used to make application  available by testing and deploying latest updates.|
### Security:
| ID | Requirement |
| -------------| ---------- |
| NFR25 | Customer's personal data shall be stored in database in encrypted format.
| NFR26 | Unsuccessful login of user shall be recorded and audited.
| NFR27 | User data shall not be shared with any other party.|
| NFR28 | No user shall have access to delete any post unless they have created that post.|
| NFR29 | The source coding shall follow secure coding practices.|

# Change Management Plan:

This section will describe a change management plan for ShareRide application. It will focus on training users, platform availability, performance and issue handling process.


## Why Shareride App?
ShareRide is a cross-platform mobile application for Grand Valley State
University, where all students and faculty members can join and share rides. Any
member of our application can ask for a ride by simply posting a plan, and whichever
member who has a vehicle can pick up the member who asked for a ride. Alternatively,
any member who already owns a vehicle can post his/her plan to visit somewhere, and
whoever fits the schedule can join the trip in first-come-first-serve basis.
## Training Strategy:
We will train people/students by proposing this system to the students during
Students orientation which happens at the start of every new semester and help them
login to the platform using their GVSU email. Like Uber, the first ride will have some
offers. The information about the application will be promoted in the form of posters all
over the campus where the QR code of the app will be provided in the posters.
## Integration within GVSU ecosystem:
The ShareRide application will be integrated on myBanner website, a GVSU
official portal. Since the application is designed for GVSU’s students, it would be
available to them on their official website. Students can get to know about the application
and download the application with the QR code in myBanner.
## Performance Issue and Monitoring:
We will continuously monitor the application’s performance and fix bugs. The application follows CI/CD pipeline, deployed on AWS CodePipeline which tests the code
before deploying.
## Availability of the Mobile Application:
The application will be available in both commanly used operating system - Android and iOS.

# Traceability links
This section represents relationship between requirements and other project artifacts such as class diagram, Use case diagram and activity diagram.
## Use Case Diagram Traceability
| Artifact ID | Artifact Name | Requirement ID |
| :-------------: | :----------: | :----------: |
|1| [Sign In/Login](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Use_Case_SignIn.pdf) | FR1, FR3, FR6, FR26|
|2| [Sign Up/Registration](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Use_Case_Email_Verification_Registration.pdf) | FR7-11|
|3|[Edit Profile](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Use_Case_Edit_Profile.pdf)| FR12-14, FR16|
|4| [Post/Comment](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Use_Case_Post_Comment_Details.pdf)| FR18-21, FR25|
## Class Diagram Traceability
| Artifact Name | Requirement ID |
| :-------------: |:----------: |
| [User](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/ClassDiagram.pdf) | FR1, FR2, FR7, FR8, FR12-FR14 |
| [Vehicle](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/ClassDiagram.pdf) | FR8 |
| [RideDetails](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/ClassDiagram.pdf) | FR18, FR20,21 |
| [Post/Comment](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/ClassDiagram.pdf) | FR17-23 |



## Activity Diagram Traceability
| Artifact ID | Artifact Name | Requirement ID |
| :-------------: | :----------: | :----------: |
| [5](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Activity_Diagram_Login.pdf) | Login | FR1-5, NFR2, NFR26 |
|[6](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Activity_Diagram_Edit_Profile.pdf)|Edit Profile | FR12-16, NFR25, |
|[7](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Activity_Diagram_Sign_In.pdf)|  SignIn | FR2-5, FR8-11, NFR1, NFR3,NFR4, NFR7, NFR10, NFR12, NFR17, NFR16 |


# Software Artifacts
 [1 - Sign In/Login UseCase](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Use_Case_SignIn.pdf)

 [2 -  Sign Up/Registration UseCase](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Use_Case_Email_Verification_Registration.pdf)

[3 - Edit Profile UseCase](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Use_Case_Edit_Profile.pdf)

[4 - Post/Comment UseCase](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Use_Case_Post_Comment_Details.pdf)

 [5 -  Login Activity](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Activity_Diagram_Login.pdf)

 [6 -  Edit Profile Activity](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Activity_Diagram_Edit_Profile.pdf)

[7 -  SignIn Activity](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Activity_Diagram_Sign_In.pdf)

[8 - Behavioral Diagram](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/Behavioral_Diagram_Sequence_StateMachine.pdf)

[9 - Combined Class Diagram](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/ClassDiagram.pdf)

[10 - Combined Use Case and Activity Diagram](https://github.com/Purva8852/GVSU-CIS641-Team-S/blob/master/artifacts/functional-models/UseCasesAndADs.pdf)
