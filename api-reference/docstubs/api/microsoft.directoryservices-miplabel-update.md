---
title: "Update mipLabel"
description: "Update the properties of a mipLabel object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update mipLabel

Namespace: Microsoft.DirectoryServices

Update the properties of a [mipLabel](../resources/microsoft.directoryservices-miplabel.md) object.

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
PATCH /mipLabels/{mipLabelsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [mipLabel](../resources/microsoft.directoryservices-miplabel.md) object.

The following table shows the properties that are required when you create the [mipLabel](../resources/microsoft.directoryservices-miplabel.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|labelId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|protectGroupAction|[mipProtectGroupLabelAction](../resources/microsoft.directoryservices-mipprotectgrouplabelaction.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [mipLabel](../resources/microsoft.directoryservices-miplabel.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_miplabel"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/mipLabels/{mipLabelsId}
Content-Type: application/json
Content-length: 378

{
  "@odata.type": "#Microsoft.DirectoryServices.mipLabel",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "labelId": "Label Id value",
  "displayName": "Display Name value",
  "protectGroupAction": {
    "@odata.type": "Microsoft.DirectoryServices.mipProtectGroupLabelAction",
    "isAccessAllowedToGuestUsers": true,
    "privacy": "Privacy value"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.mipLabel",
  "id": "042103df-03df-0421-df03-2104df032104",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "labelId": "Label Id value",
  "displayName": "Display Name value",
  "protectGroupAction": {
    "@odata.type": "Microsoft.DirectoryServices.mipProtectGroupLabelAction",
    "isAccessAllowedToGuestUsers": true,
    "privacy": "Privacy value"
  }
}
```

