we would like to challenge you, to see how quickly you can adapt to potentially new technologies, or what you would focus on, should the core requirements be no problem for you.
try how far you get in 1-3 hours. if you get stuck on some framework details, thats okay. write out how you would solve the rest of the requirements and what you think is important in the implementation.

### requirements
- create a client application with typescript, react and vite (feel free to use a vite template)
- create a nodejs express api (feel free to use express generator) with a single endpoint `/character/:code` that takes a "UTF-16 char code" as integer number and returns the corresponding character as string. eg: `GET localhost:8080/character/42` -> "*"
- the client app should show a text input field that allows users to input a number, and a button. clicking the button sends the number from the input field to the express api endpoint. the result of the http call should be shown below the input field and button.

![image](https://github.com/kitsunekyo/intro-challenge/assets/8297816/24b134d5-e19f-446c-8129-f15cdb56a66c)

### (optional) bonus points
- style the client application with tailwindcss
- use typescript for the express api
