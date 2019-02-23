# CruzHacks 2020 Frontend Engineering Team Coding Challenge

Front-End engineers work closely with our UX/UI designers to develop effective user interfaces that delight and empower users. In this scenario, you're tasked with developing a hacker sign in dashboard for organizers.

On the first day of the hackathon, it's essential for the organizing team to know how many hackers have signed in. Other relevant information includes how many hackers have signed in who have dietary preferences, physical handicaps, or any other necessary accommodations.

Data will be retrieved from a Hacker API that retrieves data from a hacker database. Your responsibility will be to develop a web page that receives data from the Hacker API and displays that data in a clear, actionable format to organizers.
API Schema
You'll be retrieving data via HTTP GET requests to this endpoint. Remember, it might not be important to display all the data about each hacker. Use your discretion.

## API SCHEMA AND ENDPOINT

The endpoint for the hacker API is `https://cruzhacks-2020-demo-hacker-api.azurewebsites.net/api/`

**Sample Response**:

`GET https://cruzhacks-2020-demo-hacker-api.azurewebsites.net/api/101`

```json
{
  "code": 200,
  "count": 1,
  "results": [
    {
      "_id": "5c7079d20cdc2a302145457d",
      "index": 101,
      "isCheckedIn": false,
      "age": 23,
      "name": "Tommie Meyer",
      "email": "WinifredBall@college.edu",
      "phone": "+1 (813) 405-3266",
      "physicalAccommodations": false,
      "dietaryAccommodations": false
    }
  ]
}
```

## Design Considerations

Organizers are extremely busy during registration. Thus data and visualizations must be straightforward to access and understand.
While a design mockup is given, you can take creative liberties to customize as you see fit. So don't worry about following the mockup precisely since there's a chance you could come up with a superior design. That said, don't deviate too much.

(Optional): It could prove valuable to have a section that displays the name and information for each signed in hacker. Since the number of signed in hackers could be in the hundreds, you'd want to use pagination to cycle through pages. If you opt not to use pagination, display the first ten hackers.

[Design Mockup](./Front-End-Challenge-Mockup.png)

## Technologies

You can use any technologies you’re comfortable with for this project as long as dependencies are explicitly specified and setup is minimal. Our team will be using ReactJS.

The Github repo should include a readme with instructions on how to run your project.
