# List Events

Retrieve a list of event objects.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /me/Calendar/Events
GET /Users/<Id>/Calendar/Events
GET /me/Events/<Id>/Calendar/Events
```
### Optional query parameters
|Name|Value|Description|
|:---------------|:--------|:-------|
|$count|none|The count of related entities can be requested by specifying the $count query option.|
|$expand|string|Comma-separated list of relationships to expand and include in the response. See relationships table of [Event](../resources/event.md) for supported names. |
|$filter|string|Filter string that lets you filter the response based on a set of criteria.|
|$orderby|string|Comma-separated list of properties that are used to sort the order of items in the response collection.|
|$select|string|Comma-separated list of properties to include in the response.|
|$skip|int|The number of items to skip in a result set.|
|$skipToken|string|Paging token that is used to get the next set of results.|
|$top|int|The number of items to return in a result set.|

### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://outlook.office.com/v1.0/me/Calendar/Events
```
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2453

{
  "value": [
    {
      "ResponseStatus": {
        "Response": "Response-value",
        "Time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "Reminder": 99,
      "HasAttachments": true,
      "Subject": "Subject-value",
      "Body": {
        "ContentType": "ContentType-value",
        "Content": "Content-value"
      },
      "BodyPreview": "BodyPreview-value",
      "Importance": "Importance-value",
      "Sensitivity": "Sensitivity-value",
      "Start": "datetime-value",
      "OriginalStart": "datetime-value",
      "StartTimeZone": "StartTimeZone-value",
      "End": "datetime-value",
      "EndTimeZone": "EndTimeZone-value",
      "Location": {
        "DisplayName": "DisplayName-value",
        "Address": {
          "Street": "Street-value",
          "City": "City-value",
          "State": "State-value",
          "CountryOrRegion": "CountryOrRegion-value",
          "PostalCode": "PostalCode-value"
        },
        "Coordinates": {
          "Altitude": 99,
          "Latitude": 99,
          "Longitude": 99,
          "Accuracy": 99,
          "AltitudeAccuracy": 99
        }
      },
      "IsAllDay": true,
      "IsCancelled": true,
      "IsOrganizer": true,
      "Recurrence": {
        "Pattern": {
          "Type": "Type-value",
          "Interval": 99,
          "Month": 99,
          "DayOfMonth": 99,
          "DaysOfWeek": [
            "DaysOfWeek-value"
          ],
          "FirstDayOfWeek": "FirstDayOfWeek-value",
          "Index": "Index-value"
        },
        "Range": {
          "Type": "Type-value",
          "StartDate": "datetime-value",
          "EndDate": "datetime-value",
          "NumberOfOccurrences": 99
        }
      },
      "ResponseRequested": true,
      "SeriesMasterId": "SeriesMasterId-value",
      "ShowAs": "ShowAs-value",
      "Type": "Type-value",
      "Attendees": [
        {
          "Status": {
            "Response": "Response-value",
            "Time": "datetime-value"
          },
          "Type": "Type-value"
        }
      ],
      "Organizer": {
        "EmailAddress": {
          "Name": "Name-value",
          "Address": "Address-value"
        }
      },
      "WebLink": "WebLink-value",
      "ChangeKey": "ChangeKey-value",
      "Categories": [
        "Categories-value"
      ],
      "DateTimeCreated": "datetime-value",
      "DateTimeLastModified": "datetime-value",
      "Id": "Id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List Events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->