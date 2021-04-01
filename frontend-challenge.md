# CruzHacks 2021 Frontend Engineering Challenge

Engineers work closely with our UX/UI designers to develop interfaces that are visually appealing and accessible to users.

For this challenge you will be developing a mock of the following website. We have designed a mockup [here](https://www.figma.com/file/aayZoTtxjGVvMPrjnvUEEi/Cruzhacks-Frontend-Challenge-2022?node-id=0%3A1) for you to use.
While a design is given, you may take creative liberties wherever you see fit during this challenge. Don't worry about mimicing every detail but we want to see your ability to replicate styles through jsx and css.

## Notes

Any updates, general questions, and additional notes will be listed here and I will update this section throughout the challenge. While unrealistic for any changes in the challenge description or visual design, if there are changes don't worry if your application is based on older specifications.

____
### FAQ


### Updates


____

## API Schema And Endpoint

Annoucements will be requested from a [RESTful API](https://www.codecademy.com/articles/what-is-rest) that retrieves data from a database.

You'll be retrieving data via HTTP GET requests to this endpoint. The endpoint for the API is `https://cruzhacks22-organizer-endpoint.herokuapp.com/api/announcements`.

**Sample Response**:

```json
{
    "statusCode": 200,
    "message": "ok",
    "count": 3,
    "results": [
        {
            "description": "CruzHacks Applications are Out!",
            "link": "https://www.cruzhacks.com/",
            "dateTime": "11/1/2021 11:00 AM",
            "isLink": true
        },
        {
            "description": "Applications will close in a week, Have a Happy Thanksgiving!",
            "dateTime": "11/24/2021 08:30 PM",
            "isLink": false
        },
        {
            "description": "Applications are Closing Tonight! at 11:59PM",
            "link": "https://www.cruzhacks.com/",
            "dateTime": "12/1/2021 12:00 PM",
            "isLink": true
        }
    ]
}
```

We can assume description, dateTime, and isLink will always appear in every request. Link is an optional field and will appear in a response if isLink is true. Please try to account for situations where the response code is not successful and not 200, the count is 0, there are many results to render, and any issues causing slow fetches or failure to fetch.


## Application Form

Our goal is to create an application system that will allow both hackers and volunteers/mentors/judges to apply for CruzHacks. All applicants will have the general questions and depending on whether they inputted hacker or volunteer their next questions will be different. We want to make use of conditional rendering so we aren't showing questions that are unrelated to applicants.  When dealing with any integration between a client and server it is important that we validate data on both the client and the server. Refer to [this schema](https://docs.google.com/document/d/1gPo9_31LTOIkPMnFt-n4zWBOg7HsOB-yEDPmuAKsM6I/edit?usp=sharing) for the application fields and input constraints.

We won't be integrating a backend into our application but we do want to see what the data of the form is. Please include either a state that renders the json or log the form data to the console. The rest of the submission functionality such as changing pages/states can be stubbed to whatever you see fit.
  

### Technologies

In previous years we have used [ReactJS](https://reactjs.org/docs/thinking-in-react.html) for our frontend. We will be using React again this year so we **Very Strongly Recommend** that this challenge should be completed using ReactJS (Javascript or Typescript). Please make use of the component based architecture to design scalable code.


### Responsiveness

People access our website on a variety of devices— phones, laptops, and desktops all have vastly different screen sizes, and we'd like to deliver seamless user experiences consistently. We need our application to have an intuitive interface for all screen sizes. Here's a [guide to help with that in the context of CSS](https://www.freecodecamp.org/news/how-to-start-thinking-responsively/).


### Documentation 

Documentation is extremely important as we are designing applications that should be able to used for future development teams. Your code should be easy to read so consistent naming conventions, comments in your code, and modularity. Please include, in a README, thorough instructions on how to run your application, response schemas, why did you design your application the way you did, what went well, what didn't go well, and what things you could have done better.

## Submission

Finished? Don't worry if you can't meet every guideline, we just want to see what you can do! We don't expect you to have everything completed but we do hope that you are able to complete a good chunk of this challenge. You will have the opportunity to learn more & hone your skills if you show commitment throughout this challenge.

To send us your implementation:

* Create a Github repo to host your React project. [If you're unfamiliar with Git, this will get you running.](https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/)
* Create a zip of your application
* Email a link of your repo to [contact@cruzhacks.com](mailto:contact@cruzhacks.com) and cc [dev@cruzhacks.com] with the subject line `CruzHacks Challenge - Last, First`, or send us a zip of your code with the file called `Last_First_CruzHacks_Frontend.zip`.
    * Please include any .env information necessary to run the application
    * If you have any other sensitive files that should not be shared in a git repo add a file called `frontend_secrets.zip`

* If you are also attempting the backend challenge, please attach the other challenge in the same email.
  

We'll get back to you all a few weeks after the deadline!

If you ever have questions or need help, please reach out to us at [contact@cruzhacks.com](mailto:contact@cruzhacks.com).



