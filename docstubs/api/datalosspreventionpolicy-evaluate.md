---
title: "evaluate"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# evaluate

Namespace: microsoft.graph



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
POST /informationProtection/dataLossPreventionPolicies/evaluate
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|target|String||
|evaluationInput|[dlpEvaluationInput](../resources/dlpevaluationinput.md)||
|notificationInfo|[dlpNotification](../resources/dlpnotification.md)||



## Response
If successful, this action returns a `200 OK` response code and a [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "datalosspreventionpolicy_evaluate"
}
-->
``` http
POST https://graph.microsoft.com/beta/informationProtection/dataLossPreventionPolicies/evaluate

Content-type: application/json
Content-length: 640

{
  "target": "Target value",
  "evaluationInput": {
    "@odata.type": "microsoft.graph.dlpEvaluationInput",
    "discoveredSensitiveTypes": [
      {
        "@odata.type": "microsoft.graph.discoveredSensitiveType",
        "id": "174827b3-27b3-1748-b327-4817b3274817",
        "count": 5,
        "confidence": 10
      }
    ],
    "currentLabel": {
      "@odata.type": "microsoft.graph.currentLabel",
      "id": "Id value",
      "applicationMode": "String"
    },
    "accessScope": "String"
  },
  "notificationInfo": {
    "@odata.type": "microsoft.graph.dlpNotification",
    "author": "Author value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dlpevaluatepoliciesjobresponse"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 586

{
  "value": {
    "@odata.type": "#microsoft.graph.dlpEvaluatePoliciesJobResponse",
    "id": "3d3dd919-d919-3d3d-19d9-3d3d19d93d3d",
    "type": "Type value",
    "status": "Status value",
    "tenantId": "Tenant Id value",
    "creationDateTime": "2016-12-31T23:57:30.6368517+03:00",
    "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
    "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
    "error": {
      "@odata.type": "microsoft.graph.classificationError"
    },
    "result": {
      "@odata.type": "microsoft.graph.dlpPoliciesJobResult"
    }
  }
}
```

