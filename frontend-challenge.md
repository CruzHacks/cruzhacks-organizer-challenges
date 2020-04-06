# CruzHacks 2021 Frontend Engineering Challenge

Engineers work closely with our UX/UI designers to develop user interfaces that delight and empower users. 


In this scenario, you're tasked with developing a dashboard that hackers can use to view announcements & register for the hackathon. The designers have conjured a mockup [here](https://www.figma.com/file/pxkqgNnVvLCZrvBP6no7Jr/Cruzhacks-Frontend-Challenge?node-id=0%3A1).
While a design mockup is given, you may take creative liberties as you see fit during this challenge. We don't need a pixel-perfect recreation of the mockup; rather, focus on delivering a seamless user experience! 


## Announcements 
Annoucements will be requested from a [RESTful API](https://www.codecademy.com/articles/what-is-rest) that retrieves data from a database. 


### API Schema And Endpoint

You'll be retrieving data via HTTP GET requests to this endpoint. The endpoint for the API is `https://[firebase URL]/api/`

**Sample Response**:

`GET https://[firebase URL]/api/retrieve`

```json
{
  "code": 200,
  "count": 2,
  "results": [
    {
      "datetime": "11/30/2019 08:16:28",
      "annoucement: "Check out our pre-hack workshops via Zoom!"
    },
    {
      "datetime": "11/19/2019 14:15:31",
      "annoucement: "Hacker application now open! Scroll below."
    },
  ]
}
```

## Application Form
The application form consists of three [conditionally-rendered](https://reactjs.org/docs/conditional-rendering.html) pages. Since we don't have a registration API available yet, [stub](https://en.wikipedia.org/wiki/Method_stub) the submit/save functionality. Focus on having strong form validation & functional pagination!

Refer to [this schema](https://docs.google.com/document/d/1gPo9_31LTOIkPMnFt-n4zWBOg7HsOB-yEDPmuAKsM6I/edit?usp=sharing) for user input constraints. Don't forget to notify the user if an input field fails validation!

## Design Considerations

### Responsiveness

### Accessibility

# [REWRITING]

## Technologies

You can use any technologies you’re comfortable with for this project as long as dependencies are explicitly specified and setup is minimal. Our team will be using ReactJS.

The Github repo should include a readme with instructions on how to run your project.
