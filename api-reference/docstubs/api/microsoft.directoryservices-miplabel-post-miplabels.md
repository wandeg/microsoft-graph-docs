---
title: "Create mipLabel"
description: "Create a new mipLabel object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create mipLabel

Namespace: Microsoft.DirectoryServices

Create a new [mipLabel](../resources/microsoft.directoryservices-miplabel.md) object.

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
POST /mipLabels
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and a [mipLabel](../resources/microsoft.directoryservices-miplabel.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_miplabel_from_miplabels"
}
-->
``` http
POST https://graph.microsoft.com/changelog/mipLabels
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
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.miplabel"
}
-->
``` http
HTTP/1.1 201 Created
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

