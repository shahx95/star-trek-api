# Star Trek API: 

A repository storing a read only Star Trek API.   

![Star Trek logo](https://i.imgur.com/JNUTLus.jpeg "Star Trek API")

## Tech Used:
HTML, Node.js, Express, GitHub and Heroku

## API Information:

API returns details about the species in the Star Trek eco-system. 

Previously, the API was using hard coded json data of Star Trek species. If a species was not found, the API returned data for Humans. 

Now the API uses data from a MangoDB database for Star Trek species. At the moment, the MongoDB database is populated with Vulcans, Klingons, Romulans, Borg, Gorn, Trill and Humans. If a species is not found, the API does not return anything.

 
## Give It A Try:

Global host name: `http://got-star-trek.herokuapp.com/`

Route: `/api/{query}`

**Example:**

Route: `/api/vulcans`

Returns:
```
{
    "_id":"62a21dc3175956eabc05d6ef",
    "name": "vulcans",
    "speciesName": "Vulcans",
    "homeworld": "Vulcan",
    "features": "Pointed ears, upward-curving eyebrows",
    "interestingFact": "Practice an extreme form of emotional regulation that focuses on logic above all else, pioneered by a Vulcan named Surak",
    "notableExamples": "Spock, T'Pol, Sarek",
    "image": "https://static.wikia.nocookie.net/aliens/images/7/75/Vulcans-FirstContact.jpg"
}
```

## Installation:

- Clone the repository
- Run `npm install`
- Provide ID and password for your MangoDB database

## Usage:

- Run `node server.js`
- Go to http://localhost:8000/ in a web browser
- Make a GET request to http://localhost:8000/api/{query}, replacing `{query}` with the case-insensitive name of a species to obtain its information.


## Optimization:

The API has been updated by connecting it to a database, but at the moment it is unable to serve a user friendly response for values not in the database. This should be improved in the future. Right now it is focusing on the species in Star Trek. In the future, API's scope can be expanded by adding data for individual characters, series, starships, planets and more. 
## More:

The API has been used in the [Star Trek Finder](https://github.com/shahx95/star-trek-client)  project.  

