# Overview

The purpose of the Software Requirement Specification is to define assumptions and requirements for the product. The goal is to provide a high level of understanding of the System "The Cook Book", a modern recipe-sharing website, which aims to provide users with a variety of food recipes and be the starting point of development. This document provides a comprehensive understanding of the system’s underlying features and functionalities i.e what the system can do and the non-functional requirements which gives an insight into the system behavior and ensures the usability and effectiveness of the system. 

# Functional Requirements
<ol type="1">
    <li> Sign Up
        <ol type="1">
            <li>The system shall register the new user when the user fills out the sign-up form provided with a valid unique
                email address.</li>
            <li>The system shall validate the data entered by the user while filling out the form.</li>
            <li>The system shall display appropriate error messages if a user enters invalid data while filling out the form.</li>
            <li>The system shall display appropriate messages after successful signup.</li>
            <li>The system shall redirect the end user to the login screen after successful signup.</li>
        </ol>
    </li>
    <li> Log In
        <ol type="1">
            <li>The system shall allow the end user to enter his username and password on the login screen of the website.</li>
            <li>The system shall validate user login data entered on the login screen of the website.</li>
            <li>The system shall display appropriate error messages if a user enters an invalid username or password.</li>
            <li>The system shall allow a user to reset his password by clicking on forgot password.</li>
            <li>The system shall redirect the end user to the home screen after successful login.</li>
        </ol>
    </li>
    <li> Manage Account
        <ol type="1">
            <li>The system shall allow the registered user to update their personal information.</li>
            <li>The system shall update the updated information of the registered user in the database.</li>
            <li>The system shall allow the registered user to change and update the current password.</li>
            <li>The system shall update the updated password of the registered user in the database.</li>  
            <li>The system shall allow the registered user to upload a profile image to the account.</li> 
            <li>The system shall insert the profile image uploaded by the registered user in the database.</li>  
        </ol>
    </li>
    <li> Search Recipe
        <ol type="1">
            <li>The system shall allow the registered user to search for recipes.</li>
            <li>The system shall allow the registered user to add filters to the search.</li>
            <li>The system shall allow the registered user to search for recipes based on the number of likes on recipes.</li>
            <li>The system shall fetch limited data per page.</li>
            <li>The system shall allow the registered user to select a recipe from the search list result.</li>
        </ol>
    </li>
    <li> View Recipe
        <ol type="1">
            <li>The system shall allow the registered user to view the recipe selected.</li>
        </ol>
    </li>
    <li> Upload a Recipe
        <ol type="1">
            <li>The system shall allow the registered user to upload a recipe.</li>
            <li>The system shall allow the registered user to upload an image of the recipe being uploaded.</li>
            <li>The system shall allow the registered user to add the recipe instructions of the recipe being uploaded.</li>
            <li>The system shall validate the data entered by the user while uploading the recipe</li>
            <li>The system shall display appropriate error messages if the user tries to upload an existing recipe.</li>
            <li>The system shall insert the recipe uploaded by the registered user in the database.</li>
        </ol>
    </li>
    <li> Add a Review Comment
        <ol type="1">
            <li>The system shall allow the registered user to add a review comment on a recipe.</li>
            <li>The system shall insert the comment added by the registered user in the database.</li>
            <li>The system shall allow the registered user to view the review published.</li>
            <li>The system shall allow the registered user to view other users' review comments on a recipe.</li>
            <li>The system shall allow the registered user to update a review comment added by him or her on a recipe.</li>
            <li>The system shall update the comment updated by the registered user in the database.</li>
        </ol>
    </li>
    <li> Like a Recipe
        <ol type="1">
            <li>The system shall allow the registered user to hit like on a recipe.</li>
            <li>The system shall insert the like added by the registered user in the database.</li>
            <li>The system shall allow the registered user to remove like on a recipe already liked by him or her.</li>
            <li>The system shall update the likes removed by the registered user in the database.</li>
            <li>The system shall allow the registered user to view the total number of likes on a recipe.</li>
        </ol>
    </li>
    <li> Log Out
        <ol type="1">
            <li>The system shall allow the logged-in registered user to log out.</li>
            <li>The system shall redirect to the login page after the user logs out successfully.</li>
        </ol>
    </li>
</ol>

# Non-Functional Requirements
<ol type="2">
    <li> Availability
        <ol type="1">
            <li> The system should have an availability of 99.99999%.</li>
        </ol>
    </li>
    <li> Accessibility
        <ol type="1">
            <li>The system shall be rendered on screen in less than 2 seconds.</li>
            <li>The system should enable the users to Comment on a recipe in less than 10 seconds.</li>
            <li>The system should enable the users to search for a recipe in less than 10 seconds.</li>
            <li>The System when Restarted, should not take more than 30 seconds to go back to live.</li>
        </ol>
    </li>
     <li> Compatability
        <ol type="1">
            <li>The System should be supported by all types of Web Browsers.</li>
        </ol>
    </li>
    <li> Restricting Users
        <ol type="1">
            <li>The system should not allow users to see the personal identifiable information (PII) of other users.</li>
            <li>The system should not allow non-registered users to see the data.</li>
            <li>The system shouldn’t allow a  non-registered user to upload the recipe. A such attempt should be reported to the administrator.</li>
        </ol>
    </li>
    <li> Reliability
        <ol type="1">
            <li>The system should enable maintaining services with 0 downtimes.</li>
            <li>The system should be able to scale up and scale down based on the load on the website.</li>
            <li>The system should pass all the test cases(for that feature) at any point of development.</li>
            <li>The system should be able to perform the same when the simultaneous users are at least < 500.</li>
        </ol>
    </li>
    <li> User Friendly
        <ol type="1">
            <li>The system should be easy to use for a non-technical person.</li>
        </ol>
    </li>
    <li> Tracking Activities
        <ol type="1">
            <li>The system should log the action done on the database.</li>
        </ol>
    </li>
    <li> Structuring
        <ol type="1">
            <li>The system should follow the folder structure decided by the technical architecture for further adding any feature.</li>
        </ol>
    </li>
</ol>
