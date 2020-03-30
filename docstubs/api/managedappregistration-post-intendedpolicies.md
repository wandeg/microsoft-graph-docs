---
title: "Add intendedPolicies"
description: "Add intendedPolicies by posting to the intendedPolicies collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add intendedPolicies

Namespace: microsoft.graph

Add intendedPolicies by posting to the intendedPolicies collection.

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
POST /me/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedAppPolicy](../resources/managedapppolicy.md) object.

The following table shows the properties that are required when you create the [managedAppPolicy](../resources/managedapppolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|roleScopeTagIds|String collection||
|version|String||



## Response
If successful, this method returns a `201 Created` response code and a [managedAppPolicy](../resources/managedapppolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managedapppolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedapppolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 402

{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "id": "ac01154b-154b-ac01-4b15-01ac4b1501ac",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
  "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value"
}
```

