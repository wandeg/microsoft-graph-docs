---
title: "Update exactMatchLookupJob"
description: "Update the properties of a exactMatchLookupJob object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update exactMatchLookupJob

Namespace: microsoft.graph

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
In the request body, supply a JSON representation for the [exactMatchLookupJob](../resources/exactmatchlookupjob.md) object.

The following table shows the properties that are required when you create the [exactMatchLookupJob](../resources/exactmatchlookupjob.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|startDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|lastUpdatedDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|completionDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|error|[classificationError](../resources/classificationerror.md)| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
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
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.exactMatchLookupJob not found
Content-type: application/json
Content-length: 858

{
  "@odata.type": "#microsoft.graph.exactMatchLookupJob",
  "creationDateTime": "2017-01-01T00:02:11.4839005+03:00",
  "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
  "lastUpdatedDateTime": "2016-12-31T23:57:46.2985547+03:00",
  "completionDateTime": "2016-12-31T23:56:58.8026209+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:59:22.9712113+03:00",
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
Content-Length: 907

{
  "@odata.type": "#microsoft.graph.exactMatchLookupJob",
  "id": "c5506bf3-6bf3-c550-f36b-50c5f36b50c5",
  "creationDateTime": "2017-01-01T00:02:11.4839005+03:00",
  "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
  "lastUpdatedDateTime": "2016-12-31T23:57:46.2985547+03:00",
  "completionDateTime": "2016-12-31T23:56:58.8026209+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:59:22.9712113+03:00",
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

