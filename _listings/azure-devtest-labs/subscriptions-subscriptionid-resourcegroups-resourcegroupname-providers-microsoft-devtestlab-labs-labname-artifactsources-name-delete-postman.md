{
  "info": {
    "name": "Azure DevTest Labs API Artifact Sources Delete",
    "_postman_id": "a737ac6e-0e18-4f63-9a3e-b0c25e920d5c",
    "description": "Delete artifact source.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "artifact sources",
      "item": [
        {
          "id": "2fe870ad-02fc-42b3-a534-4ad12f734c42",
          "name": "ArtifactSources_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.DevTestLab/labs/:labName/artifactsources/:name"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "labName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete artifact source"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81cdc730-5229-43e9-813c-a89a935c9180"
            }
          ]
        }
      ]
    }
  ]
}