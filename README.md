# Create Azure IoT Hub using ARM Template
This ARM template is to create Azure IoT hub with different parameters

## List of Parameters

"parameters": {
    "hubName": {
      "type": "string"
    },
    "retentionTimeInDays": {
      "type": "int",
      "defaultValue": 1
    },
    "partitionCount": {
      "type": "int",
      "defaultValue": 4
    },
    "partitionIds": {
      "type": "array",
      "defaultValue": [ "0", "1", "2", "3" ]
    },
    "storageAccountType": {
      "type": "string",
      "defaultValue": "Standard_RAGRS",
      "allowedValues": [
        "Standard_LRS",
        "Standard_GRS",
        "Standard_RAGRS"
      ],
      "metadata": {
        "description": "Storage Account type"
      }
    }
  },
