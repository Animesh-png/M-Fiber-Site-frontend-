# M-Fiber-Site-frontend-
Established proper UI and frontend development, including styling using CSS styling. Integrated the entire dashboard frontend , which can be used for recharging mobile and broadband services

DESCRIPTION : 

  
This code represents an M-Fiber Recharge Dashboard, a simple web application for managing mobile and broadband recharge services. It utilizes HTML, CSS, and jQuery to provide an interactive user interface. Below is the breakdown:

HTML Structure
---------------
Document Setup:

The <!DOCTYPE html> declares the HTML5 document type.
<html lang="en"> sets the language attribute for accessibility.
<meta> tags define character encoding (UTF-8) and ensure responsiveness (viewport).
Page Title:

<title>M-Fiber Recharge Dashboard</title> defines the title of the page shown on the browser tab.
Body Content:

A structured layout within <body> is divided into:
Header: Displays the title M-Fiber Recharge Dashboard.
Main Content: A container with two sections:
Recharge Form: Allows users to input recharge details.
Sidebar: Displays recharge history.
Interactive Elements:

Form Inputs:
Dropdown (<select>) to choose between Mobile or Broadband recharge.
Text and number inputs for recharge amount and customer number.
Submit button triggers form submission.
Recharge History:
Displayed as a list (<ul>), dynamically updated using JavaScript.

_________________________________________________________________________________________________________________________________

CSS Styling
------------
General Styling:

body is styled with a light background (#f4f4f4) and uses the Arial font.
Containers have centralized alignment and responsive design.
Specific Components:

Header: Styled with a green background (#4CAF50) and white text for prominence.
Form and Sidebar:
Box-shadow creates a card-like appearance.
Padding and margin provide spacing for better readability.
Responsive design ensures adaptability to smaller screens using media queries (@media).
Buttons:

Styled with green backgrounds and hover effects (hover pseudoclass).

_________________________________________________________________________________________________________________________________

JavaScript Functionality (Using jQuery)
----------------------------------------
Form Submission:

Listens to the form’s submit event, preventing the default behavior with event.preventDefault().
Input Validation:

Validates the number field to ensure a 10-digit format using a regular expression (/^\d{10}$/). Alerts the user if invalid.
Dynamic Updates:

On successful recharge:
Displays a confirmation message.
Appends a new list item (<li>) to the recharge history (#history), formatting the entry with details of the recharge.
Clears the input fields for a better user experience.
Styling Changes with jQuery:

Toggles visibility of the confirmation message using the removeClass('hidden') method.

_________________________________________________________________________________________________________________________________

Responsive Design
-------------------
The @media (max-width: 768px) query adjusts layout for smaller devices:
Converts the horizontal layout (flex-direction: row) into a vertical one (flex-direction: column).
Ensures that both the form and sidebar adjust their width for readability.

_________________________________________________________________________________________________________________________________

Key Features
-------------
Recharge Functionality:
Users can select between Mobile and Broadband recharge, enter amount, and provide customer numbers.
Validation:
Ensures correct input formats, enhancing user experience and minimizing errors.
Recharge History:
Displays a list of completed recharges, maintaining a record for reference.
Responsive UI:
Adapts seamlessly to desktop and mobile views.

_________________________________________________________________________________________________________________________________

Potential Improvements
-----------------------
Enhanced Validation:
Extend validation to check recharge amounts (e.g., minimum/maximum limits).
Persistent History:
Use browser storage (e.g., localStorage) to retain history across sessions.
Backend Integration:
Connect the form to a server API for real-time processing and data storage.
