---
title: "Create vppTokens"
description: "Create a new vppTokens object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create vppTokens

Namespace: microsoft.graph

Create a new vppTokens object.

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
POST /deviceAppManagement/vppTokens
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [vppToken](../resources/vpptoken.md) object.

The following table shows the properties that are required when you create the [vppToken](../resources/vpptoken.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|organizationName|String|**TODO: Add Description**|
|vppTokenAccountType|vppTokenAccountType|**TODO: Add Description**. Possible values are: `business`, `education`.|
|appleId|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|token|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|state|vppTokenState|**TODO: Add Description**. Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|tokenActionResults|[vppTokenActionResult](../resources/vpptokenactionresult.md) collection|**TODO: Add Description**|
|lastSyncStatus|vppTokenSyncStatus|**TODO: Add Description**. Possible values are: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|**TODO: Add Description**|
|countryOrRegion|String|**TODO: Add Description**|
|dataSharingConsentGranted|Boolean|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|locationName|String|**TODO: Add Description**|
|claimTokenManagementFromExternalMdm|Boolean|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [vppToken](../resources/vpptoken.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_vpptoken_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
Content-Type: application/json
Content-length: 688

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult"
    }
  ],
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": "Boolean",
  "countryOrRegion": "String",
  "dataSharingConsentGranted": "Boolean",
  "displayName": "String",
  "locationName": "String",
  "claimTokenManagementFromExternalMdm": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.vpptoken"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "1b5bdf0a-df0a-1b5b-0adf-5b1b0adf5b1b",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult"
    }
  ],
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": "Boolean",
  "countryOrRegion": "String",
  "dataSharingConsentGranted": "Boolean",
  "displayName": "String",
  "locationName": "String",
  "claimTokenManagementFromExternalMdm": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

