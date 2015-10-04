# Authentication

In order to be able to make requests to the Derocku API, you should first obtain an ApiKey for your account. For this, log into Derocku, click on the menu on the upper right corner of the screen, select `Account` info and then select `Api Key`.

## REST API

The Derocku REST API is reachable through the following hostname:

`https://dashboard.derocku.io/`

All requests should be sent to this endpoint with the following `Authorization` header:

`Authorization: ApiKey username:apikey`

HTTP responses are given in JSON format, so the following `Accept` header is required for every API call:

`Accept: application/json`

<aside class="notice">
You must replace <code>apikey</code> with your personal API key.
</aside>

```http
GET /api/v1/service/ HTTP/1.1
Host: dashboard.derocku.co
Authorization: ApiKey username:apikey
Accept: application/json
```

```shell
derocku login -u username -p apikey
```

> Make sure to replace **username** with your username and **apikey** with your API key
