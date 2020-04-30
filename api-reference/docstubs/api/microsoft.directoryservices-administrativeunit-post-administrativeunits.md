---
title: "Create administrativeUnit"
description: "Create a new administrativeUnit object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create administrativeUnit

Namespace: Microsoft.DirectoryServices

Create a new [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) object.

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
POST /administrativeUnits
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}
-->
``` http
POST https://graph.microsoft.com/changelog/administrativeUnits
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
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.administrativeunit"
}
-->
``` http
HTTP/1.1 201 Created
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

