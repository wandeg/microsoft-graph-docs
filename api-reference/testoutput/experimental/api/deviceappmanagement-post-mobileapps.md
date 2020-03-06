---
title: "Add mobileApps"
description: "Add mobileApps by posting to the mobileApps collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add mobileApps

Namespace: microsoft.graph

Add mobileApps by posting to the mobileApps collection.

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
POST /deviceAppManagement/mobileApps/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [mobileApp](../resources/mobileapp.md) object.

The following table shows the properties that are required when you create the [mobileApp](../resources/mobileapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The admin provided or imported title of the app.|
|description|String|The description of the app.|
|publisher|String|The publisher of the app.|
|largeIcon|[mimeContent](../resources/mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon.|
|createdDateTime|DateTimeOffset|The date and time the app was created.|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified.|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin.|
|privacyInformationUrl|String|The privacy statement Url.|
|informationUrl|String|The more information Url.|
|owner|String|The owner of the app.|
|developer|String|The developer of the app.|
|notes|String|Notes for the app.|
|uploadState|Int32|The upload state.|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Possible values are: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app.|
|dependentAppCount|Int32|The total number of dependencies the child app has.|



## Response
If successful, this method returns a `201 Created` response code and a [mobileApp](../resources/mobileapp.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mobileapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 704

{
  "@odata.type": "#microsoft.graph.mobileApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileapp"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 876

{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "89b14746-4746-89b1-4647-b1894647b189",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1
}
```

