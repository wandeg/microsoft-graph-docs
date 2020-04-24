---
title: "Update evaluateLabelJobs"
description: "Update the properties of an evaluateLabelJobs object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update evaluateLabelJobs

Namespace: microsoft.graph

Update the properties of an evaluateLabelJobs object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /dataClassification/evaluateLabelJobs
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [jobResponseBase](../resources/jobresponsebase.md) object.

The following table shows the properties that are required when you create the [jobResponseBase](../resources/jobresponsebase.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|type|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|error|[classificationError](../resources/classificationerror.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [jobResponseBase](../resources/jobresponsebase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_evaluatelabeljobs"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/evaluateLabelJobs
Content-Type: application/json
Content-length: 844

{
  "@odata.type": "#microsoft.graph.jobResponseBase",
  "type": "Type value",
  "status": "Status value",
  "tenantId": "Tenant Id value",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:57:05.4991702+03:00",
      "clientRequestId": "Client Request Id value",
      "activityId": "Activity Id value"
    },
    "details": [
      {
        "@odata.type": "microsoft.graph.classifcationErrorBase"
      }
    ]
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.jobResponseBase",
  "id": "b0cd238f-238f-b0cd-8f23-cdb08f23cdb0",
  "type": "Type value",
  "status": "Status value",
  "tenantId": "Tenant Id value",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:57:05.4991702+03:00",
      "clientRequestId": "Client Request Id value",
      "activityId": "Activity Id value"
    },
    "details": [
      {
        "@odata.type": "microsoft.graph.classifcationErrorBase"
      }
    ]
  }
}
```

