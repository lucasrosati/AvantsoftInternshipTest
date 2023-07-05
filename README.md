
# Avantsoft Internship Test

Avantsoft Internship Test, which consisted of consuming an API with PHP and displaying a frontend paginated table with 5 pages, each one containing 10 users.

## Features

**index.php**

The index.php file is responsible for displaying a list of users and implementing pagination. It does the following:

1) Get user data from an external API using the file_get_contents() and json_decode() function. Data is stored in the $data variable.
2) Checks for data in the $data variable using !empty($data).
3) If data is available, the $users variable is set to the array of users fetched.
4) Sets the number of users per page and calculates the total number of pages based on the total number of users.
5) Check the current page using $_GET['page'] or set the first page as default.
6) Calculates start and end indexes to display the correct users on the current page.
7) Use array_slice() function to get only current page users.
8) Displays users in an HTML table using a foreach loop.
9) Displays pagination links to navigate between pages.



**style.css**

The style.css file contains the CSS style rules for the page's appearance. It defines several style rules, including:

1) Centered text alignment for header and table cells.
2) Setting the body (body) to occupy the full width and height of the screen and use flexbox to center the content vertically.
3) Styles for the dark theme toggle button, including how the button looks (sun/moon) and changing theme colors.
4) Styles for the table, including borders,fonts, background colors, and text colors.
5) Styles for pagination, including top margin and link appearance.


## Installation

To use the provided code, you will need to have a local development environment set up with a web server (e.g. Apache) and PHP installed.

To download and install Apache Server, you need to install XAMPP, for this, use their official website: https://www.apachefriends.org/

1) Create a new directory on your local web server.
2) It is recommended to use /XAMPP/htdocs/"createddirectory"
3) Save the index.php file in the newly created directory.
4) Create a new file called style.css and copy the provided CSS code into this file.
5) Save the style.css file in the same directory as the index.php file.
6) Start the local web server.
7) Open a web browser and go to the local address corresponding to the directory where you saved the files (for example, http://localhost/mydirectory/).

By following these steps you should see the users page with the user list and pagination displayed correctly. You will also be able to switch between light theme and dark theme by clicking the theme toggle button.


    
## Authors

- [@lucasrosati](https://www.github.com/lucasrosati)

