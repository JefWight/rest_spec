# Create User

Use this API to create a new User.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /Users

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply a JSON representation of [User](../resources/user.md) object.


### Response
If successful, this method returns `201, Created` response code and [User](../resources/user.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://outlook.office.com/v1.0/Users
```
In the request body, supply a JSON representation of [User](../resources/user.md) object.
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 124

{
  "DisplayName": "DisplayName-value",
  "Alias": "Alias-value",
  "MailboxGuid": "MailboxGuid-value",
  "Id": "Id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->