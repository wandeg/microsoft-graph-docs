---
title: "Update administrativeUnit"
description: "Update the properties of a administrativeUnit object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update administrativeUnit

Namespace: Microsoft.DirectoryServices

Update the properties of a [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) object.

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
PATCH /administrativeUnits/{administrativeUnitsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) object.

The following table shows the properties that are required when you create the [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|visibility|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/administrativeUnits/{administrativeUnitsId}
Content-Type: application/json
Content-length: 247

{
  "@odata.type": "#Microsoft.DirectoryServices.administrativeUnit",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "visibility": "Visibility value"
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
  "@odata.type": "#Microsoft.DirectoryServices.administrativeUnit",
  "id": "a2dd7382-7382-a2dd-8273-dda28273dda2",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "visibility": "Visibility value"
}
```

