---
title: "Add emails"
description: "Add emails by posting to the emails collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add emails

Namespace: microsoft.graph

Add emails by posting to the emails collection.

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
POST /me/profile/emails/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [itemEmail](../resources/itememail.md) object.

The following table shows the properties that are required when you create the [itemEmail](../resources/itememail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|address|String||
|displayName|String||
|type|Enumeration| Possible values are: `unknown`, `work`, `personal`, `main`, `other`.|



## Response
If successful, this method returns a `201 Created` response code and a [itemEmail](../resources/itememail.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_itememail_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/emails
Content-type: application/json
Content-length: 692

{
  "@odata.type": "#microsoft.graph.itemEmail",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdBy": {
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
  "address": "Address value",
  "displayName": "Display Name value",
  "type": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itememail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 943

{
  "@odata.type": "#microsoft.graph.itemEmail",
  "id": "38d87772-7772-38d8-7277-d8387277d838",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "createdBy": {
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
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": "Address value",
  "displayName": "Display Name value",
  "type": "String"
}
```

