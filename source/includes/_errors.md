# Status codes

The API uses the following HTTP status codes:

### Error codes (HTTP status codes)

Error Code | Meaning
---------- | -------
200 OK | The request was successful (optionally you may receive data in the body)
201 Created | The entity is successfully created, you should receive or data in the response
403 Forbidden | Access to the entity or round was denied
404 Not Found | The entity or route was not found in this API (or access was denied)

### Error messages

Error messages are send as response, they're always formatted like below. There may be more than just a single error.

```json
{
    "errors": {
        "advertiser_id": [
            "The advertiser id has already been taken."
        ],
        "name": [
            "The name field is required."
        ]
    }
}
```