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
        "id": "54bef69d-f69d-54be-9df6-be549df6be54",
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
Content-Length: 585

{
  "value": {
    "@odata.type": "#microsoft.graph.dlpEvaluatePoliciesJobResponse",
    "id": "ab1b4f76-4f76-ab1b-764f-1bab764f1bab",
    "type": "Type value",
    "status": "Status value",
    "tenantId": "Tenant Id value",
    "creationDateTime": "2016-12-31T23:57:41.730992+00:00",
    "startDateTime": "2016-12-31T23:58:12.4547779+00:00",
    "endDateTime": "2016-12-31T23:56:38.1219845+00:00",
    "error": {
      "@odata.type": "microsoft.graph.classificationError"
    },
    "result": {
      "@odata.type": "microsoft.graph.dlpPoliciesJobResult"
    }
  }
}
```

