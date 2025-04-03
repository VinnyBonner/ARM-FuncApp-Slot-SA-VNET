ARM Template that creates the below resources:

VNET
Subnet for Function App
Subnet for Private Endpoints
Private DNS Zones for Storage and Function App Private Endpoints
Storage Account with Private Endpoints on each endpoint (File, Blob, Queue, Table)
Function App with Private Endpoint and VNET integrated
Function App Slot with Private Endpoint and VNET integrated

End result is the function app and slot are connecting over the VNET to the storage account's Private endpoint to run (AzureWebJobStorage) and has a Private Endpoints for inbound connection.
