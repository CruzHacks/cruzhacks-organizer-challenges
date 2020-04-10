# CruzHacks 2021 Frontend Engineering Challenge

Engineers work closely with our UX/UI designers to develop user interfaces that delight and empower users. 


In this scenario, you're tasked with developing a dashboard that hackers can use to view announcements & register for the hackathon. The designers have conjured a mockup [here](https://www.figma.com/file/pxkqgNnVvLCZrvBP6no7Jr/Cruzhacks-Frontend-Challenge?node-id=0%3A1).
While a design mockup is given, you may take creative liberties as you see fit during this challenge. We don't need a pixel-perfect recreation of the mockup; rather, focus on delivering a seamless user experience! 


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
    "1" : {
      "datetime": "11/30/2019 08:16:28",
      "annoucement": "Check out our pre-hack workshops via Zoom!"
    },
    "2" : {
      "datetime": "11/19/2019 14:15:31",
      "annoucement": "Hacker application now open! Scroll below."
    },
  ]
}
```

## Application Form
The application form consists of three [conditionally-rendered](https://reactjs.org/docs/conditional-rendering.html) pages, which contain input fields to pass data through. 

[It's important to validate the type & size of any form control for practical and security reasons.](https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation#What_is_form_validation) Refer to [this schema](https://docs.google.com/document/d/1gPo9_31LTOIkPMnFt-n4zWBOg7HsOB-yEDPmuAKsM6I/edit?usp=sharing) for user input constraints. Don't forget to notify the user if an input field fails validation!

Since we don't have a registration API available yet, [stub](https://en.wikipedia.org/wiki/Method_stub) the submit/save functionality. Focus on having well-tested form validation & pagination!

## Design Considerations
  
### Responsiveness
People access our website on a variety of devices— phones, laptops, and desktops all have vastly different screen sizes, and we'd like to deliver seamless user experiences consistently. It can be a trip conceptualizing how a website metamorphoses from a phone screen to an ultrawide monitor; here's a [guide to help with that](https://www.freecodecamp.org/news/how-to-start-thinking-responsively/). Make sure your [HTML/CSS fundementals](https://www.theodinproject.com/courses/web-development-101/lessons/html-and-css-basics) are covered before you dive in.

### Accessibility
Inclusivity is a core mission statement at CruzHacks, which is echoed in our design goals. People interact with the Internet through many ways that are not limited to a mouse, keyboard, touchscreen, or monitor. Thankfully, [standardized solutions](https://reactjs.org/docs/accessibility.html) exist to facilitate different methods of human-computer interaction.

[Here's a guide to accessability in the context of an HTML form.](https://itnext.io/form-accessibility-a-practical-guide-4062b7e2dd14)

# [REWRITING]

## Technologies

You can use any technologies you’re comfortable with for this project as long as dependencies are explicitly specified and setup is minimal. Our team will be using ReactJS.

The Github repo should include a readme with instructions on how to run your project.
