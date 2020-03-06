---
title: "List labelsAndPoliciesEvaluationJobs"
description: "Get the jobResponseBases from the labelsAndPoliciesEvaluationJobs navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List labelsAndPoliciesEvaluationJobs

Namespace: microsoft.graph

Get the jobResponseBases from the labelsAndPoliciesEvaluationJobs navigation property.

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
GET /dataClassification/labelsAndPoliciesEvaluationJobs
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [jobResponseBase](../resources/jobresponsebase.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_jobresponsebase"
}
-->
``` http
GET https://graph.microsoft.com/localtest/dataClassification/labelsAndPoliciesEvaluationJobs
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.jobresponsebase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1026

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.jobResponseBase",
      "id": "075a4843-4843-075a-4348-5a0743485a07",
      "type": "Type value",
      "status": "Status value",
      "tenantId": "Tenant Id value",
      "creationDateTime": "2016-12-31T23:59:35.5241957+03:00",
      "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
      "endDateTime": "2017-01-01T00:02:18.392989+03:00",
      "error": {
        "@odata.type": "microsoft.graph.classificationError",
        "code": "Code value",
        "message": "Message value",
        "target": "Target value",
        "innerError": {
          "@odata.type": "microsoft.graph.classificationInnerError",
          "errorDateTime": "2016-12-31T23:58:02.3445758+03:00",
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
  ]
}
```

