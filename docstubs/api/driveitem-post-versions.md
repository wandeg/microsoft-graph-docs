---
title: "Add versions"
description: "Add versions by posting to the versions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add versions

Namespace: microsoft.graph

Add versions by posting to the versions collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /workbooks/{workbooksId}/versions/$ref
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/versions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [driveItemVersion](../resources/driveitemversion.md) object.

The following table shows the properties that are required when you create the [driveItemVersion](../resources/driveitemversion.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|publication|[publicationFacet](../resources/publicationfacet.md)| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|content|Stream||
|size|Int64||



## Response
If successful, this method returns a `201 Created` response code and a [driveItemVersion](../resources/driveitemversion.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_driveitemversion_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/versions
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.driveItemVersion",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "Level value",
    "versionId": "Version Id value"
  },
  "content": "Stream",
  "size": 4
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveitemversion"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 730

{
  "@odata.type": "#microsoft.graph.driveItemVersion",
  "id": "00e11678-1678-00e1-7816-e1007816e100",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "Level value",
    "versionId": "Version Id value"
  },
  "content": "Stream",
  "size": 4
}
```

