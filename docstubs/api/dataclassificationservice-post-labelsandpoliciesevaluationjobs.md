---
title: "Add labelsAndPoliciesEvaluationJobs"
description: "Add labelsAndPoliciesEvaluationJobs by posting to the labelsAndPoliciesEvaluationJobs collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add labelsAndPoliciesEvaluationJobs

Namespace: microsoft.graph

Add labelsAndPoliciesEvaluationJobs by posting to the labelsAndPoliciesEvaluationJobs collection.

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
POST /dataClassification/labelsAndPoliciesEvaluationJobs/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [jobResponseBase](../resources/jobresponsebase.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_jobresponsebase_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/labelsAndPoliciesEvaluationJobs
Content-type: application/json
Content-length: 845

{
  "@odata.type": "#microsoft.graph.jobResponseBase",
  "type": "Type value",
  "status": "Status value",
  "tenantId": "Tenant Id value",
  "creationDateTime": "2017-01-01T00:02:15.7719196+00:00",
  "startDateTime": "2017-01-01T00:03:21.9189713+00:00",
  "endDateTime": "2016-12-31T23:58:18.8006039+00:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:58:19.2996819+00:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.jobresponsebase"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 894

{
  "@odata.type": "#microsoft.graph.jobResponseBase",
  "id": "91a91127-1127-91a9-2711-a9912711a991",
  "type": "Type value",
  "status": "Status value",
  "tenantId": "Tenant Id value",
  "creationDateTime": "2017-01-01T00:02:15.7719196+00:00",
  "startDateTime": "2017-01-01T00:03:21.9189713+00:00",
  "endDateTime": "2016-12-31T23:58:18.8006039+00:00",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "Code value",
    "message": "Message value",
    "target": "Target value",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "2016-12-31T23:58:19.2996819+00:00",
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

