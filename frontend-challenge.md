# CruzHacks 2023 Frontend Engineering Challenge

Engineers work closely with our UX/UI designers to develop interfaces that are visually appealing and accessible to users.

For this challenge you will be developing a mock of the following website. We have designed a mockup [here](https://www.figma.com/file/CJf6HOwmk8kFCPr0pUanyf/CruzHacks-Frontend-Challenge-2023?node-id=0%3A1) for you to use.
While a design is given, you may take creative liberties wherever you see fit during this challenge. Don't worry about mimicking every detail but we want to see your ability to replicate styles through jsx and css.

## Notes

Any updates, general questions, and additional notes will be listed here and I will update this section throughout the challenge. While unrealistic for any changes in the challenge description or visual design, if there are changes don't worry if your application is based on older specifications.

____
### FAQ

____
### Updates
____

## API Schema And Endpoint

The Schedule will be requested from a [RESTful API](https://www.codecademy.com/articles/what-is-rest) that retrieves data from a "database".

You'll be retrieving data via HTTP GET requests to this endpoint. The endpoint for the API is `https://cruzhacks23-organizer-endpoint.herokuapp.com/api/schedule`.

**Sample Response**:

```json
{
    "statusCode": 200,
    "message": "OK",
    "count": 3,
    "results": [
      {
        "date": "Friday, January 13, 2023",
        "events": [
          { "name": "Swag Distribution Starts", "time": "3:00 PM", "clickable": false },
          { "name": "Event Begins", "time": "5:00 PM", "clickable": false },
          { "name": "Swag Distribution Ends", "time": "", "clickable": false },
          { "name": "Opening Ceremony", "time": "7:00 PM", "clickable": false },
          { "name": "Hacking Begins", "time": "9:00 PM", "clickable": false },
          { "name": "Resume/Cover Letter", "time": "10:00 PM", "clickable": true },
          { "name": "MLH Event: Bob Ross Painting", "time": "", "clickable": true },
          { "name": "Equity In Tech", "time": "10:45 PM", "clickable": true },
        ],
      },
      {
        "date": "Saturday, January 14, 2023",
        "events": [
          {
            "name": "Adding a Backend and Database to Your App in 3 Lines",
            "time": "9:00 AM",
            "clickable": false
          },
          { "name": "Intro to Algorithm / Applications", "time": "10:00 AM", "clickable": true },
          { "name": "Tech Interviews", "time": "", "clickable": true },
          { "name": "Intro to Github", "time": "11:00 AM", "clickable": true },
          { "name": "Swag Distribution Starts", "time": "", "clickable": false },
          { "name": "What Could Go Wrong", "time": "", "clickable": true },
          { "name": "Basics of HTML", "time": "12:00 PM", "clickable": true },
          { "name": "Intro to UI Design", "time": "1:00 PM", "clickable": true },
          { "name": "Android Development", "time": "2:00 PM", "clickable": true },
          { "name": "Swag Distribution Ends", "time": "", "clickable": false },
          { "name": "Intro to Python", "time": "3:00 PM", "clickable": true },
          { "name": "Intro to React", "time": "4:00 PM", "clickable": true },
          { "name": "Environmental Innovation Guided Discussion", "time": "", "clickable": true },
          { "name": "MLH Event: Security Challenge", "time": "5:30 PM", "clickable": true },
        ],
      },
      {
        "date": "Sunday, January 15, 2023",
        "events": [
          { "name": "Project Submissions", "time": "10:00 AM", "clickable": false },
          { "name": "Judging Begins", "time": "11:30 AM", "clickable": false },
          { "name": "Closing Ceremony", "time": "2:00 PM", "clickable": false },
          { "name": "End of Event", "time": "4:00 PM", "clickable": false },
        ],
      },
    ]
}
```
Where date refers to the date of event, events refer to all events in that day at a given time and clickable denotes a workshop that one can register for.

You may expect the data returned from your fetch will remain the same each time. **Please Note** The endpoint is rate-limited and will only fulfill **100** requests per **15 minute** window.

## Schedule Component

Our goal is to create a schedule component for the day of event that will allow hackers to register for workshop events. The schedule data shall be retrieved from the endpoint provided above. Notice the json field titled 'clickable'. This is a boolean value denoting whether or not one will be able to register to the event. The schedule should render in chronological order and function with a forward and back button. If the event is clickable, the user should be able to click the title of the event and fill out a form to register to the event. While in reality we would like to exclude the functionality of event registration from the general public and include it for authenticated users; for the purpose of this challenge a simple form will suffice. Refer to [this schema](https://docs.google.com/document/d/1GNlmQF0WM7WvYZaqTvRlzzYtBcdeIh5jNqP-TZhTYl4/edit?usp=sharing) for the registration fields and input constraints. When dealing with any integration between a client and server it is important that we validate data on both the client and the server. 

We won't be integrating a backend into our application but we do want to see what the data of the form is. Please include either a state that renders the json or log the form data to the console. The rest of the submission functionality such as changing pages/states can be stubbed to whatever you see fit.
  

### Technologies

In previous years we have used [ReactJS](https://reactjs.org/docs/thinking-in-react.html) for our frontend. We will be using React again this year so we **Very Strongly Recommend** that this challenge should be completed using ReactJS (Javascript or Typescript). Please make use of the component based architecture to design scalable code.


### Responsiveness

People access our website on a variety of devices— phones, laptops, and desktops all have vastly different screen sizes, and we'd like to deliver seamless user experiences consistently. We need our application to have an intuitive interface for all screen sizes. Here's a [guide to help with that in the context of CSS](https://www.freecodecamp.org/news/how-to-start-thinking-responsively/).


### Documentation 

Documentation is extremely important as we are designing applications that should be able to used for future development teams. Your code should be easy to read so consistent naming conventions, comments in your code, and modularity are needed. Please include, in a README, thorough instructions on how to run your application, response schemas, why did you design your application the way you did, what went well, what didn't go well, and what things you could have done better.

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



