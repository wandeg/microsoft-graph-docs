---
title: "configurationManagerActionDeliveryStatus enum type"
description: "Delivery state of Configuration Manager device action"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# configurationManagerActionDeliveryStatus enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delivery state of Configuration Manager device action

## Members

| Member                            | Value | Description                                                                 |
| :-------------------------------- | ----: | :-------------------------------------------------------------------------- |
| unknown                           | 0     | Pending to deliver the action to ConfigurationManager                       |
| pendingDelivery                   | 1     | Pending to deliver the action to ConfigurationManager                       |
| deliveredToConnectorService       | 2     | Action is sent to ConfigurationManager Connector service (cloud)            |
| failedToDeliverToConnectorService | 3     | Failed to send the action to ConfigurationManager Connector service (cloud) |
| deliveredToOnPremisesServer       | 4     | Action is delivered to ConfigurationManager on-prem server                  |