# CruzHacks 2021 Frontend Engineering Challenge

Engineers work closely with our UX/UI designers to develop user interfaces that delight and empower users. 


In this scenario, you're tasked with developing a dashboard that hackers can use to view announcements & register for the hackathon. The designers have conjured a mockup [here](https://www.figma.com/file/pxkqgNnVvLCZrvBP6no7Jr/Cruzhacks-Frontend-Challenge?node-id=0%3A1).
We don't need a pixel-perfect recreation of the mockup; rather, focus on delivering a seamless user experience!


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
      "datetime": "11/30/2019",
      "annoucement: "Check out our pre-hack workshops via Zoom!"
    },
    {
      "datetime": "11/19/2019",
      "annoucement: "Hacker application now open! Scroll below."
    },
  ]
}
```

## Application Form

# [REWRITING]




## Design Considerations

Organizers are extremely busy during registration. Thus data and visualizations must be straightforward to access and understand.
While a design mockup is given, you can take creative liberties to customize as you see fit. So don't worry about following the mockup precisely since there's a chance you could come up with a superior design. That said, don't deviate too much.

(Optional): It could prove valuable to have a section that displays the name and information for each signed in hacker. Since the number of signed in hackers could be in the hundreds, you'd want to use pagination to cycle through pages. If you opt not to use pagination, display the first ten hackers.

[Design Mockup](./Front-End-Challenge-Mockup.png)

## Technologies

You can use any technologies you’re comfortable with for this project as long as dependencies are explicitly specified and setup is minimal. Our team will be using ReactJS.

The Github repo should include a readme with instructions on how to run your project.
