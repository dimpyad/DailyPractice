## Learning Goal
OAuth2 - Scopes

### Problem Statement
Craete a new app in Spotify and connect to the app using Authorization Code Flow and Client Credentials Flow from your automation script.

### Presetup
- Create a developer account in spotify - https://developer.spotify.com/
- Explore the authorization flows listed at https://developer.spotify.com/documentation/general/guides/authorization/
- Create an sample app 
- Copy the secrets needed (like client credentials/secrets etc)

### Automation Script
- Connect to spotify App from your automation script using the following two methods and generate the access tokem
  1) Authorization Code Flow 
  2) Client Credentials Flow
- After successful authorization get the list of markets where spotify is available using the access token generated in the first step.  (https://developer.spotify.com/documentation/web-api/reference/#/operations/get-available-markets)
