---
title: "Create windowsDefenderApplicationControlSupplementalPolicy"
description: "Create a new windowsDefenderApplicationControlSupplementalPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create windowsDefenderApplicationControlSupplementalPolicy

Namespace: microsoft.graph

Create a new [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.

The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The display name of WindowsDefenderApplicationControl supplemental policy.|
|description|String|The description of WindowsDefenderApplicationControl supplemental policy.|
|content|Binary|The WindowsDefenderApplicationControl supplemental policy content in byte array format.|
|contentFileName|String|The WindowsDefenderApplicationControl supplemental policy content's file name.|
|version|String|The WindowsDefenderApplicationControl supplemental policy's version.|
|creationDateTime|DateTimeOffset|The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.|
|lastModifiedDateTime|DateTimeOffset|The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.|
|roleScopeTagIds|String collection|List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.|



## Response
If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_windowsdefenderapplicationcontrolsupplementalpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/wdacSupplementalPolicies
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:02:11.4839005+03:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsdefenderapplicationcontrolsupplementalpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 517

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "e9f7fe24-fe24-e9f7-24fe-f7e924fef7e9",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:02:11.4839005+03:00",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

