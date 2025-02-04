https://docs.uipath.com/document-understanding/automation-cloud/latest/api-guide/using-the-credentials-with-the-external-application

* to get the `access_token`

  ```
  curl --data-urlencode "scope=Du.Digitization" 
  --data-urlencode "client_id={app_id}" 
  --data-urlencode "client_secret={app_secret}" 
  --data-urlencode "grant_type=client_credentials" https://cloud.uipath.com/identity_/connect/token
  ```

* | NEXT requests,
  * set `Authorization: Bearer access_tokenGotPreviousResponse`