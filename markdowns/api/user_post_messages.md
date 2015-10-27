# Create Message

Use this API to create a new Message.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/Messages
POST /Users/<Id>/Messages

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply a JSON representation of [Message](../resources/message.md) object.


### Response
If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://outlook.office.com/v1.0/me
```
In the request body, supply a JSON representation of [Message](../resources/message.md) object.
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1546

{
  "HasAttachments": true,
  "Subject": "Subject-value",
  "Body": {
    "ContentType": "ContentType-value",
    "Content": "Content-value"
  },
  "BodyPreview": "BodyPreview-value",
  "Importance": "Importance-value",
  "ParentFolderId": "ParentFolderId-value",
  "Sender": {
    "EmailAddress": {
      "Name": "Name-value",
      "Address": "Address-value"
    }
  },
  "From": {
    "EmailAddress": {
      "Name": "Name-value",
      "Address": "Address-value"
    }
  },
  "ToRecipients": [
    {
      "EmailAddress": {
        "Name": "Name-value",
        "Address": "Address-value"
      }
    }
  ],
  "CcRecipients": [
    {
      "EmailAddress": {
        "Name": "Name-value",
        "Address": "Address-value"
      }
    }
  ],
  "BccRecipients": [
    {
      "EmailAddress": {
        "Name": "Name-value",
        "Address": "Address-value"
      }
    }
  ],
  "ReplyTo": [
    {
      "EmailAddress": {
        "Name": "Name-value",
        "Address": "Address-value"
      }
    }
  ],
  "ConversationId": "ConversationId-value",
  "UniqueBody": {
    "ContentType": "ContentType-value",
    "Content": "Content-value"
  },
  "IsDeliveryReceiptRequested": true,
  "IsReadReceiptRequested": true,
  "IsRead": true,
  "IsDraft": true,
  "DateTimeReceived": "datetime-value",
  "DateTimeSent": "datetime-value",
  "WebLink": "WebLink-value",
  "ChangeKey": "ChangeKey-value",
  "Categories": [
    "Categories-value"
  ],
  "DateTimeCreated": "datetime-value",
  "DateTimeLastModified": "datetime-value",
  "Id": "Id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->