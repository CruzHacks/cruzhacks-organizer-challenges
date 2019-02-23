# CruzHacks 2020 Backend Engineering Team Coding Challenge

In this exercise, we’re asking you to create a simple REST API with a technology of your choice. You are free to use any database: PostgreSQL, MySQL, MongoDB, etc.

**NOTE**: We prefer JavaScript or Python based API’s using Express + Node or Flask respectively.

Your task is to create a series of API endpoints that perform basic [CRUD (Create, Read)](https://www.w3schools.com/tags/ref_httpmethods.asp) operations for a simple hacker model. The hacker model is an object that contains information about hackers attending CruzHacks 2020. You're only expected to build a model supporting GET and POST request. Adding PUT and DELETE is optional.

You are free to include fields you think are relevant, but be sure to consider important things like age, school, major, etc. Use your best intuition when designing what data might be in this model.

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
