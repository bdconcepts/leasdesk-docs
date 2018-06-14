# Authentication

> To authenticate, use this code:

```shell
curl "https://staging.financial.leasedesk.nl/oauth/token"
  -X POST
  -H "Accept: application/json" 
  -d "grant_type=client_credentials&client_id=<your_client_id>&client_secret=<your_client_secret>"
```

> The above command returns JSON structured like this:

```json
{
    "token_type": "Bearer",
    "expires_in": 31536000,
    "access_token": "<your_access_token>"
}
```

Getting authorised to use the API is as easy as requesting an access token using the Client ID and Client Secret codes you were handed by us.

### HTTP Request

`POST https://staging.financial.leasedesk.nl/oauth/token` 

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
grant_type | none | Set to client_credentials
client_id | none | Use the Client ID you received
client_secret | none | Use the Client Secret you received

### Response

In response to this call you'll receive an long lived access_token which can be used to access the resourced mentioned below.

<aside class="notice">
Make sure to replace with your client ID and Client Secret with the ones for the correct environment.
</aside>

# Authorization

> Add these headers to each request:

```shell
curl "<api_endpoint_url>"
  -X METHOD
  -H "Accept: application/json" 
  -H "Authorization: Bearer <token>" 
```

To authorize each next request when using the API you have to add the access_token to the header of your request. Also make sure you send the "Accept: application/json" header, this header is used by our system to render errors within the system in json instead of serving HTTP responses containing HTML.