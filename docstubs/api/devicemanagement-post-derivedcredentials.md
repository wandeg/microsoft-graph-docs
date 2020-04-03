---
title: "Add derivedCredentials"
description: "Add derivedCredentials by posting to the derivedCredentials collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add derivedCredentials

Namespace: microsoft.graph

Add derivedCredentials by posting to the derivedCredentials collection.

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
POST /deviceManagement/derivedCredentials/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.

The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|helpUrl|String||
|displayName|String||
|issuer|Enumeration| Possible values are: `intercede`, `entrustDatacard`, `purebred`, `xTec`.|
|notificationType|Enumeration| Possible values are: `none`, `companyPortal`, `email`.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementderivedcredentialsettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementderivedcredentialsettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 274

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "9393fa53-fa53-9393-53fa-939353fa9393",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "String",
  "notificationType": "String"
}
```

