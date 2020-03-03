---
title: "Create externalFile"
description: "Create a new externalFile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create externalFile

Namespace: microsoft.graph

Create a new [externalFile](../resources/externalfile.md) object.

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
POST ** Collection URI for microsoft.graph.externalFile not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [externalFile](../resources/externalfile.md) object.

The following table shows the properties that are required when you create the [externalFile](../resources/externalfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|properties|[properties](../resources/properties.md)| Inherited from [externalItem](../resources/externalitem.md)|
|content|String| Inherited from [externalItem](../resources/externalitem.md)|
|acl|[acl](../resources/acl.md) collection| Inherited from [externalItem](../resources/externalitem.md)|
|createdDateTime|DateTimeOffset||
|modifiedDateTime|DateTimeOffset||
|createdBy|String||
|lastModifiedBy|String||
|title|String||
|url|String||
|name|String||
|extension|String||
|size|Int64||



## Response
If successful, this method returns a `201 Created` response code and a [externalFile](../resources/externalfile.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_externalfile_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.externalFile not found
Content-type: application/json
Content-length: 532

{
  "@odata.type": "#microsoft.graph.externalFile",
  "properties": {
    "@odata.type": "microsoft.graph.properties"
  },
  "content": "Content value",
  "acl": [
    {
      "@odata.type": "microsoft.graph.acl",
      "type": "String",
      "value": "Value value",
      "accessType": "String",
      "identitySource": "Identity Source value"
    }
  ],
  "createdBy": "Created By value",
  "title": "Title value",
  "url": "Url value",
  "name": "Name value",
  "extension": "Extension value",
  "size": 4
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalfile"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 746

{
  "@odata.type": "#microsoft.graph.externalFile",
  "id": "26e60572-0572-26e6-7205-e6267205e626",
  "properties": {
    "@odata.type": "microsoft.graph.properties"
  },
  "content": "Content value",
  "acl": [
    {
      "@odata.type": "microsoft.graph.acl",
      "type": "String",
      "value": "Value value",
      "accessType": "String",
      "identitySource": "Identity Source value"
    }
  ],
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00",
  "createdBy": "Created By value",
  "lastModifiedBy": "Last Modified By value",
  "title": "Title value",
  "url": "Url value",
  "name": "Name value",
  "extension": "Extension value",
  "size": 4
}
```

