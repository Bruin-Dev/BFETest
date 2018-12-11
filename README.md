# BFETest
Interview project for potential Bruin Front-end Engineer

The goal of this project is to build a basic, small, working modal component for submitting a form. The form works with two APIs, one for checking if the user email is already registered, and another one to submit the user information and creating a user in the database. Its up to you to decide how to use the data from the API to create a working prototype. Feel free to use whatever tools, libraries – or even just go vanilla CSS & JS! But if you decide to use framework, use React please.

At minimum, your prototype should:

1. GET data from the API, POST data to the API.
2. Manage the modal open/close state.
3. Create a UI element that collect form data and submit data successfully.
4. Include basic form validation, and all three fields are required to save/submit the form.
5. Follow the UI specifications from the provided Figma file, you don't need to design your own.


Extra Credit:

1. Show a success modal that shows when the user is successfully created.
2. Mock an error response, turn the modal header to red and show an error message in the modal above the form.

## Interaction Specs

1. Modal contains a form that has three fields.
	* First Name: a string of user first name
	* Last Name: a string of user last name
	* Email: a string of a valid email address. It has to be a unique value in the database.
2. Click the “×” button shall close the modal.
3. Click the save button to call api to create a user, the implementation must check the the email address before creating a user to make sure the email will be unique.
4. If the email has already been registered by another user, there should be an error message shown up next to the email field.
5. The modal shall be close if the user is created successfully.

## API

`https://jsonplaceholder.typicode.com/users`

Fetch a user: GET endpoint, `https://jsonplaceholder.typicode.com/users?email=Sincere@april.biz`.
Create a user: POST body, { firstName: 'John', lastName: 'Doe', email: 'jdoe@company.com' }, the response will return the new user id.

## Figma File

`https://www.figma.com/file/Mnr5nvzRuP39kjGY6O9ZMYgN/Front-end-Test?node-id=0%3A1`

If you find yourself getting stuck on anything, don't hesitate to reach out and ask questions. Good luck!
