---
title: "Create wdacSupplementalPolicies"
description: "Create a new wdacSupplementalPolicies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create wdacSupplementalPolicies

Namespace: microsoft.graph

Create a new wdacSupplementalPolicies object.

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
POST /deviceAppManagement/wdacSupplementalPolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md) object.

The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicy](../resources/windowsdefenderapplicationcontrolsupplementalpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_windowsdefenderapplicationcontrolsupplementalpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies
Content-Type: application/json
Content-length: 403

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsdefenderapplicationcontrolsupplementalpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "00cfa809-a809-00cf-09a8-cf0009a8cf00",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

