---
title: "Create allowedDataLocation"
description: "Create a new allowedDataLocation object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create allowedDataLocation

Namespace: Microsoft.DirectoryServices

Create a new [allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md) object.

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
POST /allowedDataLocations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md) object.

The following table shows the properties that are required when you create the [allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|location|String|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|
|domain|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_alloweddatalocation_from_alloweddatalocations"
}
-->
``` http
POST https://graph.microsoft.com/changelog/allowedDataLocations
Content-Type: application/json
Content-length: 185

{
  "@odata.type": "#Microsoft.DirectoryServices.allowedDataLocation",
  "appId": "App Id value",
  "location": "Location value",
  "isDefault": true,
  "domain": "Domain value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.alloweddatalocation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.allowedDataLocation",
  "id": "22b68f8a-8f8a-22b6-8a8f-b6228a8fb622",
  "appId": "App Id value",
  "location": "Location value",
  "isDefault": true,
  "domain": "Domain value"
}
```

