---
title: "Create secureScore"
description: "Create a new secureScore object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create secureScore

Namespace: microsoft.graph

Create a new [secureScore](../resources/securescore.md) object.

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
POST /Security/secureScores
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [secureScore](../resources/securescore.md) object.

The following table shows the properties that are required when you create the [secureScore](../resources/securescore.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activeUserCount|Int32||
|averageComparativeScores|[averageComparativeScore](../resources/averagecomparativescore.md) collection||
|azureTenantId|String||
|controlScores|[controlScore](../resources/controlscore.md) collection||
|createdDateTime|DateTimeOffset||
|currentScore|Double||
|enabledServices|String collection||
|licensedUserCount|Int32||
|maxScore|Double||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||



## Response
If successful, this method returns a `201 Created` response code and a [secureScore](../resources/securescore.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_securescore_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/Security/secureScores
Content-type: application/json
Content-length: 960

{
  "@odata.type": "#microsoft.graph.secureScore",
  "activeUserCount": 15,
  "averageComparativeScores": [
    {
      "@odata.type": "microsoft.graph.averageComparativeScore",
      "averageScore": "Double",
      "basis": "Basis value"
    }
  ],
  "azureTenantId": "Azure Tenant Id value",
  "controlScores": [
    {
      "@odata.type": "microsoft.graph.controlScore",
      "controlCategory": "Control Category value",
      "controlName": "Control Name value",
      "description": "Description value",
      "score": "Double"
    }
  ],
  "currentScore": "Double",
  "enabledServices": [
    "Enabled Services value"
  ],
  "licensedUserCount": 1,
  "maxScore": "Double",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securescore"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1068

{
  "@odata.type": "#microsoft.graph.secureScore",
  "id": "532bd5c5-d5c5-532b-c5d5-2b53c5d52b53",
  "activeUserCount": 15,
  "averageComparativeScores": [
    {
      "@odata.type": "microsoft.graph.averageComparativeScore",
      "averageScore": "Double",
      "basis": "Basis value"
    }
  ],
  "azureTenantId": "Azure Tenant Id value",
  "controlScores": [
    {
      "@odata.type": "microsoft.graph.controlScore",
      "controlCategory": "Control Category value",
      "controlName": "Control Name value",
      "description": "Description value",
      "score": "Double"
    }
  ],
  "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
  "currentScore": "Double",
  "enabledServices": [
    "Enabled Services value"
  ],
  "licensedUserCount": 1,
  "maxScore": "Double",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation",
    "provider": "Provider value",
    "providerVersion": "Provider Version value",
    "subProvider": "Sub Provider value",
    "vendor": "Vendor value"
  }
}
```

