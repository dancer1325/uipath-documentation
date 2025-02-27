https://docs.uipath.com/robot/standalone/latest/admin-guide/attended-automations

* Attended automations
  * 's goal
    * run | human supervision
  * use cases
    * tasks /
      * smaller, more fragmented 
        * _Example:_ submitting expense reports
          * _Example:_ once the user logs | system -> automation fill in necessary information, attach requested items & submit the report
      * require specific user access rights
        * == users -- MUST provide -- ALL those credentials
          * ❌if user has NOT access -> user gets unauthorized access ❌
        * Reasons: 🧠 ensure security 🧠
        * [here](https://docs.uipath.com/robot/standalone/latest/admin-guide/attended-automations#permissions-to-run-attended-automations)
  * 👀how -- is it related with -- Orchestrator ? 👀
    * Orchestrator -- ensures -- 
      * centralized management
      * correct delivery of package versions -- to -- robots
  * steps / attended automation -- can access to -- resources | Orchestrator folder
    * administrator 
      * -- adds the -- corresponding account (either a user or a robot account) | specific folder
      * -- gives permissions (/ required by the automation) to the -- account
  * TODO:
  * how to authenticate?
    * 👀Orchestrator -- verifies the -- UiPath Robot's identity 👀 
    * [ALLOWED methods](orchestrator.automation-cloud.latest.user-guide.configuring-tenant-settings.md)
      * interactive user sign-in (Service URL | Assistant)
      * hybrid 
        * == user sign-in + machine key connections 
    
      
