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
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.

The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|helpUrl|String|The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.|
|displayName|String|The display name for the profile.|
|issuer|deviceManagementDerivedCredentialIssuer|The derived credential provider to use. Possible values are: `intercede`, `entrustDatacard`, `purebred`, `xTec`.|
|notificationType|deviceManagementDerivedCredentialNotificationType|The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device. Possible values are: `none`, `companyPortal`, `email`.|



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
Content-length: 225

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
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
  "id": "cb6eed73-ed73-cb6e-73ed-6ecb73ed6ecb",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "String",
  "notificationType": "String"
}
```

