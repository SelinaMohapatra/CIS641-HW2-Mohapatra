# Overview

The purpose of the Software Requirement Specification is to define assumptions and requirements for the product. The goal is to provide a high level of understanding of the System "The Cook Book", a modern recipe-sharing website, which aims to provide users with a variety of food recipes and be the starting point of development. 

# Software Requirements

This section provides a comprehensive understanding of the system’s underlying features and functionalities i.e what the system can do and the non-functional requirements which gives an insight into the system behavior and ensures the usability and effectiveness of the system. As it provides a high level of understanding of the application it is useful for developers to implement the system, testers to test the functionality, and end users and admins who would be using the application.

## Functional Requirements
<ol type="1">
    <li> Sign Up
        <ul type="1">
            <li>FR1: The system shall provide an user, with a signup option that opens a signup form.</li>
            <li>FR2: The system shall register the new user when the user fills out the signup form with valid details.</li>
            <li>FR3: The system shall validate the user does not use an invalid or existing email address.</li>
            <li>FR4: The system shall validate the user a secured password meeting standard secured password criteria.</li>
            <li>FR5: The system shall display appropriate validation messages when the user enters invalid data.</li>
            <li>FR6: The system shall display a welcome message to the user after successful signup.</li>
            <li>FR7: The system shall redirect the new user to the home screen after successful signup.</li>
            <li>FR8: The system shall allow the user to cancel the signup.</li>
        </ul>
    </li>
    <li> Log In
        <ul type="1">
            <li>FR9: The system shall allow an user to enter his username and password on the login screen of the website.</li>
            <li>FR10: The system shall validate the email input fields and display the appropriate validation message.</li>
            <li>FR11: The system shall verify user login data entered on the login screen of the website.</li>
            <li>FR12: The system shall display appropriate error messages if an user enters an invalid username or password.</li>
            <li>FR13: The system shall allow an user to reset his password by clicking on forgot password.</li>
            <li>FR14: The system shall allow the user to provide their registered email for password recovery.</li>
            <li>FR15: The system shall redirect the signed-in user to the home screen after successful login.</li>
        </ul>
    </li>
    <li> Manage Account
        <ul type="1">
            <li>FR16: The system shall allow the registered user to update their personal information except for email.</li>
            <li>FR17: The system shall allow the user to upload a new/change an existing profile picture.</li>
            <li>FR18: The system shall allow the registered user to change the password.</li>
            <li>FR19: The system shall prompt the user for the existing password along with the new password when changing the password.</li>
            <li>FR20: The system shall validate the new password as per the secured password criteria.</li>
            <li>FR21: The system shall persist the new updated information in the database for the signed-in user.</li>
        </ul>
    </li>
    <li> Search and View Recipe
        <ul type="1">
            <li>FR22: The system shall allow any user to search and view recipe(s).</li>
            <li>FR23: The system shall allow an user to search for recipes by name.</li>
            <li>FR24: the system shall allow an user to search for recipes based on ingredients.</li>
            <li>FR25: The system shall use pagination to fetch the recipe list.</li>
            <li>FR26: The system shall allow an user to select a recipe from the search list result.</li>
            <li>FR27: The system shall allow an user to view the recipe selected.</li>
        </ul>
    </li>
    <li> Upload a Recipe
        <ul type="1">
            <li>FR28: The system shall allow only logged-in users to upload recipes.</li>
            <li>FR29: The system shall allow a logged-in user to upload one recipe at a time.</li>
            <li>FR30: The system shall provide a form to upload the recipe details.</li>
            <li>FR31: The system shall allow a logged-in user to attach an image to the recipe being uploaded.</li>
            <li>FR32: The system shall validate the upload recipe form data and display the appropriate validation message.</li>
            <li>FR33: The system shall persist the uploaded recipe in the database after successful validation.</li>
            <li>FR34: The system shall close the upload recipe form and redirect the logged-in user to the upload screen after upload.</li>
        </ul>
    </li>
    <li> Add a Review Comment
        <ul type="1">
            <li>FR35: The system shall allow the logged-in user to add one or more review comments on a recipe.</li>
            <li>FR36: The system shall persist the comment added in the database.</li>
            <li>FR37: The system shall allow the logged-in user to view all review comments on a recipe.</li>
            <li>FR38: The system shall allow the logged-in user to edit their review comment.</li>
            <li>FR39: The system shall allow the logged-in user to delete their review comment.</li>
            <li>FR40: The system shall update/delete the review comment in the database based on the user's action.</li>
        </ul>
    </li>
    <li> Like a Recipe
        <ul type="1">
            <li>FR41: The system shall display the count of total likes on a given recipe.</li>
            <li>FR42: The system shall allow a logged-in user to like a recipe.</li>
            <li>FR43: The system shall persist the like action by a logged-in user for a recipe in the database.</li>
            <li>FR44: The system shall allow a logged-in user to, unlike a recipe.</li>
            <li>FR45: The system shall delete the like record for the logged-in user for the recipe in the database.</li>
            <li>FR46: The system shall refresh the total like count on the screen when a like or unlike action is performed by the logged-in user.</li>
        </ul>
    </li>
    <li> Log Out
        <ul type="1">
            <li>FR47: The system shall allow the logged-in user to log out.</li>
            <li>FR48: The system shall redirect to the home page after the registered user logs out successfully.</li>
        </ul>
    </li>
</ol>

## Non-Functional Requirements
<ol type="2">
    
    Reliability
        Availability
        Fault Tolerance
        Recoverability
    
    Security
    
    <li> Availability and Reliability
        <ul type="1">
            <li>NFR1: The system should have an availability of 99.999%.</li>
            <li>NFR1: The system should have a failover server in case of failure.</li>
            <li>NFR1: The system shall take database backups every 3 hours to allow recovery.</li>
            <li>NFR1: The system shall support a recovery time objective of 3 hours.</li>
        </ul>
    </li>
    <li> Accessibility
        <ul type="1">
            <li>NFR6: The system shall be rendered on screen in less than 1 second.</li>
            <li>NFR7: The system should retrieve the recipes in less than 2 seconds on screen.</li>
            <li>NFR8: The system should persist/update/delete a comment for a recipe in less than 0.5 seconds.</li>
            <li>NFR9: The system should persist an uploaded recipe in less than 1 second.</li>
            <li>NFR10: The system should update the like count in less than 2 seconds on like/unlike action.</li>
            <li>NFR11: The system should be supported by major web browsers.</li>
        </ul>
    </li>
    <li> Security
        <ul type="1">
            <li>NFR12: The system should not allow users to see the personal identifiable information (PII) of other users.</li>
            <li>NFR13: The system should not allow non-logged-in users to upload recipes.</li>
            <li>NFR13: The system should not allow non-logged-in users to add/update/delete review comments on a recipe.</li>
            <li>NFR13: The system .</li>
            <li>NFR15: The system should not allow users to access the database. Only the administrator would have the access to the database.</li>
            <li>NFR16: The system shall maintain data integrity by keeping backups of all updates to the database for every record transaction.</li>
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
