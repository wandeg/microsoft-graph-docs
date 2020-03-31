---
title: "Update jobResponseBase"
description: "Update the properties of a jobResponseBase object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update jobResponseBase

Namespace: microsoft.graph

Update the properties of a [jobResponseBase](../resources/jobresponsebase.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /dataClassification/jobs/{jobResponseBaseId}
PATCH /dataClassification/classifyFileJobs/{jobResponseBaseId}
PATCH /dataClassification/classifyTextJobs/{jobResponseBaseId}
PATCH /dataClassification/evaluateLabelJobs/{jobResponseBaseId}
PATCH /dataClassification/evaluateDlpPoliciesJobs/{jobResponseBaseId}
PATCH /dataClassification/labelsAndPoliciesEvaluationJobs/{jobResponseBaseId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [jobResponseBase](../resources/jobresponsebase.md) object.

The following table shows the properties that are required when you create the [jobResponseBase](../resources/jobresponsebase.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|type|String||
|status|String||
|tenantId|String||
|creationDateTime|DateTimeOffset||
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|error|[classificationError](../resources/classificationerror.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [jobResponseBase](../resources/jobresponsebase.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_jobresponsebase"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/jobs/{jobResponseBaseId}
Content-type: application/json
Content-length: 845

{
  "@odata.type": "#microsoft.graph.jobResponseBase",
  "type": "Type value",
  "status": "Status value",
  "tenantId": "Tenant Id value",
  "creationDateTime": "2017-01-01T00:01:50.3140554+03:00",
  "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
  "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:58:13.2283886+03:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 894

{
  "@odata.type": "#microsoft.graph.jobResponseBase",
  "id": "324d1724-1724-324d-2417-4d3224174d32",
  "type": "Type value",
  "status": "Status value",
  "tenantId": "Tenant Id value",
  "creationDateTime": "2017-01-01T00:01:50.3140554+03:00",
  "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
  "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:58:13.2283886+03:00",
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

