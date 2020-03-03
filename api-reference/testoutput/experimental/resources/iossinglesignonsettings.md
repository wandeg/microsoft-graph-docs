---
title: "iosSingleSignOnSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# iosSingleSignOnSettings resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAppsList|[appListItem](../resources/appListItem.md) collection|List of app identifiers that are allowed to use this login. If this field is omitted, the login applies to all applications on the device. This collection can contain a maximum of 500 elements.|
|allowedUrls|String collection|List of HTTP URLs that must be matched in order to use this login. With iOS 9.0 or later, a wildcard characters may be used.|
|displayName|String|The display name of login settings shown on the receiving device.|
|kerberosPrincipalName|String|A Kerberos principal name. If not provided, the user is prompted for one during profile installation.|
|kerberosRealm|String|A Kerberos realm name. Case sensitive.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```

