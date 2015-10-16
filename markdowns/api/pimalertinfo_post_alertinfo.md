# Create PimAlertInfo

Use this API to create a new PimAlertInfo.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /AlertInfo/

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
In the request body, supply a JSON representation of [PimAlertInfo](../resources/pimalertinfo.md) object.


### Response
If successful, this method returns `201, Created` response code and [PimAlertInfo](../resources/pimalertinfo.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_pimalertinfo_from_alertinfo"
}-->
```http
POST /AlertInfo/
Content-type: application/json
```
In the request body, supply a JSON representation of [PimAlertInfo](../resources/pimalertinfo.md) object.
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "pimalertinfo"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 370
{
  "AlertId": "AlertId-value",
  "AlertName": "AlertName-value",
  "AlertDescription": "AlertDescription-value",
  "LowSeverityThreshold": 99,
  "MediumSeverityThreshold": 99,
  "HighSeverityThreshold": 99,
  "Type": 99,
  "Severity": 99,
  "SecurityImpact": "SecurityImpact-value",
  "MitigationSteps": "MitigationSteps-value",
  "HowToPrevent": "HowToPrevent-value"
}
```

<!-- uuid: cd0ac6e4-5839-4305-8515-4bc3c3d16c47
2015-10-16 09:34:37 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create PimAlertInfo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->