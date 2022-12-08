# Overview

The purpose of the Software Requirement Specification is to define assumptions and requirements for the product. The goal is to provide a high level of understanding of the System "The Cook Book", a modern recipe-sharing website, which aims to provide users with a variety of food recipes and be the starting point of development. 

# Software Requirements

This section provides a comprehensive understanding of the system’s underlying features and functionalities i.e what the system can do and the non-functional requirements which gives an insight into the system behavior and ensures the usability and effectiveness of the system. As it provides a high level of understanding of the application it is useful for developers to implement the system, testers to test the functionality, and end users and admins who would be using the application.

## Functional Requirements
<ol type="1">
    <li> Sign Up
        <ul type="1">
            <li>FR1: The system shall register the new user when the user fills out the sign-up form provided with a valid unique
                email address.</li>
            <li>FR2: The system shall validate the data entered by the user while filling out the form.</li>
            <li>FR3: The system shall display appropriate error messages if a user enters invalid data while filling out the form.</li>
            <li>FR4: The system shall display appropriate messages after successful signup.</li>
            <li>FR5: The system shall redirect the end user to the login screen after successful signup.</li>
        </ul>
    </li>
    <li> Log In
        <ul type="1">
            <li>FR6: The system shall allow the end user to enter his username and password on the login screen of the website.</li>
            <li>FR7: The system shall validate user login data entered on the login screen of the website.</li>
            <li>FR8: The system shall display appropriate error messages if a user enters an invalid username or password.</li>
            <li>FR9: The system shall allow a user to reset his password by clicking on forgot password.</li>
            <li>FR10: The system shall redirect the end user to the home screen after successful login.</li>
        </ul>
    </li>
    <li> Manage Account
        <ul type="1">
            <li>FR11: The system shall allow the registered user to update their personal information.</li>
            <li>FR12: The system shall update the updated information of the registered user in the database.</li>
            <li>FR13: The system shall allow the registered user to change and update the current password.</li>
            <li>FR14: The system shall update the updated password of the registered user in the database.</li>  
            <li>FR15: The system shall allow the registered user to upload a profile image to the account.</li> 
            <li>FR16: The system shall insert the profile image uploaded by the registered user in the database.</li>  
        </ul>
    </li>
    <li> Search Recipe
        <ul type="1">
            <li>FR17: The system shall allow the registered user to search for recipes.</li>
            <li>FR18: the system shall allow the registered user to add filters to the search.</li>
            <li>FR19: The system shall allow the registered user to search for recipes based on the number of likes on recipes.</li>
            <li>FR20: The system shall fetch limited data per page.</li>
            <li>FR21: The system shall allow the registered user to select a recipe from the search list result.</li>
        </ul>
    </li>
    <li> View Recipe
        <ul type="1">
            <li>FR22: The system shall allow the registered user to view the recipe selected.</li>
            <li>FR23: The system shall allow the registered user to save a recipe selected for future reference.</li>
            <li>FR24: The system shall allow the registered user to view the list of saved recipes.</li>
            <li>FR25: The system shall allow the registered user to select a recipe from the saved list of recipes.</li>
            <li>FR26: The system shall allow the registered user to remove a recipe from the saved list of recipes.</li>
        </ul>
    </li>
    <li> Upload a Recipe
        <ul type="1">
            <li>FR27: The system shall allow the registered user to upload a recipe.</li>
            <li>FR28: The system shall allow the registered user to upload an image of the recipe being uploaded.</li>
            <li>FR29: The system shall allow the registered user to add the recipe instructions of the recipe being uploaded.</li>
            <li>FR30: The system shall validate the data entered by the user while uploading the recipe.</li>
            <li>FR31: The system shall display appropriate error messages if the user tries to upload an existing recipe.</li>
            <li>FR32: The system shall insert the recipe uploaded by the registered user in the database.</li>
        </ul>
    </li>
    <li> Add a Review Comment
        <ul type="1">
            <li>FR33: The system shall allow the registered user to add a review comment on a recipe.</li>
            <li>FR34: The system shall insert the comment added by the registered user in the database.</li>
            <li>FR35: The system shall allow the registered user to view the review published.</li>
            <li>FR36: The system shall allow the registered user to view other users' review comments on a recipe.</li>
            <li>FR37: The system shall allow the registered user to update a review comment added by him or her on a recipe.</li>
            <li>FR38: The system shall update the comment updated by the registered user in the database.</li>
        </ul>
    </li>
    <li> Like a Recipe
        <ul type="1">
            <li>FR39: The system shall allow the registered user to hit like on a recipe.</li>
            <li>FR40: The system shall insert the like added by the registered user in the database.</li>
            <li>FR41: The system shall allow the registered user to remove like on a recipe already liked by him or her.</li>
            <li>FR42: The system shall update the likes removed by the registered user in the database.</li>
            <li>FR43: The system shall allow the registered user to view the total number of likes on a recipe.</li>
        </ul>
    </li>
    <li> Log Out
        <ul type="1">
            <li>FR44: The system shall allow the logged-in registered user to log out.</li>
            <li>FR45: The system shall redirect to the login page after the user logs out successfully.</li>
        </ul>
    </li>
