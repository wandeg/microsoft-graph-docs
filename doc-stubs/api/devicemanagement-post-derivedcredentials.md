---
title: "Create derivedCredentials"
description: "Create a new derivedCredentials object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create derivedCredentials

Namespace: microsoft.graph

Create a new derivedCredentials object.

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
POST /deviceManagement/derivedCredentials
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.

The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|helpUrl|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|issuer|deviceManagementDerivedCredentialIssuer|**TODO: Add Description**. Possible values are: `intercede`, `entrustDatacard`, `purebred`, `xTec`.|
|notificationType|deviceManagementDerivedCredentialNotificationType|**TODO: Add Description**. Possible values are: `none`, `companyPortal`, `email`.|



## Response

If successful, this method returns a `201 Created` response code and a [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementderivedcredentialsettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
Content-Type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "helpUrl": "String",
  "displayName": "String",
  "issuer": "String",
  "notificationType": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementderivedcredentialsettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "fff17386-7386-fff1-8673-f1ff8673f1ff",
  "helpUrl": "String",
  "displayName": "String",
  "issuer": "String",
  "notificationType": "String"
}
```

