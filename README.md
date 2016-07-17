# Pokemon go REST API Documentation
The Pokemon go REST API was created so that all apps/programs could access one universal API. Currently, the API only supports getting information about player and collecting an authentication token. In the future finding pokestops, gyms and moving the player will be possible. Google authentication is also planned.
# Auth:
Currently, the API only supports auth via Pokemon trainer club, this is done via basic auth in all requests.
An example of this is:
`username:password@pokemongoapi.app/api/gettoken`
This gets an authentication token from Nintendo with the PTC username 'username' and password 'password'
# Endpoints:

There are currently only two API endpoints (expect many more in the immediate future)
### Auth Token
Get authentication token from the server:

Send a GET request to with authentication headers to:

`http://pokemongoapi.app/api/gettoken`

This will return an authentication token from the Pokemon go servers

Example response:

`{"token":"TGT-4078970-GBgGIN**************usnc7DXlIl5c4IQkAbSGskETZ6fMm-sso.pokemon.com"}`

### Profile information

Getting a players profile information:

`http://pokemongoapi.app/api/profile`

Example response:

`{"token":"TGT-4078970-GBgGIN**************usnc7DXlIl5c4IQkAbSGskETZ6fMm-sso.pokemon.com","endpoint":"https://pgorelease.nianticlabs.com/plfe/254/rpc","username":"fr0th13","storage":250,"istorage":350,"stardust":100,"pokecoins":null}`



More coming soon...


