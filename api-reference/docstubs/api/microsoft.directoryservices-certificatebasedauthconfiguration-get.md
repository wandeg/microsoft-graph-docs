---
title: "Get certificateBasedAuthConfiguration"
description: "Read properties and relationships of a certificateBasedAuthConfiguration object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get certificateBasedAuthConfiguration

Namespace: Microsoft.DirectoryServices

Read properties and relationships of a [certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md) object.

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
GET /certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/changelog/certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.certificateBasedAuthConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.certificateBasedAuthConfiguration",
    "id": "bd0b4e5c-4e5c-bd0b-5c4e-0bbd5c4e0bbd",
    "certificateAuthorities": [
      {
        "@odata.type": "Microsoft.DirectoryServices.certificateAuthority",
        "isRootAuthority": true,
        "certificateRevocationListUrl": "https://example.com/certificateRevocationListUrl/",
        "deltaCertificateRevocationListUrl": "https://example.com/deltaCertificateRevocationListUrl/",
        "certificate": "Y2VydGlmaWNhdGU=",
        "issuer": "Issuer value",
        "issuerSki": "Issuer Ski value"
      }
    ]
  }
}
```

