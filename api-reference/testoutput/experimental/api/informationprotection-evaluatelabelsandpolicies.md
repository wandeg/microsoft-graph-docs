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

## HTTP Request
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
|Authorization|Bearer {token}|
|Content-Type|application/json|

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

## Example

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
    "id": "e29d35fd-35fd-e29d-fd35-9de2fd359de2",
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
Content-Length: 603

{
  "value": {
    "@odata.type": "#microsoft.graph.evaluateLabelsAndPoliciesJobResponse",
    "id": "b61f2273-2273-b61f-7322-1fb673221fb6",
    "type": "Type value",
    "status": "Status value",
    "tenantId": "Tenant Id value",
    "creationDateTime": "2017-01-01T00:02:11.4839005+03:00",
    "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
    "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
    "error": {
      "@odata.type": "microsoft.graph.classificationError"
    },
    "result": {
      "@odata.type": "microsoft.graph.evaluateLabelsAndPoliciesResult"
    }
  }
}
```

