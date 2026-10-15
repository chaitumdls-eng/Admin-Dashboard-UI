Project Overview
The Admin Dashboard UI is a beginner-friendly project built with HTML, CSS, and JavaScript. It provides a dashboard interface where administrators can log in, manage users, view user statistics, and search through user records. The dashboard of this project consists of a login page, sidebar, user statistics cards, add/edit user form, and user table. JavaScript manages the login process, user creation, editing, deletion, and search functionality. Additionally, the project uses localStorage to save user records and sessionStorage to maintain the login status during the browser session.

This project is designed for frontend learning and demonstration purposes. The login uses fixed credentials, so it does not provide secure, production-level authentication. However, it gives beginners valuable experience with DOM manipulation, browser storage, form validation, responsive layouts, and dynamic table rendering

Live Preview
Key Features
Admin Login System: It includes a login screen where users must enter the predefined username and password. JavaScript checks the credentials and displays error message if details are incorrect.
Session-Based Login Status: After successful login, the application stores "isLoggedIn" in sessionStorage. When the page loads, JavaScript checks this value and displays the dashboard if the session is still active.
Dashboard Layout: The dashboard contains a sidebar, top navigation bar, statistics cards, user form, search field, and user table. Which creates a structure similar to a basic admin management interface.
Sidebar Navigation: It displays the Admin Panel title along with Dashboard, Users, and Logout options. On smaller screens, JavaScript uses a toggle function to open and close the sidebar.
User Statistics: Dashboard contains two cards i.e Total Users and Active Users. The Total Users card shows how many people have signed up for the application, while the Active Users shows how many are online. 
Add Users: Administrators can enter a name and email address through the form and click Save. JavaScript validates the fields before adding a new user to the users array.
Edit Users: Each user row contains an Edit button that loads the selected user’s name and email into the form. The application then updates the existing record instead of creating a duplicate user.
Delete Users: Delete button removes the selected user from the users array. After deletion, the application updates localStorage and refreshes the table.
LocalStorage Data Management: User records are stored in localStorage using JSON.stringify(). Therefore, the data remains available even after the page is refreshed.
Search Functionality: Users can search the table by typing a name into the search field. The searchUser() function checks each row and hides the rows that do not match the entered text.
Dynamic User Table: JavaScript creates table rows from the stored user data. Each row displays the user ID, name, email, and Edit and Delete action buttons.
Form Validation: The saveUser() function checks whether the name and email fields contain values. If either field is empty, the application displays an error message and stops the save operation.
Responsive Design: The dashboard uses CSS media queries to respond to different screen sizes. At smaller sizes than 768px, the cards turn into a vertical layout, and the form takes the full width of the screen. Moreover, the sidebar turns into a hamburger menu.
Logout Functionality: Logout option removes the login status from sessionStorage. It then hides the dashboard and displays the login page again.
Clean Admin Interface: This project uses cards, a table, a sidebar, and a form to organize dashboard information. This structure makes the interface easier to understand and extend.
What You'll Learn
How to create a basic admin dashboard layout.
How to build a simple login interface using HTML and JavaScript.
How to validate fixed login credentials.
How to use sessionStorage to manage login status.
How to use localStorage to store user records.
How to convert arrays into JSON using JSON.stringify().
How to retrieve stored data using JSON.parse().
How to add, edit, and delete objects from an array.
How to use map(), find(), and filter() for user management.
How to generate dynamic table rows using template literals.
How to update dashboard statistics dynamically.
How to implement search functionality using querySelectorAll().
How to show and hide elements with JavaScript.
How to create a responsive sidebar using CSS media queries.
