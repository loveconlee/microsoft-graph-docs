﻿# androidForWorkAppConfigurationSchema resource type

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Schema describing an Android for Work application's custom configurations.
## Methods
|Method|Return Type|Description|
|---|---|---|
|[List androidForWorkAppConfigurationSchemas](../api/intune_androidforwork_androidforworkappconfigurationschema_list.md)|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) collection|List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) objects.|
|[Get androidForWorkAppConfigurationSchema](../api/intune_androidforwork_androidforworkappconfigurationschema_get.md)|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)|Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.|
|[Create androidForWorkAppConfigurationSchema](../api/intune_androidforwork_androidforworkappconfigurationschema_create.md)|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)|Create a new [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.|
|[Delete androidForWorkAppConfigurationSchema](../api/intune_androidforwork_androidforworkappconfigurationschema_delete.md)|None|Deletes a [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).|
|[Update androidForWorkAppConfigurationSchema](../api/intune_androidforwork_androidforworkappconfigurationschema_update.md)|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)|Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.|

## Properties
|Property|Type|Description|
|---|---|---|
|id|String|Key of the entity the Android package name for the application the schema corresponds to|
|exampleJson|[androidForWorkAppConfigurationExample](../resources/intune_androidforwork_androidforworkappconfigurationexample.md)|Example JSON confirming to this schema that demonstrates how to set the configuration for this app|
|schemaItems|[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md) collection|Collection of items each representing a named configuration option in the schema|

## Relationships
None
## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchema"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": {
    "@odata.type": "microsoft.graph.androidForWorkAppConfigurationExample"
  },
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "String",
      "displayName": "String",
      "description": "String",
      "defaultBoolValue": true,
      "defaultIntValue": 1024,
      "defaultStringValue": "String",
      "defaultStringArrayValue": [
        "String"
      ],
      "dataType": "String",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "key": "String",
          "value": "String"
        }
      ]
    }
  ]
}
```



