---
title: "Create secureScores"
description: "Create a new secureScores object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create secureScores

Namespace: microsoft.graph

Create a new secureScores object.

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
POST /Security/secureScores
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [secureScore](../resources/securescore.md) object.

The following table shows the properties that are required when you create the [secureScore](../resources/securescore.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activeUserCount|Int32|**TODO: Add Description**|
|averageComparativeScores|[averageComparativeScore](../resources/averagecomparativescore.md) collection|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|controlScores|[controlScore](../resources/controlscore.md) collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|currentScore|Double|**TODO: Add Description**|
|enabledServices|String collection|**TODO: Add Description**|
|licensedUserCount|Int32|**TODO: Add Description**|
|maxScore|Double|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [secureScore](../resources/securescore.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_securescore_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/secureScores
Content-Type: application/json
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securescore"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.secureScore",
  "id": "24050234-0234-2405-3402-052434020524",
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
  "createdDateTime": "2017-01-01T00:01:28.5453509+00:00",
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

