---
title: "Get certificateBasedAuthConfiguration"
description: "Read the properties and relationships of a certificateBasedAuthConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get certificateBasedAuthConfiguration

Namespace: microsoft.graph

Read the properties and relationships of a [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.

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
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
    "id": "468dac06-ac06-468d-06ac-8d4606ac8d46",
    "certificateAuthorities": [
      {
        "@odata.type": "microsoft.graph.certificateAuthority"
      }
    ]
  }
}
```

