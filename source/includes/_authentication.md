# Authentication

> To authorize, use this code:

```shell
curl "https://ptchr-bdlease-hexon.dev/oauth/token"
  -X POST
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

`POST https://ptchr-bdlease-hexon.dev/oauth/token` 

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
grand_type | none | Set to client_credentials
client_id | none | Use the Client ID you received
client_secret | none | Use the Client Secret you received

### Response

In response to this call you'll receive an long lived access_token which can be used to access the resourced mentioned below.

<aside class="notice">
Make sure to replace with your client ID and secret
</aside>