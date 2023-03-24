This repo include 'user interface specification' document.

# User Management Screen
The User Management Screen provides a list of existing users and allows you to add new users. The list displays the ID, User Name, Email, and whether the user is Enabled (active) or not. You can edit user information by clicking on the user row in the list.

## User List
The User List displays all users in the system. The table columns are:

- ID: The unique identifier of the user.
- User Name: The user name of the user.
- Email: The email address of the user.
- Enabled: Whether the user is currently active or not.
- Users are listed in alphabetical order by User Name.

### Hide Disabled User Checkbox
There is a checkbox labeled 'Hide Disabled User' next to the 'New User' button. When this checkbox is checked, only enabled users are displayed in the User List Table. When it is unchecked, all users, both enabled and disabled, are displayed.

## New User Form
Clicking on the 'New User' button opens the New User Form. This form allows you to add a new user with the following fields:

- Username: The user name of the user (required, alphanumeric characters only).
- Display Name: The display name of the user (required, up to 50 characters).
- Phone: The phone number of the user (optional, up to 20 characters).
- Email: The email address of the user (required, up to 100 characters).
- User Roles: The role(s) of the user (required, one or more of Guest, Admin, or SuperAdmin).
- Enabled: Whether the user is currently active or not (required, defaults to true).
- The User Roles field is now a set of checkboxes instead of a dropdown list. You can select one or more of the Guest, Admin, or SuperAdmin roles.

## UI Components
The User Management Screen consists of the following UI components:

- User List Table: A table that displays a list of existing users.
- New User Button: A button that opens the New User Form.
- Hide Disabled User Checkbox: A checkbox that toggles the display of disabled users in the User List Table.
- New User Form: A form that allows you to add a new user.

## Behavior of Components

### User List Table
The User List Table displays a list of users in alphabetical order by User Name. The table displays the following columns:

- ID: The unique identifier of the user.
- User Name: The user name of the user.
- Email: The email address of the user.
- Enabled: Whether the user is currently active or not.

Clicking on a user row in the table opens the Edit User Form.

### New User Button
Clicking on the New User Button opens the New User Form.

### Hide Disabled User Checkbox
When the 'Hide Disabled User' checkbox is checked, only enabled users are displayed in the User List Table. When it is unchecked, all users, both enabled and disabled, are displayed.

### New User Form
The New User Form allows you to add a new user with the following fields:

-Username: The user name of the user (required, alphanumeric characters only).
- Display Name: The display name of the user (required, up to 50 characters).
- Phone: The phone number of the user (optional, up to 20 characters).
- Email: The email address of the user (required, up to 100 characters).
- User Roles: The role(s) of the user (required, one or more of Guest, Admin, or SuperAdmin).
- Enabled: Whether the user is currently active or not (required, defaults to true).

Once you have filled out the form, clicking the 'Create User' button adds the new user to the system and redirects you back to the User List Table.

## Initial Display
When the User Management Screen is first displayed, the User List Table is populated with all users in the system, including those that are disabled. The 'Hide Disabled User' checkbox is unchecked.

## Error Handling
If there are any errors in the form, such as missing or invalid input, the form will display an error message next to the corresponding field(s). When the form is submitted, the User Management Screen will display a message indicating whether the user was successfully created or if there was an error.

## Conclusion
The User Management Screen allows you to manage users in the system by displaying a list of existing users and allowing you to add new ones. The screen includes a User List Table, New User Button, and New User Form, along with a Hide Disabled User Checkbox that toggles the display of disabled users in the User List Table. The New User Form now includes checkboxes for User Roles. Error handling is implemented to prevent invalid input and to provide feedback to the user.

## Visual Representation
Here is a visual representation of the User Management Screen:

:-- +-------------------------------------------------+
:-- |             User Management Screen              |
+-------------------------------------------------+
|                           
|   [ New User ]         [ ] Hide Disabled User   |
|                                                 |

|   User List Table                               |
|                                                 |
|   +----+-------------+----------------+-------+
|   | ID | User Name   | Email          | Enabled |
|   +----+-------------+----------------+-------+
|   | 1  | AdminUser| admin@piworks.net    | true |
|   | 2  | TestUser | testuser@piworks.net | true |
|   +----+-------------+----------------+-------+
|                                                 |
|                                                 |
|   New User Form                                 |
|                                                 |
|   Username:  [___________]                      |
|                                                 |
|   Display Name: [___________]                   |
|                                                 |
|   Phone: [___________]                          |
|                                                 |
|   Email: [___________]                          |
|                                                 |
|   User Roles:                                   |
|   [ ] Guest                                     |
|   [ ] Admin                                     |
|   [ ] SuperAdmin                                |
|                                                 |
|   Enabled  [x]                                  |
|                                                 |
|   [Create User]                                 |
|                                                 |
+-------------------------------------------------+
Note: This is just a sample mockup and the actual design may differ based on the requirements and preferences of the project.




