https://docs.uipath.com/automation-cloud/automation-cloud/latest/api-guide/authentication-methods

* Personal Access Tokens
  * == secure bridge between your applications -- & -- OUR  API 
  * use cases
    * individual users / -- access programmatically to -- our platform
      * scripts,
      * automated tasks,
      * small-scale integrations 
  * how can it be managed?
    * users can 
      * generate them -- through -- their user preferences
      * enable fine-grained control -- over the -- data

* OAuth 2.0 for External Apps
  * == External apps can -- via obtaining client credentials, -- register with us
    * facilitates secure authorization / WITHOUT exposing user credentials
  * use case
    * third-party applications / seeking access | our platform -- on behalf of -- users
      * larger integrations / access MULTIPLE users' data
      * applications / access MULTIPLE users' data 

* API Keys
  * == simple way to authenticate requests
  * use cases
    * resources or scenarios / WITHOUT fine-grained control 
      * Reason: 🧠key -- is associated with -- SOME endpoints 🧠
  * ⚠️ from April 2025, deprecated ⚠️
