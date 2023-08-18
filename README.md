# Creating a Single-Page React Application
Manage user profiles and dynamically display different components based on user roles. Here's what you need to do:


1. **Header**: Display a header that reads "Welcome to the app, \$USER!".
2. **User Card**: Create a card component that displays a user's profile picture, name, email, and phone number.
3. **Fetch user**: Implement a fetch function to fetch users on button click from the provided api. Display any one of them with the card component.
4. **Role-based Components**: Show different components in the app based on the current user's role(s):
   - **Admin**: Display an "Admin Settings" button and "Delete User" button.
   - **Editor**: Enable the Edit -> Save button for editing the profile.
   - **Viewer**: Disable all edit functionalities; show only the user profile.
5. **Editable Fields**: Allow users with "Editor" role to edit the name, email, and phone number via an Edit -> Save button at the bottom of the card. Implement a function to save the edited version to the api.
6. **State Synchronization**: Sync the value of the user's name to the header.

api endpoints:
`https://user-workers-demo.alexpear.workers.dev`
`GET /users` : returns a list of users
`PATCH /users/:id` : edit user info (email and name)
