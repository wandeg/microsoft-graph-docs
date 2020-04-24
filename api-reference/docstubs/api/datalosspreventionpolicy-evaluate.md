---
title: "dataLossPreventionPolicy: evaluate"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# evaluate

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
POST /invitations/{invitationsId}/invitedUser/informationProtection/dataLossPreventionPolicies/evaluate
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
|target|String|**TODO: Add Description**|
|evaluationInput|[dlpEvaluationInput](../resources/dlpevaluationinput.md)|**TODO: Add Description**|
|notificationInfo|[dlpNotification](../resources/dlpnotification.md)|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "datalosspreventionpolicy_evaluate"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/informationProtection/dataLossPreventionPolicies/evaluate

Content-Type: application/json
Content-length: 640

{
  "target": "Target value",
  "evaluationInput": {
    "@odata.type": "microsoft.graph.dlpEvaluationInput",
    "discoveredSensitiveTypes": [
      {
        "@odata.type": "microsoft.graph.discoveredSensitiveType",
        "id": "081ab855-b855-081a-55b8-1a0855b81a08",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dlpevaluatepoliciesjobresponse"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.dlpEvaluatePoliciesJobResponse",
    "id": "49f18bbb-8bbb-49f1-bb8b-f149bb8bf149",
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
      "@odata.type": "microsoft.graph.dlpPoliciesJobResult"
    }
  }
}
```

