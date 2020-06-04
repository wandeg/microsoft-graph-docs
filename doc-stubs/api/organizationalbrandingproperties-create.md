---
title: "Create organizationalBrandingProperties"
description: "Create a new organizationalBrandingProperties object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create organizationalBrandingProperties

Namespace: microsoft.graph

Create a new [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.

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
POST ** Collection URI for microsoft.graph.organizationalBrandingProperties not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.

The following table shows the properties that are required when you create the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|backgroundColor|String|**TODO: Add Description**|
|backgroundImage|Stream|**TODO: Add Description**|
|bannerLogo|Stream|**TODO: Add Description**|
|signInPageText|String|**TODO: Add Description**|
|squareLogo|Stream|**TODO: Add Description**|
|usernameHintText|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_organizationalbrandingproperties_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.organizationalBrandingProperties not found
Content-Type: application/json
Content-length: 256

{
  "@odata.type": "#microsoft.graph.organizationalBrandingProperties",
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
  "@odata.type": "microsoft.graph.organizationalbrandingproperties"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.organizationalBrandingProperties",
  "id": "74810118-0118-7481-1801-817418018174",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "bannerLogo": "Stream",
  "signInPageText": "String",
  "squareLogo": "Stream",
  "usernameHintText": "String"
}
```

