https://docs.uipath.com/orchestrator/automation-cloud/latest/user-guide/configuring-tenant-settings

* TODO:
* Robot Security Tab
  * TODO:
  * Authentication
    * unattended robot authentication
    * attended robot authentication
      * Interactive Sign-in SSO
        * 👀recommended 👀
        * requirements
          * robot connections / tokens can expire
        * == users MUST signing-in -- with -- their credentials | Assistant 
          * ⚠️if you want to run attended robots, make Orchestrator HTTP requests, or view processes | Assistant -> user MUST sign in ⚠️ 
        * ❌NO need -- to create -- machine objects | Orchestrator ❌
      * Hybrid
        * requirements
          * tokens / 
            * NOT expire (machine key)
            * expire ( == interactive sign-in or client credentials) 
        * OPTIONAL
          * users sign-in -- with -- their credentials
* TODO: