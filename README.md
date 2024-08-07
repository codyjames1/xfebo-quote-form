# Free Quote Form - First Choice Health Company
This repository contains the HTML and JavaScript code for the multi-step form used by First Choice Health Company to provide free quotes for final expense coverage.

## Table of Contents
Overview
Features
Technologies Used
Form Steps and Functionality
Validation and Formatting
Data Submission
Additional Scripts
Folder Structure
License
Overview
The multi-step form collects user information to provide a free quote for final expense coverage. The form is designed with a focus on user experience, ensuring each step is straightforward and easy to complete. This document provides a detailed explanation of how the form was built, including the technologies used, form steps, validation, data submission, and additional scripts.

# Features
Multi-step form with progress indicators
Input validation for each step
Phone number formatting
AJAX submission to multiple endpoints
Loading animations and thank you message upon form submission
Handles iFrame loading for embedded usage
## Technologies Used
HTML5
CSS3
JavaScript (ES6)
jQuery
Ionicons for icons
Lottie for loading animations
## Form Steps and Functionality
### Step 1: ZIP Code
Collects the user's ZIP code.
Auto-fills ZIP code and IP address using the IPinfo.io API.
### Step 2: Gender
User selects their gender (Male/Female).
Enables the "Next" button once a selection is made.
### Step 3: Birth Year
User inputs their year of birth.
Enables the "Next" button once the field is filled.
### Step 4: Health Status
User selects their health status (Poor/Fair/Good).
Enables the "Next" button once a selection is made.
### Step 5: Name
User inputs their first and last name.
Enables the "Next" button once both fields are filled.
### Step 6: Contact Information
User inputs their phone number and email address.
Formats phone number input.
Enables the "Submit" button once both fields are filled.
# Validation and Formatting
Input fields are validated to ensure required information is provided.
Phone number field auto-formats to the (XXX) XXX-XXXX format.
Year of birth field allows only numerical input and ensures it is a valid year.
# Data Submission
Form data is submitted via AJAX to two endpoints:
### ChaseDataCorp CRM API
### Google Sheets Script
### Displays loading animation and thank you message upon successful submission.
### Uses a hidden iframe to handle form submission and response.
# Additional Scripts
### IP and ZIP Code Fetching: 
Uses IPinfo.io API to auto-fill ZIP code and IP address.
### iFrame Detection: 
Detects if the form is loaded within an iFrame and adjusts styling accordingly.
### Form Progression: 
JavaScript functions manage the visibility and progression of form steps.
### Lottie Animation: 
Displays a loading animation during form submission.

This project is licensed under the MIT License - see the LICENSE file for details.
