---
title: "Add createdOnBehalfOf"
description: "Add createdOnBehalfOf by posting to the createdOnBehalfOf collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Add createdOnBehalfOf

Namespace: Microsoft.DirectoryServices

Add createdOnBehalfOf by posting to the createdOnBehalfOf collection.

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
POST /applications/{applicationsId}/createdOnBehalfOf/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [directoryObject](../resources/microsoft.directoryservices-directoryobject.md) object.

The following table shows the properties that are required when you create the [directoryObject](../resources/microsoft.directoryservices-directoryobject.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/microsoft.directoryservices-directoryobject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryobjects"
}
-->
``` http
POST https://graph.microsoft.com/changelog/applications/{applicationsId}/createdOnBehalfOf/$ref
Content-Type: application/json
Content-length: 128

{
  "@odata.type": "#Microsoft.DirectoryServices.directoryObject",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.directoryobject"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.directoryObject",
  "id": "a9c594c0-94c0-a9c5-c094-c5a9c094c5a9",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00"
}
```

