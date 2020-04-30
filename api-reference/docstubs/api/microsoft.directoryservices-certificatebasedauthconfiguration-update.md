---
title: "Update certificateBasedAuthConfiguration"
description: "Update the properties of a certificateBasedAuthConfiguration object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update certificateBasedAuthConfiguration

Namespace: Microsoft.DirectoryServices

Update the properties of a [certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md) object.

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
PATCH /certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md) object.

The following table shows the properties that are required when you create the [certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|certificateAuthorities|[certificateAuthority](../resources/microsoft.directoryservices-certificateauthority.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [certificateBasedAuthConfiguration](../resources/microsoft.directoryservices-certificatebasedauthconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_certificatebasedauthconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
Content-Type: application/json
Content-length: 552

{
  "@odata.type": "#Microsoft.DirectoryServices.certificateBasedAuthConfiguration",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
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
```

