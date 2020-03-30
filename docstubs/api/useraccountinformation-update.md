---
title: "Update userAccountInformation"
description: "Update the properties of a userAccountInformation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userAccountInformation

Namespace: microsoft.graph

Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object.

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
PATCH /me/profile/account/{userAccountInformationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [userAccountInformation](../resources/useraccountinformation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_useraccountinformation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/account/{userAccountInformationId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1106

{
  "@odata.type": "#microsoft.graph.userAccountInformation",
  "id": "352d7d85-7d85-352d-857d-2d35857d2d35",
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
  "ageGroup": "Age Group value",
  "countryCode": "Country Code value",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo",
    "locale": "Locale value"
  },
  "userPrincipalName": "User Principal Name value"
}
```

