---
title: "Update directoryObjectPartnerReference"
description: "Update the properties of a directoryObjectPartnerReference object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update directoryObjectPartnerReference

Update the properties of a [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object.

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
PATCH ** Entity URI for microsoft.graph.directoryObjectPartnerReference not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [directoryObjectPartnerReference](../resources/directoryObjectPartnerReference.md) object.

The following table shows the properties that are required when you create the [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|description|String||
|displayName|String||
|externalPartnerTenantId|Guid||
|objectType|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_directoryobjectpartnerreference"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.directoryObjectPartnerReference not found
Content-type: application/json
Content-length: 319

{
  "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
  "deletedDateTime": "2017-01-01T00:02:13.7092325+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "externalPartnerTenantId": "b4e14d2f-4d2f-b4e1-2f4d-e1b42f4de1b4",
  "objectType": "Object Type value"
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
Content-Length: 368

{
  "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
  "id": "2785b77e-b77e-2785-7eb7-85277eb78527",
  "deletedDateTime": "2017-01-01T00:02:13.7092325+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "externalPartnerTenantId": "b4e14d2f-4d2f-b4e1-2f4d-e1b42f4de1b4",
  "objectType": "Object Type value"
}
```

