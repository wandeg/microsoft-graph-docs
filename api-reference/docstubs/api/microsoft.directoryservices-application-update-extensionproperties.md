---
title: "Update extensionProperties"
description: "Update the properties of an extensionProperties object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update extensionProperties

Namespace: Microsoft.DirectoryServices

Update the properties of an extensionProperties object.

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
PATCH /applications/{applicationsId}/extensionProperties
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md) object.

The following table shows the properties that are required when you create the [extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|appDisplayName|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|dataType|String|**TODO: Add Description**|
|isSyncedFromOnPremises|Boolean|**TODO: Add Description**|
|targetObjects|String collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [extensionProperty](../resources/microsoft.directoryservices-extensionproperty.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_extensionproperties"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/applications/{applicationsId}/extensionProperties
Content-Type: application/json
Content-length: 327

{
  "@odata.type": "#Microsoft.DirectoryServices.extensionProperty",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "appDisplayName": "App Display Name value",
  "name": "Name value",
  "dataType": "Data Type value",
  "isSyncedFromOnPremises": true,
  "targetObjects": [
    "Target Objects value"
  ]
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
  "@odata.type": "#Microsoft.DirectoryServices.extensionProperty",
  "id": "bac24b26-4b26-bac2-264b-c2ba264bc2ba",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "appDisplayName": "App Display Name value",
  "name": "Name value",
  "dataType": "Data Type value",
  "isSyncedFromOnPremises": true,
  "targetObjects": [
    "Target Objects value"
  ]
}
```

