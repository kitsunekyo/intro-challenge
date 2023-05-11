# Intro Challenge

We would like to challenge you, to see how quickly you can adapt to potentially new technologies, or what you would focus on, should the core requirements be no problem for you.
Try how far you can get in the expected timeframe. If you get stuck on some details, thats okay. Write out how you would solve the rest of the requirements and what you think is important in the implementation.

## Core Requirements
- Store your source code on a git provider of your choice and include a meaningful readme on how to start or test your project (fork this repository, or create a new one on github)
- Create a client application with typescript, react and vite (feel free to use a vite template)
- Create a nodejs express api (feel free to use express generator) with a single endpoint `/character/:code` that takes a "UTF-16 char code" as integer number and returns the corresponding character as string. eg: `GET localhost:8080/character/42` -> "*"
- The client app should show a text input field that allows users to input a number, and a button. clicking the button sends the number from the input field to the express api endpoint. the result of the http call should be shown below the input field and button.

![image](https://github.com/kitsunekyo/intro-challenge/assets/8297816/24b134d5-e19f-446c-8129-f15cdb56a66c)

## Extension
- Connect your express api to a mongodb instance (host it locally or in the cloud, e.g. on Atlas) using mongoose
- Store every integer-to-character conversion request in the database, including the original integer, the resulting character and a timestamp. A schema definition for this could look like the following:
```
const Schema = mongoose.Schema;

const Conversion = new Schema({
  number: Number,
  character: String,
  createdAt: Date
});
```
- Create a second endpoint in your express api which returns all stored conversions from your database
- Implement a second view in your react application which displays the stored conversions in a neat visual way (e.g. a  table)


## Bonus points
- Style the client application with tailwindcss
- Use typescript for the express api
- Unit test your number-to-string conversion logic with a framework of your choice to make sure it works as intended

### Resources
- https://react.dev/
- https://vitejs.dev/
- https://expressjs.com/
- https://tailwindcss.com/
- https://www.typescriptlang.org/
- https://mongoosejs.com/
- https://www.mongodb.com/atlas/database
