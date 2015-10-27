# Update user

Update the properties of user object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /me
PATCH /Users/<Id>
```
### Optional request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Alias|String|The user's alias. Typically the SMTP address of the user.|
|DisplayName|String|The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates.|
|MailboxGuid|Guid|The GUID assigned to the user's mailbox.|

### Response
If successful, this method returns a `200 OK` response code and updated [User](../resources/user.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PUT https://outlook.office.com/v1.0/me
Content-type: application/json
Content-length: 124

{
  "DisplayName": "DisplayName-value",
  "Alias": "Alias-value",
  "MailboxGuid": "MailboxGuid-value",
  "Id": "Id-value"
}
```
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->