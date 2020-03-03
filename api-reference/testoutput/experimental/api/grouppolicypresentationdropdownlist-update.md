---
title: "Update groupPolicyPresentationDropdownList"
description: "Update the properties of a groupPolicyPresentationDropdownList object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update groupPolicyPresentationDropdownList

Update the properties of a [groupPolicyPresentationDropdownList](../resources/grouppolicypresentationdropdownlist.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.graph.groupPolicyPresentationDropdownList not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/groupPolicyPresentationDropdownList.md) object.

The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/grouppolicypresentationdropdownlist.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/groupPolicyPresentation.md)|
|defaultItem|[groupPolicyPresentationDropdownListItem](../resources/groupPolicyPresentationDropdownListItem.md)|Localized string value identifying the default choice of the list of items.|
|items|[groupPolicyPresentationDropdownListItem](../resources/groupPolicyPresentationDropdownListItem.md) collection|Represents a set of localized display names and their associated values.|
|required|Boolean|Requirement to enter a value in the parameter box. The default value is false.|



## Response
If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/grouppolicypresentationdropdownlist.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_grouppolicypresentationdropdownlist"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.groupPolicyPresentationDropdownList not found
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem"
    }
  ],
  "required": true
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
Content-Length: 527

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "id": "66fc555c-555c-66fc-5c55-fc665c55fc66",
  "label": "Label value",
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem"
    }
  ],
  "required": true
}
```

