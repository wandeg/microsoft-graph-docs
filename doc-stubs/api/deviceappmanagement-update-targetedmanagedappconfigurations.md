---
title: "Update targetedManagedAppConfigurations"
description: "Update the properties of a targetedManagedAppConfigurations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update targetedManagedAppConfigurations

Namespace: microsoft.graph

Update the properties of a targetedManagedAppConfigurations object.

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
PATCH /deviceAppManagement/targetedManagedAppConfigurations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.

The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|description|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|roleScopeTagIds|String collection|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|version|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description** Inherited from [managedAppConfiguration](../resources/managedappconfiguration.md)|
|deployedAppCount|Int32|**TODO: Add Description**|
|isAssigned|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_targetedmanagedappconfigurations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
Content-Type: application/json
Content-length: 355

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "deployedAppCount": "Integer",
  "isAssigned": "Boolean"
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
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "id": "b41aba42-ba42-b41a-42ba-1ab442ba1ab4",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "deployedAppCount": "Integer",
  "isAssigned": "Boolean"
}
```

