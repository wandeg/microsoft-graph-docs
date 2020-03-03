---
title: "Add extensionProperties"
description: "Add extensionProperties by posting to the extensionProperties collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add extensionProperties

Namespace: microsoft.graph

Add extensionProperties by posting to the extensionProperties collection.

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
POST /applications/{applicationsId}/extensionProperties/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [extensionProperty](../resources/extensionproperty.md) object.

The following table shows the properties that are required when you create the [extensionProperty](../resources/extensionproperty.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|appDisplayName|String||
|name|String||
|dataType|String||
|isSyncedFromOnPremises|Boolean||
|targetObjects|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [extensionProperty](../resources/extensionproperty.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_extensionproperty_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/applications/{applicationsId}/extensionProperties
Content-type: application/json
Content-length: 315

{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "deletedDateTime": "2017-01-01T00:02:42.9789072+03:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionproperty"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 364

{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "id": "5c0eb8c4-b8c4-5c0e-c4b8-0e5cc4b80e5c",
  "deletedDateTime": "2017-01-01T00:02:42.9789072+03:00",
  "appDisplayName": "App Display Name value",
  "name": "Name value",
  "dataType": "Data Type value",
  "isSyncedFromOnPremises": true,
  "targetObjects": [
    "Target Objects value"
  ]
}
```

