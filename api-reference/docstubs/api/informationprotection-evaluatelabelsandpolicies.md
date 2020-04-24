---
title: "informationProtection: evaluateLabelsAndPolicies"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# evaluateLabelsAndPolicies

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /informationProtection/evaluateLabelsAndPolicies
POST /me/informationProtection/evaluateLabelsAndPolicies
POST /users/{usersId}/informationProtection/evaluateLabelsAndPolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|evaluateSensitivityLabels|[evaluateSensitivityLabelsRequest](../resources/evaluatesensitivitylabelsrequest.md)|**TODO: Add Description**|
|evaluateDataLossPreventionPolicies|[dlpEvaluatePoliciesRequest](../resources/dlpevaluatepoliciesrequest.md)|**TODO: Add Description**|
|classifyText|[textClassificationRequest](../resources/textclassificationrequest.md)|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "informationprotection_evaluatelabelsandpolicies"
}
-->
``` http
POST https://graph.microsoft.com/beta/informationProtection/evaluateLabelsAndPolicies

Content-Type: application/json
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
    "id": "8df80a4c-0a4c-8df8-4c0a-f88d4c0af88d",
    "text": "Text value",
    "sensitiveTypeIds": [
      "Sensitive Type Ids value"
    ],
    "scopesToRun": "String"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.evaluatelabelsandpoliciesjobresponse"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.evaluateLabelsAndPoliciesJobResponse",
    "id": "a795190e-190e-a795-0e19-95a70e1995a7",
    "type": "Type value",
    "status": "Status value",
    "tenantId": "Tenant Id value",
    "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
    "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
    "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
    "error": {
      "@odata.type": "microsoft.graph.classificationError"
    },
    "result": {
      "@odata.type": "microsoft.graph.evaluateLabelsAndPoliciesResult"
    }
  }
}
```

