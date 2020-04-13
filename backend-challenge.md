# CruzHacks 2021 Backend Engineering Challenge

In this exercise, we’re asking you to create a simple REST API that supports the application portal created in the front end challenge.  

**NOTE**: This year, we will be using Firebase to host and deploy our site and functions. We are asking all applicants to create and deploy their functions via [Firebase](https://firebase.google.com/).

## Challenge

Your task is to create a series of API endpoints that perform basic [CRUD (Create, Read, Update)](https://www.codecademy.com/articles/what-is-crud) operations for a simple application portal. The application database will consist of hacker documents, which stores hacker information. You are expected to create API endpoints that supports POST, PUT, and GET requests.

* POST will create a hacker document in your database
* PUT will update your hacker's data
* GET will retreieve that information and display it in your appliacation portal until it's been submitted. Information should not be able to be updated once submit has been pressed.

## Database Schema

Your database schema should follow the application portal's fields. Form validation should be done client side, but fields inside each hacker object should have their respective constraints. Please refer to this [schema](https://docs.google.com/document/d/1gPo9_31LTOIkPMnFt-n4zWBOg7HsOB-yEDPmuAKsM6I/edit) when creating your database.

As mentioned, our team will be using Firebase this year, so we ask that your database also be hosted on Firebase as well. For the application portal, we will be using the [Cloud Firestore Database](https://firebase.google.com/docs/firestore).

### Sample Responses

Your completed program should be fully functional and provide appropriate responses when tested with actual API requests.

For example, the following request:

`curl -X POST -H "Content-Type:applicaton/json" http://[projectID].cloudfunctions.net/getHackerInfo -d '{"firstName": "John", "lastName": "Doe:}'`

Will create a hacker document in your hacker database with John Doe's information inside that document. It might return JSON similar to:

```json
{
  "code": 200,
  "message": "Succesful post to database"
}

OR

{
  "code": 400,
  "message": "Unable to add user to database"
}
```

Keep in mind this is an example for one endpoint, your completed program should have enough endpoints that allow for full CRUD functionality on the hacker object.

## Things to Consider

As software engineers, being able to write and implement code is half the solution to a problem. Testing allows us to ensure that our code will run properly during production and allows us to catch errors before releasing our product to the public. As an addition to our REST API Backend challenge, we are asking you to not only to create and implement functions, but to test your code along the way. Using Mocha and Firebase's testing suite, we are asking you to perform [unit tests](https://firebase.google.com/docs/functions/unit-testing) that debug your functions.

## Submission

Don't be discouraged if you are unable to complete the challenge in its entirety. We are looking to see how, as software engineers, you tackle each problem presented to you. You will not be judged based on how much you completed, rather on the thoroughness of your work.

### How To Submit

* Create a public github repository containing code for your functions and your tests
* Your Readme inside your repository should contain the necessary information that we should know regarding your project
* Readme should also contain the links to your API endpoints so we can properly test your code
* If you are also attempting to do the frontend challenge, please attach a link to your repository to [contact@cruzhacks.com](mailto:contact@cruzhacks.com) with the subject line `firstLastname Dev Challenge` in the same email

Good luck and we'll get back to you all a few weeks after the deadline!

If you ever have questions or need help, please reach out to us at [contact@cruzhacks.com](mailto:contact@cruzhacks.com).
