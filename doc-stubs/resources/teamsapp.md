---
title: "teamsApp resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# teamsApp resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List teamsApps](../api/teamsapp-list.md)|[teamsApp](../resources/teamsapp.md) collection|Get a list of the [teamsApp](../resources/teamsapp.md) objects and their properties.|
|[Create teamsApp](../api/teamsapp-create.md)|[teamsApp](../resources/teamsapp.md)|Create a new [teamsApp](../resources/teamsapp.md) object.|
|[Get teamsApp](../api/teamsapp-get.md)|[teamsApp](../resources/teamsapp.md)|Read the properties and relationships of a [teamsApp](../resources/teamsapp.md) object.|
|[Update teamsApp](../api/teamsapp-update.md)|[teamsApp](../resources/teamsapp.md)|Update the properties of a [teamsApp](../resources/teamsapp.md) object.|
|[Delete teamsApp](../api/teamsapp-delete.md)|None|Deletes a [teamsApp](../resources/teamsapp.md) object.|
|[List appDefinitions](../api/teamsapp-list-appdefinitions.md)|[teamsAppDefinition](../resources/teamsappdefinition.md) collection|Get the teamsAppDefinitions from the appDefinitions navigation property.|
|[Create appDefinitions](../api/teamsapp-post-appdefinitions.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Create a new appDefinitions object.|
|[Get appDefinitions](../api/teamsapp-get-teamsappdefinition.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Read the properties and relationships of a [teamsAppDefinition](../resources/teamsappdefinition.md) object.|
|[Update appDefinitions](../api/teamsapp-update-appdefinitions.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Update the properties of an appDefinitions object.|
|[Delete appDefinitions](../api/teamsapp-delete-appdefinitions.md)|None|Delete a [teamsAppDefinition](../resources/teamsappdefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|distributionMethod|teamsAppDistributionMethod|**TODO: Add Description**. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|
|externalId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appDefinitions|[teamsAppDefinition](../resources/teamsappdefinition.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsApp",
  "id": "String (identifier)",
  "externalId": "String",
  "displayName": "String",
  "distributionMethod": "String"
}
```

