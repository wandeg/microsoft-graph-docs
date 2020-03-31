---
title: "Update webAccount"
description: "Update the properties of a webAccount object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update webAccount

Namespace: microsoft.graph

Update the properties of a [webAccount](../resources/webaccount.md) object.

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
PATCH /me/profile/webAccounts/{webAccountId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [webAccount](../resources/webaccount.md) object.

The following table shows the properties that are required when you create the [webAccount](../resources/webaccount.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|description|String||
|userId|String||
|service|[serviceInformation](../resources/serviceinformation.md)||
|statusMessage|String||
|webUrl|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_webaccount"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/webAccounts/{webAccountId}
Content-type: application/json
Content-length: 910

{
  "@odata.type": "#microsoft.graph.webAccount",
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
  "description": "Description value",
  "userId": "User Id value",
  "service": {
    "@odata.type": "microsoft.graph.serviceInformation",
    "name": "Name value",
    "webUrl": "https://example.com/webUrl/"
  },
  "statusMessage": "Status Message value",
  "webUrl": "https://example.com/webUrl/"
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
Content-Length: 1160

{
  "@odata.type": "#microsoft.graph.webAccount",
  "id": "9525ab38-ab38-9525-38ab-259538ab2595",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
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
  "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": "Description value",
  "userId": "User Id value",
  "service": {
    "@odata.type": "microsoft.graph.serviceInformation",
    "name": "Name value",
    "webUrl": "https://example.com/webUrl/"
  },
  "statusMessage": "Status Message value",
  "webUrl": "https://example.com/webUrl/"
}
```

