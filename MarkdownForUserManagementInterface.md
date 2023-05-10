# User Management Screen UI Specification

## Requirements
- The user management screen should allow admins to manage user accounts.
- The screen should allow admins to add, edit, disable, and view user accounts.
- The screen should display a list of all user accounts in a table.
- The table should allow sorting and filtering of user accounts.
- The screen should allow admins to hide disabled user accounts.
- The screen should display appropriate error messages if any errors occur during user account management.

## UI Components

### Top of Screen
- There should be a html div at top of the screen. This div should be like a header div and its length should be of reseanoble size to contain a button.
- There should be three components located in this div (The "New User" button, the "Hide Disabled User" checkbox, and the "Save User" button).
- The "New User" button should be blue have a "+" sign before the "New User" text and located at the left end of the header div.
- The "Hide Disabled User" checkbox should be next to the "New User" button, but with reasobable space between them.
- The "Save User" button should be located at the other end. By the right end of the header div, have a blue background but with a white overlay- indicating that it isn't active yet.

### User Account Table
- The user account table should display the following information for each user account:
  - ID
  - User Name
  - Email
  - Enabled (values should be true or false)
- The table header should have a blue background, and the name of the columns listed above written in white - each having two white icons to their right end; a sort icon (arrow up and arrow down) and a filter icon (a funnel) just after the sort icon, and every column demarcated with thin white lines.
- The table should allow sorting of user accounts by any of the columns.
- The table should allow filtering of user accounts by any of the columns.
- The table should have a white background and user details in black text.

### New User Account Form
- Heading should be "New User" and the div containing this should have an ash background with the "New User" text written in black.
- The form should have a white background and texts in black.
- The New User account form should include the following fields:
  - Username
  - Display Name
  - Phone
  - Email address
  - User Roles (Guest, Admin, SuperAdmin)
  - Enabled (A check box should be displayed here)
- The form should display appropriate error messages if any required fields are left blank or if the email address is not valid.
- The form should be displayed side-by-side with the user account table.


## Page Behavior
- When the user management screen is loaded, it should display the user account table with all user accounts.
- Admins should be able to add a new user account by clicking on the "New User" button and filling out the New User account form which will be displayed side-by-side with the user account table.
- If any errors occur during user account management (e.g. a required field is left blank), appropriate error messages should be displayed to the admin.
- The "Save User" button should have a blue background but with a white overlay- indicating that it isn't active yet. This white overlay should be removed and the button made active once the details of the New User has been entered.
- When the "Hide Disabled User" checkbox is checked, it should turn blue with a white checkmark, and all disabled users should be hidden and not shown on the table.

## Initial Display
- When the user management screen is loaded, it should display the user account table with all user accounts sorted by ID in ascending order.
- The header div should be displayed with all of its components.
- The "Save User" button should have a blue background but with a white overlay- indicating that it isn't active yet.