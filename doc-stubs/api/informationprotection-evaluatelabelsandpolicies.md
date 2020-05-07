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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
Content-length: 490

{
  "evaluateSensitivityLabels": {
    "@odata.type": "microsoft.graph.evaluateSensitivityLabelsRequest"
  },
  "evaluateDataLossPreventionPolicies": {
    "@odata.type": "microsoft.graph.dlpEvaluatePoliciesRequest"
  },
  "classifyText": {
    "@odata.type": "#microsoft.graph.textClassificationRequest",
    "id": "String (identifier)",
    "text": "String",
    "fileExtension": "String",
    "sensitiveTypeIds": [
      "String"
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
    "id": "String (identifier)",
    "type": "String",
    "status": "String",
    "tenantId": "String",
    "creationDateTime": "String (timestamp)",
    "startDateTime": "String (timestamp)",
    "endDateTime": "String (timestamp)",
    "error": {
      "@odata.type": "microsoft.graph.classificationError"
    },
    "result": {
      "@odata.type": "microsoft.graph.evaluateLabelsAndPoliciesResult"
    }
  }
}
```

