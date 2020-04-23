---
title: "List certificateBasedAuthConfiguration"
description: "Get the certificateBasedAuthConfigurations from the certificateBasedAuthConfiguration navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List certificateBasedAuthConfiguration

Namespace: microsoft.graph

Get the certificateBasedAuthConfigurations from the certificateBasedAuthConfiguration navigation property.

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
GET /organization/{organizationId}/certificateBasedAuthConfiguration
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
If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}/certificateBasedAuthConfiguration
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.certificatebasedauthconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
      "id": "e1f46a41-6a41-e1f4-416a-f4e1416af4e1",
      "certificateAuthorities": [
        {
          "@odata.type": "microsoft.graph.certificateAuthority",
          "isRootAuthority": true,
          "certificateRevocationListUrl": "https://example.com/certificateRevocationListUrl/",
          "deltaCertificateRevocationListUrl": "https://example.com/deltaCertificateRevocationListUrl/",
          "certificate": "Y2VydGlmaWNhdGU=",
          "issuer": "Issuer value",
          "issuerSki": "Issuer Ski value"
        }
      ]
    }
  ]
}
```

