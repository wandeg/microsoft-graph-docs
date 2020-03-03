---
title: "Update exactMatchLookupJob"
description: "Update the properties of a exactMatchLookupJob object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update exactMatchLookupJob

Update the properties of a [exactMatchLookupJob](../resources/exactmatchlookupjob.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.graph.exactMatchLookupJob not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [exactMatchLookupJob](../resources/exactMatchLookupJob.md) object.

The following table shows the properties that are required when you create the [exactMatchLookupJob](../resources/exactmatchlookupjob.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactMatchJobBase.md)|
|startDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactMatchJobBase.md)|
|lastUpdatedDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactMatchJobBase.md)|
|completionDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactMatchJobBase.md)|
|error|[classificationError](../resources/classificationError.md)| Inherited from [exactMatchJobBase](../resources/exactMatchJobBase.md)|
|state|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [exactMatchLookupJob](../resources/exactmatchlookupjob.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_exactmatchlookupjob"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.exactMatchLookupJob not found
Content-type: application/json
Content-length: 856

{
  "@odata.type": "#microsoft.graph.exactMatchLookupJob",
  "creationDateTime": "2017-01-01T00:00:59.0982804+03:00",
  "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
  "lastUpdatedDateTime": "2017-01-01T00:01:04.1563754+03:00",
  "completionDateTime": "2017-01-01T00:02:23.013137+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2017-01-01T00:03:21.298689+03:00",
      "clientRequestId": "Client Request Id value",
      "activityId": "Activity Id value"
    },
    "details": [
      {
        "@odata.type": "microsoft.graph.classifcationErrorBase"
      }
    ]
  },
  "state": "State value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 905

{
  "@odata.type": "#microsoft.graph.exactMatchLookupJob",
  "id": "c31ee9fd-e9fd-c31e-fde9-1ec3fde91ec3",
  "creationDateTime": "2017-01-01T00:00:59.0982804+03:00",
  "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
  "lastUpdatedDateTime": "2017-01-01T00:01:04.1563754+03:00",
  "completionDateTime": "2017-01-01T00:02:23.013137+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2017-01-01T00:03:21.298689+03:00",
      "clientRequestId": "Client Request Id value",
      "activityId": "Activity Id value"
    },
    "details": [
      {
        "@odata.type": "microsoft.graph.classifcationErrorBase"
      }
    ]
  },
  "state": "State value"
}
```

