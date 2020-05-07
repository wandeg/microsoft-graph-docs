---
title: "Update iosLobAppProvisioningConfigurations"
description: "Update the properties of an iosLobAppProvisioningConfigurations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update iosLobAppProvisioningConfigurations

Namespace: microsoft.graph

Update the properties of an iosLobAppProvisioningConfigurations object.

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
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md) object.

The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|payloadFileName|String|**TODO: Add Description**|
|payload|Binary|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_ioslobappprovisioningconfigurations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
Content-Type: application/json
Content-length: 304

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "String (timestamp)",
  "payloadFileName": "String",
  "payload": "Binary",
  "roleScopeTagIds": [
    "String"
  ],
  "description": "String",
  "displayName": "String",
  "version": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "acfac795-c795-acfa-95c7-faac95c7faac",
  "expirationDateTime": "String (timestamp)",
  "payloadFileName": "String",
  "payload": "Binary",
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": "Integer"
}
```

