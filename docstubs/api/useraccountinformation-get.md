---
title: "Get userAccountInformation"
description: "Read properties and relationships of the userAccountInformation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userAccountInformation

Namespace: microsoft.graph

Read properties and relationships of the [userAccountInformation](../resources/useraccountinformation.md) object.

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
GET /me/profile/account/{userAccountInformationId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [userAccountInformation](../resources/useraccountinformation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/account/{userAccountInformationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1193

{
  "value": {
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
}
```

