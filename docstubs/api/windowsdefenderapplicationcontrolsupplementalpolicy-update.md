---
title: "Update windowsDefenderApplicationControlSupplementalPolicy"
description: "Update the properties of a windowsDefenderApplicationControlSupplementalPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windowsDefenderApplicationControlSupplementalPolicy

Namespace: microsoft.graph

Update the properties of a [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.

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
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.

The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|content|Binary||
|contentFileName|String||
|version|String||
|creationDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|roleScopeTagIds|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_windowsdefenderapplicationcontrolsupplementalpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
Content-type: application/json
Content-length: 403

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:02:18.736171+00:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
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
Content-Length: 516

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "fbc55652-5652-fbc5-5256-c5fb5256c5fb",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:02:18.736171+00:00",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

