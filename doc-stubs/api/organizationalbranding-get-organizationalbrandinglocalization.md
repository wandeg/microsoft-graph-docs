---
title: "Get localizations"
description: "Read the properties and relationships of an organizationalBrandingLocalization object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get localizations

Namespace: microsoft.graph

Read the properties and relationships of an [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) object.

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
GET /organization/{organizationId}/branding/localizations
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

If successful, this method returns a `200 OK` response code and an [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandinglocalization"
}
-->
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}/branding/localizations
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.organizationalBrandingLocalization"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.organizationalBrandingLocalization",
    "id": "57881191-1191-5788-9111-885791118857",
    "backgroundColor": "String",
    "backgroundImage": "Stream",
    "bannerLogo": "Stream",
    "signInPageText": "String",
    "squareLogo": "Stream",
    "usernameHintText": "String"
  }
}
```

