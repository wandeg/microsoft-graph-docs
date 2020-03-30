---
title: "Update personAnniversary"
description: "Update the properties of a personAnniversary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update personAnniversary

Namespace: microsoft.graph

Update the properties of a [personAnniversary](../resources/personanniversary.md) object.

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
PATCH /me/profile/anniversaries/{personAnniversaryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [personAnniversary](../resources/personanniversary.md) object.

The following table shows the properties that are required when you create the [personAnniversary](../resources/personanniversary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|type|Enumeration| Possible values are: `birthday`, `wedding`, `unknownFutureValue`.|
|date|Date||



## Response
If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_personanniversary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/anniversaries/{personAnniversaryId}
Content-type: application/json
Content-length: 648

{
  "@odata.type": "#microsoft.graph.personAnniversary",
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
  "type": "String",
  "date": "Date"
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
Content-Length: 899

{
  "@odata.type": "#microsoft.graph.personAnniversary",
  "id": "8a56b00c-b00c-8a56-0cb0-568a0cb0568a",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
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
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "type": "String",
  "date": "Date"
}
```

