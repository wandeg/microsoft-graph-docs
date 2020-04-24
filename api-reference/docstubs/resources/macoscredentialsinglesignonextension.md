---
title: "macOSCredentialSingleSignOnExtension resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# macOSCredentialSingleSignOnExtension resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [macOSSingleSignOnExtension](../resources/macossinglesignonextension.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurations|[keyTypedValuePair](../resources/keytypedvaluepair.md) collection|Gets or sets a list of typed key-value pairs used to configure Credential-type profiles. This collection can contain a maximum of 500 elements.|
|domains|String collection|Gets or sets a list of hosts or domain names for which the app extension performs SSO.|
|extensionIdentifier|String|Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.|
|realm|String|Gets or sets the case-sensitive realm name for this profile.|
|teamIdentifier|String|Gets or sets the team ID of the app extension that performs SSO for the specified URLs.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSCredentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCredentialSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "domains": [
    "String"
  ],
  "realm": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```

