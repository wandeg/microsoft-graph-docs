---
title: "Add account"
description: "Add account by posting to the account collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add account

Namespace: microsoft.graph

Add account by posting to the account collection.

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
POST /me/profile/account/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [userAccountInformation](../resources/useraccountinformation.md) object.

The following table shows the properties that are required when you create the [userAccountInformation](../resources/useraccountinformation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|ageGroup|String||
|countryCode|String||
|preferredLanguageTag|[localeInfo](../resources/localeinfo.md)||
|userPrincipalName|String||



## Response
If successful, this method returns a `201 Created` response code and a [userAccountInformation](../resources/useraccountinformation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_useraccountinformation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/account
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.userAccountInformation",
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
  "ageGroup": "Age Group value",
  "countryCode": "Country Code value",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo",
    "locale": "Locale value"
  },
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.useraccountinformation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1106

{
  "@odata.type": "#microsoft.graph.userAccountInformation",
  "id": "7ba7206b-206b-7ba7-6b20-a77b6b20a77b",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData",
    "confidenceScore": "Double",
    "userHasVerifiedAccuracy": true
  },
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "ageGroup": "Age Group value",
  "countryCode": "Country Code value",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo",
    "locale": "Locale value"
  },
  "userPrincipalName": "User Principal Name value"
}
```

