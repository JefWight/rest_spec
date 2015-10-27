# Create Event

Use this API to create a new Event.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/CalendarView
POST /Users/<Id>/CalendarView

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply a JSON representation of [Event](../resources/event.md) object.


### Response
If successful, this method returns `201, Created` response code and [Event](../resources/event.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://outlook.office.com/v1.0/me
```
In the request body, supply a JSON representation of [Event](../resources/event.md) object.
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2080

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->