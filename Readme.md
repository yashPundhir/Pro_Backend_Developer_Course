# Pro Backend Development Course from LCO

## Section 1: Getting Started (6 Videos)

- Intro => `done`
---
- Tools for Backend => `incomplete` 
  - Description about Postman => 3:18 to 5:50
  - To Understand API:
    - [What is API by AWS](https://aws.amazon.com/what-is/api/) 
    - [What is API by MuleSoft](https://www.mulesoft.com/resources/api/what-is-an-api) => Watch only the video of this article.
  - To Understand YAML:
    - [YAML Tutorial by CloudBees](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started)
    - [YAML Crash Course by Hitesh Sir](https://www.youtube.com/watch?v=9BGWtTahGnw)
---
- MongoDB Mac/Linux Installation => `done`
  - Installation of MongoDB on Mac and Linux is similar so same video will work for both.
  - [MongoDB Mac/Linux Installation according to Pro Backend Course](https://www.youtube.com/watch?v=MIByvzueqHQ)
  - [MongoDB Mac Installation wrt to latest settings](https://www.youtube.com/watch?v=s1WQ0eEpqqg)
  - `Keep in mind all the key pointers specified in the videos so that margin of error is minimum wrt installation`
---
- MongoDB windows install => `done`
  - [MongoDB Windows Installation according to Pro Backend Course](https://www.youtube.com/watch?v=sluiQOXKUmQ)
  - But there are some complexities wrt the Installation video given above. The Current Version of MongoDB that I have installed is 6.0.3 and in this version the Legacy MongoDB Shell is unavailable. So a new and enhanced MongoDB Shell aka `mongosh` need to be installed separately so that the MongoDB Servers could run properly.
  - [MongoDB Server Community Edition Download Link](https://www.mongodb.com/try/download/community)
  - [MongoDB Server Installation Docs](https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-windows/)
  - [MongoDB Shell (mongosh) Download Link](https://www.mongodb.com/try/download/shell)
  - [MongoDB Shell (mongosh) Installation Docs](https://www.mongodb.com/docs/mongodb-shell/install/)
  - `Keep in  mind to download both MongoDB Server as well as MongoDB Shell (Mongosh) in .msi format and not in .zip format bcz the task of adding the required binary to the PATH environment variables is being handled by .msi installer automatically but in case of .zip files, it needs to be done manually`
  - To start MongoDB Server: 
    - Open cmd in `administrator` mode
    - Then write the following command:
    ```console
    net start mongodb
    ```
  - To stop MongoDB Server: 
    - Open cmd in `administrator` mode
    - Then write the following command:
    ```console
    net stop mongodb
    ```
  - To run MongoDB Shell CLI:
    - Open cmd in `normal` mode
    - Then write the following command:
    ```console
    mongosh.exe
    ```
  - To exit from the MongoDB CLI:
    - Either press `ctrl + D` once or press `ctrl + C` twice or type `.exit` in the currently opened cmd console
  - `Note:` MongoDB Shell CLI gets activated only when the mongoDB Server is up running, otherwise it will give error. So, in case of error while activating Shell CLI, just verify whether the MongoDB server is running or not
---
- MongoDB in cloud - Atlas => `done`
  - This video contains the basic overview of the cloud based MongoDB aka MongoDB Atlas
  - This vdo might be helpful in case of working with the MongoDB Atlas bcz it gives the walkthrough as well as how to do the basic settings and stuff.
  - But then Hitesh Sir recommended that it is better to work with MongoDB installed locally on the system so I'll go with local setup only.
---
- MongoDB GUI - Compass => `done` `Important`
  - MongoDB Cmpass is a tool that helps us to give a visualization of the database and it gives us the advantage in debugging the code.
  - This video is imp as it gives the overview of how to work with our databases using a GUI (MongoDB Compass)
  - How to connect MongoDB Compass to a MongoDB Atlas Cluster => 2:17 to 5:00
---
## Section 2: Take it up to Heroku - Production (12 Videos + 1 SandBox) (SandBox is given only for reference)

- Things you need to deploy on Heroku => `done`
  - Basic overview of the Entire Section
  - Hitesh Sir is using `Heroku` to push the application to the production as `Free Tier` was available at that time.
  - But now as `Heroku's Free Tier has ended` few other options can be considered to Push Application to the production instead of Heroku
  - Such few alternatives of Heroku are: 
    - [Cyclic](https://www.cyclic.sh/)
      - Free Tier is available with lots of features
    - [Railway](https://railway.app/)
      - Free Tier is available with less features
    - [Render](https://render.com/)
      - Free Tier is available with functionality similar to Heroku
    - [Digital Ocean](https://www.digitalocean.com/)
      - Free Tier is not available but Paid Version is also not that much costly
      - This platform is very good for Professional Applications Deployment
  - [Application Deployment on Render, Railway & Cyclic](https://www.youtube.com/watch?v=MusIvEKjqsc)
    - This video is helpful as it gives the basic introduction as well as the deployment steps for each Platform (Render, Railway & Cyclic)
---
- Plan your application => `done`
  - This video is all about planning the entire flow of the application using the `Mind Mapping Tool`
  - `Miro` is the Mindmapping Tool that I have used:
    - [Miro](https://miro.com/mind-map/): Just Sign In & start drawing the Mind Map to plan the flow of the application
    - Imp shortcuts of Miro:
      - Scroll Up to Zoom in
      - Scroll Down to Zoom Out
      - Right Click and Drag to Move within the Drawing Space
      - Click on the Miro Icon in the top left corner to exit the drawing space
      - Click on the `?` Icon in the bottom right corner to access the tutorials
---
- Types of web requests => `done`

  - [Types of Web Requests](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)
---
- Framework - Express, Koa, Hapi => `done`
---
- Starting with package.json File => `done`
---
- My 1st Express App => `done`
---
- Request Response & Status Code => `done`

  - [HTTP Response Status Codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
  - [Explanation about HTTP Cookies](https://www.youtube.com/watch?v=rdVPflECed8&t=181s)
---
- All Social Routes => `done`
---
- Handle the Date Situation => `done`
---
- Parameters and Bugs in Route => `done`
---
- Pushing app to HEROKU => `done`
---
- Debug Social App in Production => `done`
---
- Social App - Sandbox => `My code is similar to Hitesh Sir's Code`
  - [Social App GitHub Repo](https://github.com/yashPundhir/socialApp_ProBackend)
---
## Section 3: Swagger Docs (15 Videos + 1 SandBox) (SandBox is given only for reference)

- What is Swagger & API Docs => `done`

  - [Specification Guidelines](https://swagger.io/specification/)
  - [**Basic Structure**](https://swagger.io/docs/specification/basic-structure/)
---
- Nodemon ext & YAML Docs => `done`

  - [swagger-ui-express](https://www.npmjs.com/package/swagger-ui-express)
  - [swagger-jsdoc](https://www.npmjs.com/package/swagger-jsdoc) : Recommended when writing API Docs on top of every Route.
  - [yamljs](https://www.npmjs.com/package/yamljs)
  
  - To Understand YAML:
    - [YAML Tutorial by CloudBees](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started)
    - [YAML Crash Course by Hitesh Sir](https://www.youtube.com/watch?v=9BGWtTahGnw)
---
- Authentication token for swagger docs => `done`
  - In Swagger Docs, under the Servers, whichever URL is selected, all the requests will be going to that particular URL.
---
- Docs for HTTP Methods Swagger => `done`
---
- A new documentation centric project => `done`
---
- Setup Information - Swagger => `done`
---
- Authentication and Authorization - Swagger => `done`
---
- String based GET Request - Swagger => `done`
---
- Handling objects - Swagger => `done`
---
- Handling Array in Swagger Docs => `done`
---
- Sending Data in URL - Swagger => `done`
---
- Managing Request Body in Swagger => `done`
---
- Handle URL Query in Swagger => `done`
---
- Handling Images in Swagger => `done`
---
- Handling Header Tokens in Swagger => `done`
---

## Section 4: Authentication (18 Videos + 1 SandBox) (SandBox is given only for reference)

- Topics covered till Section 3 in Backend => `done`
---
- Hiding Secrets in Backend => `done`
---
- Picking up a DB for Backend => `done`
---
- Why we need Mongoose - ODM => `done`
---
- Pro DB Modeling Tools => `done`
---
- Creating Model for Auth Systems => `done`
---
- Creating Basic Structure for auth systems => `done`
---
- Creating User Schema & Dotenv => `done`
---
- Registering a User in Auth System => `done`
---
- DataBase Connection in Auth System => `done`
---
- What is a Middleware => `done`
---
- Handling Password Situation => `done`
---
- What is JWT & Creating Token => `done`
---
- Register Route in Auth App => `done`
---
- Login Flow for Auth App => `done`
---
- Web vs Mobile => `done`
---
- Writing custom Middleware => `done`
---
- Setting up secure cookies => `done`
---

## Section 5: File, Image & Form Handling (8 Videos)

- Why people face issue in image upload => `done`
---
- Cloudinary & EJS => `done`
---
- How GET Works & PostMan Isues => `done`
---
- Using Template Engines => `done`
---
- Biggest Confusion in Front-End Forms => `done`
---
- Handling Images in Forms => `done`
---
- Handling Images in Forms part 2 => `done`
---
- Upload Image to Cloudinary or other providers => `done`
---
- Handling Multiple files & Uploading them => `done`
---

## Section 6: Theory & Razorpay (7 Videos)

- File Structure for Production App => `done`
---
- Getting a Logger - MORGAN => `done`
---
- Error Handler & Promises => `done`
---
- Sending Emails Using NodeMailer => `done`
---
- Why Mongoose Docs are Important => `done`
---
- Razorpay Project => `done`
--- 
- Razorpay Front-End Integration => `done`
--- 

## Section 7: Big E-Commerce App Starts (6 Videos)

- Project Requirement => `done`
---
- User Modeling & File Structure => `done`
---
- Product Model Discussion => `done`
---
- Order Model Discussion => `done`
---
- How Forgot Password Feature Works => `done`
---
- Functions in User Model & Hooks => `done`
---

## Section 8: Basic Config & Imports (6 Videos)

- Getting Files & Folders Ready => `done`
---
- Preparing Basic Express App => `done`
---
- Routes & Controllers in Dummy => `done`
--- 
- Injecting Docs & Middleware => `done`
---
- Custom Error Handlers => `done`
---
- The Big Promise => `done`
--- 

## Section 9: User Model & Signup (12 Videos)

- Creating a User Model & Validator => `done`
---
- Password Encryption & Mongoose Prototypes => `done`
---
- Validating The Password => `done`
---
- Creating JWT Tokens => `done`
---
- Forgot Password & Crypto Hashing => `done`
---
- User Routes & Postman => `done`
---
- Signup a User & Cookies => `done`
---
- DataBase Connection => `done`
---
- Testing the User Signup with Postman => `done`
---
- Handling Image Upload => `done`
---
