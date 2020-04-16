# CruzHacks 2021 Frontend Engineering Challenge

Engineers work closely with our UX/UI designers to develop interfaces that delight and empower users.

In this scenario, you're tasked with developing a dashboard that hackers can use to view announcements & register for the hackathon. The designers have conjured a mockup [here](https://www.figma.com/file/pxkqgNnVvLCZrvBP6no7Jr/Cruzhacks-Frontend-Challenge?node-id=0%3A1).
While a design mockup is given, you may take creative liberties as you see fit during this challenge. We don't always need a pixel-perfect recreation of the mockup; rather, focus on delivering a seamless user experience!

## Announcements

Annoucements will be requested from a [RESTful API](https://www.codecademy.com/articles/what-is-rest) that retrieves data from a database.

### API Schema And Endpoint

You'll be retrieving data via HTTP GET requests to this endpoint. The endpoint for the API is `https://us-central1-cruzhacks-test-challenge-65ccc.cloudfunctions.net/getDB`

**Sample Response**:

`curl https://us-central1-cruzhacks-test-challenge-65ccc.cloudfunctions.net/getDB`

```json
{
  "code": 200,
  "count": 2,
  "results": [
    "uniqueIndex1" : {
      "datetime": "11/30/2019 08:16:28",
      "annoucement": "Check out our pre-hack workshops via Zoom!"
    },
    "uniqueIndex2" : {
      "datetime": "11/19/2019 14:15:31",
      "annoucement": "Hacker application now open! Scroll below."
    },
  ]
}
```

## Application Form

The application form consists of three [conditionally-rendered](https://reactjs.org/docs/conditional-rendering.html) pages, which contain input fields to pass data through. 

[It's important to validate the **type** & **size** of any form data for practical and security reasons.](https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation#What_is_form_validation) Refer to [this schema](https://docs.google.com/document/d/1gPo9_31LTOIkPMnFt-n4zWBOg7HsOB-yEDPmuAKsM6I/edit?usp=sharing) for user input constraints.

Since we don't have a registration API available yet, [stub](https://en.wikipedia.org/wiki/Method_stub) the submit/save functionality. Focus on having well-tested form validation & submission!

## Design Considerations
  
### Responsiveness

People access our website on a variety of devices— phones, laptops, and desktops all have vastly different screen sizes, and we'd like to deliver seamless user experiences consistently. It can be a trip conceptualizing how a website metamorphoses from a phone screen to an ultrawide monitor; here's a [guide to help with that in the context of CSS](https://www.freecodecamp.org/news/how-to-start-thinking-responsively/).

### Accessibility

Inclusivity is a core mission statement at CruzHacks, which is echoed in our design goals. People interact with the Internet through many ways that are not limited to a mouse, keyboard, touchscreen, or monitor. Thankfully, [standardized solutions](https://reactjs.org/docs/accessibility.html) exist to facilitate different methods of human-computer interaction.

[Here's a guide to accessability in the context of an HTML form.](https://itnext.io/form-accessibility-a-practical-guide-4062b7e2dd14)

## Technologies

We will be using [ReactJS](https://reactjs.org/docs/thinking-in-react.html), a Javascript library that enables powerful [component-based web development](https://reactjs.org/docs/components-and-props.html) by abstracting away raw HTML/CSS. Please take this opportunity to familiarize yourself with this highly in-demand user interface builder!

ReactJS supports [Jest](https://jestjs.io/), a testing framework that can [mock functions](https://jestjs.io/docs/en/mock-functions.html) and run [unit tests](https://en.wikipedia.org/wiki/Unit_testing). [Here's a guide on using Jest and Enzyme](https://dzone.com/articles/unit-testing-in-reactjs-using-jest-and-enzyme) to write a test suite! Enzyme is a companion that enables thorough testing of React components. [See how Enzyme and Jest complement one another here.](https://medium.com/codeclan/testing-react-with-jest-and-enzyme-20505fec4675)

## Submission

All done?! Don't worry if you can't meet every guideline outlined here; we just want to see what you can do! You will have the opportunity to learn more & hone your skills if you show commitment throughout this challenge.

To send us your ReactJS implementation:

* Create a public Github repo to host your React project. [If you're unfamiliar with Git, this will get you running.](https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/)
* Email a link of your repo to [contact@cruzhacks.com](mailto:contact@cruzhacks.com) with the subject line `CruzHacks Challenge - Last, First`
  * If you are also attempting the backend challenge, please attach a link to that second repository in the same email.
  
We'll get back to you all a few weeks after the deadline!
If you ever have questions or need help, please reach out to us at [contact@cruzhacks.com](mailto:contact@cruzhacks.com).
