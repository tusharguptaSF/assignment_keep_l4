## Design & implement, Notes Application as a personal productivity tool for quickly taking (& saving) notes, organize notes efficiently. Below are its endpoints those you need to design.

- Core features
	- As a user, i should be able to register.
	- As a user, i should be able to login.
	- As a user, i should be able to create a note.
	- As a user, i should be able to list all created notes by me.
	- As a user, i should be able to update note's **title**, **text** and **state** (**started**, **not-started**, **completed**)

- What must be implemented:- 
	- NodeJS based server side application (server part only of the application)
	- Automated test cases to test the server side application
	- Must be able to interface & integrate with any web based clients
	- Implement the application using TDD approach

- API for user registration **/api/v1/users/register**
	- Registration API will insert **username** and **password** into database
	- **bycript** npm module should be used to store **password** in bycript form.
- API for login  **/api/v1/users/login**
	- User should be able to login into system using **username** and **password**
- API for creating a note **/api/v1/notes/**
	- Note model will have **id**, **title**, **text**, **state**, **userId**, **createdOn**, **modifiedOn** attributes
	- **userId** will be passed as query param into request and will be used to store notes by **userId**.
- API for getting all notes of a user **/api/v1/notes/**
	- **userId** will be passed as **query param** into request and will be used to fetch notes by **userId**.
- API for updating a note **/api/v1/notes/:noteId**
	- **noteId** will be passed as route parameters into url and will be used to update note by **id**