</ol>

## Non-Functional Requirements
<ol type="2">
    <li> Availability
        <ul type="1">
            <li>NFR1: The system should have an availability of 99.99999 percent.</li>
            <li>NFR2: The system should be supported and be available 99.99999 percent by all types of Web Browsers.</li>
            <li>NFR3: The system should have an availability of 99.99999 percent for new user sign-up.</li>
            <li>NFR4: The system should have an availability of 99.99999 percent for registered user login.</li>
            <li>NFR5: The system should have an availability of 99.99999 percentfor the registered user to upload a recipe.</li>
        </ul>
    </li>
    <li> Accessibility
        <ul type="1">
            <li>NFR6: The system shall be rendered on screen in less than 1 second.</li>
            <li>NFR7: The system should enable the users to search for a recipe in less than 2 seconds.</li>
            <li>NFR8: The system should enable the users to publish a comment for a recipe in less than 2 seconds.</li>
            <li>NFR9: The system should enable the users to upload a recipe in less than 5 seconds.</li>
            <li>NFR10: The system should enable the users to like a recipe in less than 2 seconds.</li>
            <li>NFR11: The system when Restarted, should not take more than 30 seconds to go back to live.</li>
        </ul>
    </li>
    <li> Security
        <ul type="1">
            <li>NFR12: The system should not allow users to see the personal identifiable information (PII) of other users.</li>
            <li>NFR13: The system should not allow non-registered users to see the data.</li>
            <li>NFR14: The system shouldn’t allow a  non-registered user to upload the recipe. A such attempt should be reported to the administrator.     </li>
            <li>NFR15: The system should not allow users to access the database. Only the administrator would have the access to the database.</li>
            <li>NFR16: The system shall maintain data integrity by keeping backups of all updates to the database for every record transaction.<li>
        </ul>
    </li>
    <li> Reliability
        <ul type="1">
            <li>NFR17:The system should enable maintaining services with 0 downtimes.</li>
            <li>NFR18: The system should be able to scale up and scale down based on the load on the website.</li>
            <li>NFR19: The system should pass all the test cases(for that feature) at any point of development.</li>
            <li>NFR20: The system should be able to perform the same when the simultaneous users are at least < 500.</li>
            <li>NFR21: The system should allow the registered user to access and perform any updates on his or her profile 99.99999 percent of the time without failure.</li>
        </ul>
    </li>
    <li> Usability
        <ul type="1">
            <li>NFR22: The system should be user-friendly and easy to use for a non-technical person.</li>
            <li>NFR23: The error rate of users submitting the sign-up form on the system should be less than 10 percent.</li>
        </ul>
    </li>
    <li> Tracking Activities
        <ul type="1">
            <li>NFR24: The system should log the action done on the database.</li>
        </ul>
    </li>
    <li> Structuring
        <ul type="1">
            <li>NFR25: The system should follow the folder structure decided by the technical architecture for further adding any feature.</li>
        </ul>
    </li>
</ol>

# Change Management Plan

A change management plan is a document used to offer a detailed, step-by-step strategy for adopting change. The purpose of the change management plan is to help manage the change process and also ensure control of the budget, schedule, scope, communication, and resources. The change management plan will minimize the impact a change can have on the application and the stakeholders involved thus reducing the risk and resistance while improving communication and long-term adoption of the new system or process.
