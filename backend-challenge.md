# CruzHacks 2022 Backend Engineering Challenge

In this exercise, we’re asking you to create a [REST API](https://restfulapi.net/) that supports the application portal created in the frontend challenge.  

## Notes

Any updates, general questions, and additional notes will be listed here and I will update this section throughout the challenge. While unrealistic for any changes in the challenge description, if there are changes don't worry if your application is based on older specifications.

____
### FAQ


### Updates

____

## Challenge

Your task is to create a series of API endpoints that perform basic [CRUD (Create, Read, Update, Delete)](https://www.codecademy.com/articles/what-is-crud) operations for a simple application portal. The application database will consist of applicant documents, which stores applicant information. You will need to create endpoints that support GET, PUT, POST, and DELETE requests. 

* GET will be used to retrieve information on applicants in your database
* POST will create a new submission document in your database
* PUT will update a submission document in your database
* DELETE will delete a submission document in your database

You can use any programming language you want, we **recommend** that you use a [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) or [Typescript](https://www.typescriptlang.org/). In the past we've deployed our APIs through [firebase cloud functions](https://firebase.google.com/docs/functions). Javascript is also extremely high powered and provides a lot of tools for quick development.

## Database Schema

Your database schema should follow the application portal's fields. When validating data both the client and server should integrate some validation. Please refer to this [schema](https://docs.google.com/document/d/1_sfDZU1M_3VnejPx7pqxIdOLxWbW_DZVOmeB4UrA3q4/edit#) when creating your database.

You can use any [NoSQL](https://www.geeksforgeeks.org/introduction-to-nosql/) database you want. We **strongly recommend** Firebase but again you can use whatever NoSQL database you feel best with.

## Endpoint Functionality

* Get all the applicants
* Get an applicant by a specific document id and or email
* Get all hackers
* Get all volunteers
* Create a new applicant document
* Update an applicant document 
  * Prevent updating Email or Application Type
  * Given a PUT request with the following body `{"age": 21, "major": "Computer Engineering"}` should update the given fields
* Delete an applicant document given an id and or email

### Security Rules

Security is a very serious part of being a software engineer at CruzHacks, especially when it comes to user information. For all endpoints include authentication to ensure that only specific users are able to reach the endpoint. We don't expect a full implementation of creating and signing tokens with timeouts but we do want to see you implement some level of security within the endpoints to ensure that only certain users can access our endpoints. We recommend that you check out [jwt](https://jwt.io/) if you want to get an idea of authentication.

### Our Testing

Your completed program should be functional and provide appropriate responses when tested with actual API requests. It's your choice on how you want to implement the response format, just ensure you are providing enough information that if a client wanted to use your program they would know whether it succeeded or not and what errors may have occurred. 

We will be testing your APIs using [Postman](https://www.postman.com/).

As software engineers, being able to write and implement code is half the solution to a problem. Testing allows us to prove that our code meets expectations and we can catch errors before shipping to the public. We would like you to perform unit tests that debug your functions. 

### Documentation 

Documentation is extremely important as we are designing applications that should be able to used for future development teams. Your code should be easy to read so consistent naming conventions, comments in your code, and modularity are needed. Please include, in a README, thorough instructions on how to run your application, response schemas, why did you design your application the way you did, what went well, what didn't go well, and what things you could have done better.

## Submission

There is a lot of content within this challenge and we do expect that you have functionality for a good chunk of this challenge. We don't expect every requirement and recommendation to be completed but we want to see what you can do so don't worry if you can't complete the entire challenge. Try your best to take on each part of this challenge. We are looking for developers who are thinking about their design and are willing to take on these challenges. 

### How To Submit

* Create a public Github repo with your project. [If you're unfamiliar with Git, this will get you running.](https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/)
* Create a zip of your application
* Email a link of your repo or or send us a zip of your code with the file called `Last_First_CruzHacks_Backend.zip` in the email to [contact@cruzhacks.com](mailto:contact@cruzhacks.com) and cc [dev@cruzhacks.com] with the subject line `CruzHacks Challenge - Last, First`.
  * Please include any .env information necessary to run the application
  * If you have any other sensitive files that should not be shared in a git repo add a file called `backend_secrets.zip`

* If you are also attempting the other challenge, please attach the other challenge in the same email.

Good luck and we'll get back to you all as soon as possible! We can't wait to see what everyone here can do!

If you ever have questions or need help, please reach out to us at [contact@cruzhacks.com](mailto:contact@cruzhacks.com) or [dev@cruzhacks.com](mailto:dev@cruzhacks.com).
