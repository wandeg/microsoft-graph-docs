---
title: "Create localizations"
description: "Create a new localizations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create localizations

Namespace: microsoft.graph

Create a new localizations object.

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
POST /organization/{organizationId}/branding/localizations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) object.

The following table shows the properties that are required when you create the [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|backgroundColor|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|backgroundImage|Stream|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|bannerLogo|Stream|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|signInPageText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|squareLogo|Stream|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|
|usernameHintText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md)|



## Response

If successful, this method returns a `201 Created` response code and an [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_organizationalbrandinglocalization_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/organization/{organizationId}/branding/localizations
Content-Type: application/json
Content-length: 270

{
  "@odata.type": "#Microsoft.DirectoryServices.organizationalBrandingLocalization",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.organizationalbrandinglocalization"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.organizationalBrandingLocalization",
  "id": "57881191-1191-5788-9111-885791118857",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```

