https://docs.uipath.com/orchestrator/automation-cloud/latest/api-guide/authorizing-api-calls-in-swagger

* Swagger authentication time life
  * by default, 30'
  * if you want to modify -> adjust `Auth.Cookie.Expire` | "Web.config" 

* How to obtain an Access Token?
  * click | "Authorize" button

* How to generate a NEW Access Token?
  * click | "Authorize" button
  * click | Logout
    * Reason: 🧠revoke previous credentials 🧠