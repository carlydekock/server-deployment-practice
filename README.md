# LAB: Node Ecosystem, CI, CD

Time to get hands on with Node.js development! Today, you'll create and deploy a web server using CI and CD and get used to the general process of building and deploying servers, and prepping your work for grading.

## [Link to GitHub Repository](https://github.com/carlydekock/server-deployment-practice.git)

## The Setup

### How to install

- Clone down repository from GitHub
- Run the command ```npm install``` to install dependencies (dotenv, express, jest, supertest)
- create .env file with PORT variable

### How to test

- Run the command ```npm test``` to test and verify the server is working

### How to run

- Start the server using ```nodemon```
- Visit http://localhost:PORT at the PORT number you've assigned in your .env

## Lab Instructions

### Github

1. Create a new repository at GitHub, called `server-deployment-practice`
   - Select the "Add a README" option
   - Select the "Add a .gitignore" option, and choose Node.js
   - Opt for the MIT license
1. Clone this to your local machine.

### Heroku

At heroku, we're going to setup 2 deployments. One for your dev branch and one for your main branch. As you check in code, you should be able to see Heroku instantly deploy from GitHub, assuming your tests pass!

1. Login to your Heroku account
1. Create a new Heroku app, called `yourname-server-deploy-prod`
   1. Go to the deployment tab
   1. Choose "GitHub"
   1. Connect to your repository
   1. Choose the "master" or "main" branch
   1. Choose the "Wait for CI to pass before deploy" option
   1. Choose the "enable automatic deploys" option

### The Code

You've been provided a working demo server by your instructor. Get this code working locally. Note that while you are permitted to simply copy the files, it's better if you create the server from scratch, typing the lines of code in the demo provide. Build up your muscle memory

1. Initialize your app -- `npm init -y`
1. Install your dependencies -- `npm install dotenv express jest supertest`
1. Create the files and folders required for the application
1. Create the correct content in the files
1. Test your server -- `npm test`
   - You should see 100% of tests passing
1. Start your server -- `nodemon`
   - Visit <http://localhost:3000/data> in your browser to confirm that the server is visible

## Deployed links

- [Link to deployed site](https://carlydekock-server-deploy-prod.herokuapp.com/)
- [Link to GitHub actions](https://github.com/carlydekock/server-deployment-practice/actions)
