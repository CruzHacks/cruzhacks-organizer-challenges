# CruzHacks 2023 Backend Engineering Challenge

## Challenge

In this challenge, you will create a REST API that will support GET, POST, and PATCH operations for applicants in a database. In order to build this, please follow [this schema](https://docs.google.com/document/d/1BgSQSDng0lSiNozgYCiJHzBA3ezg9MRalg9fIrSapbU/edit?usp=sharing)  when creating your repository

Our testing will be done using Postman, so we recommend you use this to format the request bodies for your documentation.

## Technology

You can use any language and database you'd like provided you document how to setup and run your server in your README. This year we will be using Firebase and Typescript Node.js to write our backend so we **recommend** you use this stack. JavaScript/TypeScript is really easy to learn and allows for really fast development of your API.

## GET Request

The GET Request should satisfy the following requirements:

* GET applicant by email
* GET applicant by ID in database

## POST Request

The POST Request should satisfy the following requirements:

* POST using schema described above

## PATCH Request

The PATCH Request should satisfy the following requirements:

* Using an email, PATCH any field in the Schema EXCEPT the email and Applicant Type

## DELETE (optional)

Feel free to add a delete option as well which would:

* DELETE by ID
* DELETE by email

## Security (optional)

It's important to make sure our endpoints are not able to be accessed by unauthorized users. We suggest looking into [JWTs](https://jwt.io/introduction) to securing your endpoints. We will most likely be using Auth0 to develop our security for our endpoints this year, but many databases have their own built in JWT APIs. In Firebase, for example, they are known as tokens.

## Unit Testing (optional)

In a CI/CD environment, it is very likely we will make changes to our architecture. However, it is important that any change we do does not affect endpoints that only exist without good reason. For this reason, we suggest looking into unit testing each of your endpoints for the functionality they should provide (Mostly Responses). If you are working in Node.js, we will be using Jest and Supertest to test our endpoints.

## Documentation 

Documentation is an incredibly important part of being a developer. You want to create your program so that any other developer can understand what your program does at a glance. For this challenge we **strongly recommend** you fulfill as many of the documentation standards we give below:

* Consistent naming scheme for variables
* Comment functionality of all your functions or anything that is not obvious at first sight
* Create a README that explains how to use your endpoints (How to run your application, and an example of your Schema and usage of your endpoints)

## Style

We don't have a specific coding style for this challenge so feel free to use your own. However, we do want you to make your naming scheme as consistent as consistent as possible. For example, variables follow snake_case while functions follow PascalCase, the choice is up to you of course. In addition, we will be looking for modularity of code. It should be quick and easy to make adjustments to your code if necessary, so try and break up your code wherever you see fit.

## Submission

We understand that this is quite a bit, especially to fit into your busy college lives. That said, we do want to see as many specifications completed as possible. While we are looking for functionality, we are also looking for mindful developers that take care in developing their applications with maintability in mind. 


### How to Submit

To send us your application:
* Create a Github repo to host your application. [If you're unfamiliar with Git, this will get you running.](https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/)
* Create a zip of your application
* Email a link of your repo to [contact@cruzhacks.com](mailto:contact@cruzhacks.com) and cc [dev@cruzhacks.com] with the subject line `CruzHacks Challenge - Last, First`, or send us a zip of your code with the file called `Last_First_CruzHacks_Backend.zip`.
    * Please include any .env information necessary to run the application
    * Please **DO NOT** include any node_modules folder in your repo, just the package.json and package-lock.json should be fine.
    * If you have any other sensitive files that should not be shared in a git repo add a file called `backend_secrets.zip`

* If you are also attempting the frontend challenge, please attach the other challenge in the same email.