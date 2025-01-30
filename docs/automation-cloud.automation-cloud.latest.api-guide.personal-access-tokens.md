https://docs.uipath.com/automation-cloud/automation-cloud/latest/api-guide/personal-access-tokens

* Personal Access Tokens (PATs)
  * == unique alphanumeric string /
    * 👀-- REPLACEMENT of -- your username & password 👀
      * == MORE SECURE
    * limited expiration date -- can be -- set
  * allow you to
    * access 
      * UiPath
        * services
        * resources
      * grained == SPECIFIC defined != ALL
        * == Token scopes
          * _Example:_ `OR.Folders` - allows reading folder data, creating, modifying, and managing folders | Orchestrator
  * use case
    * -- interacting with -- our APIs and services
  * requirements
    * local users 
      * ⚠️!= directory users or SAML ⚠️
  * [how to generate a token?](https://docs.uipath.com/automation-cloud/automation-cloud/latest/api-guide/personal-access-tokens#generating-a-token)
  * [how to revoke a token?](https://docs.uipath.com/automation-cloud/automation-cloud/latest/api-guide/personal-access-tokens#revoking-a-token)
    * ⚠️once you revoke -> PAT have validity +1 EXTRA hour ⚠️
      * Reason: 🧠Orchestrator's caching mechanism 🧠
  * [how to regenerate a token?](https://docs.uipath.com/automation-cloud/automation-cloud/latest/api-guide/personal-access-tokens#token-regeneration)
    * requirements
      * ⚠️valid ONLY | PAT / have NOT YET expired ⚠️
    * ⚠️-> update the application / script ... / use it ⚠️
  
