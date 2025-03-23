Chat Interface Assessment

Set Up Instructions
-Once the application is downloaded from GitHub open it as a project on Visual Studio
-Simply run the application from Visual Studio and it will run at localhost in a new browser window

How the application works
--Once the application is launched you will be presented with a login page.
--For the assessment the correct values are "Admin" and "Admin123" for username and password respectively.
--The user will then be redirected to the chat page.
--There will be a text input presented to the user. The user must enter a question in the input and 
  press the "Enter" button.
--The user's message as well as a "Loading response..." message will appear in a chat window
--The user has the option to clear the chat history by pressing the "Clear" button
--Note that the post action takes a bit of time and on more complex requests the API post action might timeout
--Please note that the APi Key might need to be updated if the application gives a 401 error. This can be done by getting an API Key
  on OpenRouter and assigning it to the APIKey variable.

Chosen Hosting Model
--Blazor Server was chosen as per recommendation by the assessment document

Design Choices
--An encrypted version of the password is used to compare to the entered password, which is encrypted upon submission,
  to simulate how it will be done in a real world scenario
--A list was used for the chat history for ease of adding and removing elements
--A "Loading response..." message was used to display to the user that the response is being fetched for a seamless
  user experience
--A "Clear" button was added to give the user an option to clear the chat history
--Both the "Enter" and "Chat" buttons are disabled while the action is running to prevent the user to enter multiple
  calls at once
--DeepSeek R1 Zero was chosen as the free model for this project
