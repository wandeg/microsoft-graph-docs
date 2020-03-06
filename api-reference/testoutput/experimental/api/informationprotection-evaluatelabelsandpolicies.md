---
title: "evaluateLabelsAndPolicies"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# evaluateLabelsAndPolicies

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
POST /informationProtection/evaluateLabelsAndPolicies
POST /me/informationProtection/evaluateLabelsAndPolicies
POST /users/{usersId}/informationProtection/evaluateLabelsAndPolicies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|evaluateSensitivityLabels|[evaluateSensitivityLabelsRequest](../resources/evaluatesensitivitylabelsrequest.md)||
|evaluateDataLossPreventionPolicies|[dlpEvaluatePoliciesRequest](../resources/dlpevaluatepoliciesrequest.md)||
|classifyText|[textClassificationRequest](../resources/textclassificationrequest.md)||



## Response
If successful, this action returns a `200 OK` response code and a [evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "informationprotection_evaluatelabelsandpolicies"
}
-->
``` http
POST https://graph.microsoft.com/localtest/informationProtection/evaluateLabelsAndPolicies

Content-type: application/json
Content-length: 978

{
  "evaluateSensitivityLabels": {
    "@odata.type": "microsoft.graph.evaluateSensitivityLabelsRequest",
    "discoveredSensitiveTypes": [
      {
        "@odata.type": "microsoft.graph.discoveredSensitiveType",
        "count": 5
      }
    ],
    "currentLabel": {
      "@odata.type": "microsoft.graph.currentLabel"
    }
  },
  "evaluateDataLossPreventionPolicies": {
    "@odata.type": "microsoft.graph.dlpEvaluatePoliciesRequest",
    "evaluationInput": {
      "@odata.type": "microsoft.graph.dlpEvaluationInput",
      "accessScope": "String"
    },
    "notificationInfo": {
      "@odata.type": "microsoft.graph.dlpNotification",
      "author": "Author value"
    }
  },
  "classifyText": {
    "@odata.type": "#microsoft.graph.textClassificationRequest",
    "id": "b28c8213-8213-b28c-1382-8cb213828cb2",
    "text": "Text value",
    "sensitiveTypeIds": [
      "Sensitive Type Ids value"
    ],
    "scopesToRun": "String"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.evaluatelabelsandpoliciesjobresponse"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "value": {
    "@odata.type": "#microsoft.graph.evaluateLabelsAndPoliciesJobResponse",
    "id": "aa770a77-0a77-aa77-770a-77aa770a77aa",
    "type": "Type value",
    "status": "Status value",
    "tenantId": "Tenant Id value",
    "creationDateTime": "2016-12-31T23:59:35.5241957+03:00",
    "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
    "endDateTime": "2017-01-01T00:02:18.392989+03:00",
    "error": {
      "@odata.type": "microsoft.graph.classificationError"
    },
    "result": {
      "@odata.type": "microsoft.graph.evaluateLabelsAndPoliciesResult"
    }
  }
}
```

