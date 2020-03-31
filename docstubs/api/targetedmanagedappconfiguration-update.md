---
title: "Update targetedManagedAppConfiguration"
description: "Update the properties of a targetedManagedAppConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update targetedManagedAppConfiguration

Namespace: microsoft.graph

Update the properties of a [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.

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
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object.

The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|description|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|createdDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|roleScopeTagIds|String collection| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|version|String| Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/keyvaluepair.md) collection| Inherited from [managedAppConfiguration](../resources/managedappconfiguration.md)|
|deployedAppCount|Int32||
|isAssigned|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/targetedmanagedappconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_targetedmanagedappconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 621

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "id": "2ee7cda2-cda2-2ee7-a2cd-e72ea2cde72e",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

