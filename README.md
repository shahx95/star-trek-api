# Star Trek API: 

A repository storing a read only Star Trek API.   

![Star Trek logo](https://i.imgur.com/JNUTLus.jpeg "Star Trek API")

## Tech Used:
HTML, Node.js, Express, GitHub and Heroku

## API Information:

API returns details about the species in the Star Trek eco-system. The API uses hard coded json data for Star Trek species. Hard coded species include Vulcans, Klingons, Romulans, Borg, Gorn, Trill and Humans. If a species is not found, the API will return data for Humans. 
 
## Give It A Try:

Global host name: `http://got-star-trek.herokuapp.com/`

Route: `/api/{query}`

**Example:**

Route: `/api/vulcans`

Returns:
```
{
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

## Usage:

- Run `node server.js`
- Go to http://localhost:8000/ in a web browser
- Make a GET request to http://localhost:8000/api/{query}, replacing `{query}` with the case-insensitive name of a species to obtain its information.


## Optimization:

The API is currently focusing on the species in Star Trek. In the future, API's scope can be expanded by adding data for individual characters, series, starships, planets and more. The data could be migrated into a MongoDB database.
## More:

The API has been used in the [Star Trek Finder](https://github.com/shahx95/star-trek-client)  project.  

