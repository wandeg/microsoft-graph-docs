---
title: "List jobResponseBases"
description: "List properties and relationships of the jobResponseBase objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List jobResponseBases

Namespace: microsoft.graph

List properties and relationships of the [jobResponseBase](../resources/jobresponsebase.md) objects.

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
GET /dataClassification/jobs
GET /dataClassification/classifyFileJobs
GET /dataClassification/classifyTextJobs
GET /dataClassification/evaluateLabelJobs
GET /dataClassification/evaluateDlpPoliciesJobs
GET /dataClassification/labelsAndPoliciesEvaluationJobs
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [jobResponseBase](../resources/jobresponsebase.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_jobresponsebase"
}
-->
``` http
GET https://graph.microsoft.com/localtest/dataClassification/jobs
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
Content-Length: 1027

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.jobResponseBase",
      "id": "e3582e2c-2e2c-e358-2c2e-58e32c2e58e3",
      "type": "Type value",
      "status": "Status value",
      "tenantId": "Tenant Id value",
      "creationDateTime": "2017-01-01T00:02:11.4839005+03:00",
      "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
      "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
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
      }
    }
  ]
}
```

