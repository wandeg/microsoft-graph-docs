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
  "creationDateTime": "2016-12-31T23:57:35.2754224+03:00",
  "startDateTime": "2016-12-31T23:57:07.1037922+03:00",
  "endDateTime": "2016-12-31T23:57:36.8091086+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2017-01-01T00:00:00.4847018+03:00",
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
  "id": "f13e7d7f-7d7f-f13e-7f7d-3ef17f7d3ef1",
  "type": "Type value",
  "status": "Status value",
  "tenantId": "Tenant Id value",
  "creationDateTime": "2016-12-31T23:57:35.2754224+03:00",
  "startDateTime": "2016-12-31T23:57:07.1037922+03:00",
  "endDateTime": "2016-12-31T23:57:36.8091086+03:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2017-01-01T00:00:00.4847018+03:00",
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

