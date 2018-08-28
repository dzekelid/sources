{
  "info": {
    "name": "HHS Media Services Get JPG preview for MediaItem",
    "_postman_id": "dd5761a9-d451-458e-9c79-aaf267a7efa4",
    "description": "Returns the JPG preview, where applicable, for the MediaItem identified by the 'id'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "d82e27d4-bdb7-4c8a-97e4-e602973ac757",
          "name": "getMediaByCampaignId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/campaigns/:id/media.json"
              ],
              "query": [
                {
                  "key": "max",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of MediaItems for the Campaign identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35b72f13-1bcb-46d3-82d9-5db4f0d3ee8e"
            }
          ]
        },
        {
          "id": "c2b5e387-9672-44fe-8254-6ae13e83fbf1",
          "name": "getMedia",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/media.json?collectionId=%7B%7D&contentAuthoredBeforeDate=%7B%7D&contentAuthoredInRange=%7B%7D&contentAuthoredSinceDate=%7B%7D&contentPublishedBeforeDate=%7B%7D&contentPublishedInRange=%7B%7D&contentPublishedSinceDate=%7B%7D&contentReviewedBeforeDate=%7B%7D&contentReviewedInRange=%7B%7D&contentReviewedSinceDate=%7B%7D&contentUpdatedBeforeDate=%7B%7D&contentUpdatedInRange=%7B%7D&contentUpdatedSinceDate=%7B%7D&createdBy=%7B%7D&customThumbnailUrl=%7B%7D&customThumbnailUrlContains=%7B%7D&dateContentAuthored=%7B%7D&dateContentPublished=%7B%7D&dateContentReviewed=%7B%7D&dateContentUpdated=%7B%7D&dateSyndicationCaptured=%7B%7D&dateSyndicationUpdated=%7B%7D&descriptionContains=%7B%7D&hash=%7B%7D&hashContains=%7B%7D&languageId=%7B%7D&languageIsoCode=%7B%7D&languageName=%7B%7D&max=%7B%7D&mediaTypes=%7B%7D&name=%7B%7D&nameContains=%7B%7D&offset=%7B%7D&order=%7B%7D&restrictToSet=%7B%7D&sort=%7B%7D&sourceAcronym=%7B%7D&sourceAcronymContains=%7B%7D&sourceId=%7B%7D&sourceName=%7B%7D&sourceNameContains=%7B%7D&sourceUrl=%7B%7D&sourceUrlContains=%7B%7D&syndicationCapturedBeforeDate=%7B%7D&syndicationCapturedInRange=%7B%7D&syndicationCapturedSinceDate=%7B%7D&syndicationUpdatedBeforeDate=%7B%7D&syndicationUpdatedInRange=%7B%7D&syndicationUpdatedSinceDate=%7B%7D&syndicationVisibleBeforeDate=%7B%7D&syndicationVisibleInRange=%7B%7D&syndicationVisibleSinceDate=%7B%7D&tagIds=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of MediaItems matching the specified query parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "894a7cd6-5bc8-4e37-ac80-e14f844791d1"
            }
          ]
        },
        {
          "id": "13cd6229-8c36-4bff-85fa-9e0753131310",
          "name": "getFeaturedMedia",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/media/featured.json?max=%7B%7D&offset=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of featured content in the syndication system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dce02ae9-876c-4f46-9156-924c917e192e"
            }
          ]
        },
        {
          "id": "49c75589-ed06-4e8c-a316-c18caeafaa55",
          "name": "getMostPopularMedia",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/media/mostPopularMedia.json?max=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of MediaItems with the highest ratings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca96e362-8360-4069-9814-6a9a728a6833"
            }
          ]
        },
        {
          "id": "dfdfbab3-8d7b-4af6-88af-4411b583a72b",
          "name": "searchMedia",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/media/searchResults.json?max=%7B%7D&offset=%7B%7D&q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of MediaItems matching the search query 'q'.The search query 'q' is a Lucene query.The syntax for a Lucene query can be found here"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9db175f6-3386-4e6f-96aa-b30053219422"
            }
          ]
        },
        {
          "id": "5f0286c0-c070-4d50-a989-1bcbb845a1fe",
          "name": "getMediaById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the MediaItem identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "046cdc82-de4f-465c-8066-748f8d697038"
            }
          ]
        },
        {
          "id": "f1f6bb2d-123d-4ede-b098-393c3af56342",
          "name": "getMediaContentById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id/content"
              ],
              "query": [
                {
                  "key": "calledByBuild",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the raw content (html, image, etc...) for the MediaItem identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c14b48d-5187-4ad1-834d-78d385fb6e43"
            }
          ]
        },
        {
          "id": "7e084df9-80e6-40be-9d98-7fe359c66148",
          "name": "getMediaEmbedById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id/embed.json"
              ],
              "query": [
                {
                  "key": "displayMethod",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "divId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "excludeDiv",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "excludeJquery",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "flavor",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "height",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "iframeName",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "width",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the javascript or iframe embed code for the MediaItem identified by 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "575df259-a956-484c-a65e-8a46b900c3bf"
            }
          ]
        },
        {
          "id": "3977bb5f-8511-43b0-9f77-76f04b41387f",
          "name": "getMediaPreviewById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id/preview.jpg"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the JPG preview, where applicable, for the MediaItem identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cedaa65-79a2-4203-9a24-1a25d94b974a"
            }
          ]
        }
      ]
    }
  ]
}