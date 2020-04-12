# CruzHacks 2021 Backend Engineering Team Coding Challenge

In this exercise, we’re asking you to create a simple REST API that supports the application portal created in the front end challenge.  

**NOTE**: This year, we will be using Firebase to host and deploy our site and functions. We are asking all applicants to create and deploy their functions via [Firebase](https://firebase.google.com/).

## Challenge

Your task is to create a series of API endpoints that perform basic [CRUD (Create, Read, Update)](https://www.codecademy.com/articles/what-is-crud) operations for a simple hacker model. The hacker model is an object that contains information about hackers attending CruzHacks 2021. You are expected to create API endpoints that supports POST, PUT, and GET requests.

* POST will create a hacker object in your database
* PUT will update your hacker's data
* GET will retreieve that information and display it in your appliacation portal until it's been submitted.

## Database Schema

Your database schema should follow the application portal's fields. Form validation should be done client side, but fields inside each hacker object should have their respective constraints. Please refer to this [schema](https://docs.google.com/document/d/1gPo9_31LTOIkPMnFt-n4zWBOg7HsOB-yEDPmuAKsM6I/edit) when creating your database.

As mentioned, our team will be using Firebase this year, so we ask that your database also be hosted on Firebase as well. For the application portal, we will be using the [Cloud Firestore Database](https://firebase.google.com/docs/firestore).

Your completed program should be fully functional and provide appropriate responses when tested with actual API requests.

For example, the following request:

`curl -XGET -H ‘Content-Type: application/json’ http://localhost:300/hackers/1`

Might return json similar to:

```json
{
  "name": "John Doe",
  "id": 1,
  "email": "john@doe.com",
}
```

Keep in mind this is an example for one endpoint, your completed program should have enough endpoints that allow for full CRUD functionality on the hacker object.

The Github repo should include a readme with instructions on how to run your project.
