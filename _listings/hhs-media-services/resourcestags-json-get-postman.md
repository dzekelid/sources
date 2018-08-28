{
  "info": {
    "name": "HHS Media Services Get Tags",
    "_postman_id": "ae1e5efc-a52a-4893-81a7-a739ddf5c6ee",
    "description": "Returns the list of Tags matching the specified query parameters in the specified 'format'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "7db1628e-5699-4f17-8174-bdfa7537b8c1",
          "name": "getResources",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources.json?q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of Resources matching the search query 'q'.The search query 'q' is a Lucene query.The syntax for a Lucene query can be found here."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0666db4-6ae7-45f5-a9f9-b09ec43d79f4"
            }
          ]
        },
        {
          "id": "d3c3366b-81bb-4eaa-881d-620b7707f257",
          "name": "getCampaigns",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/campaigns.json?max=%7B%7D&offset=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of Campaigns."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0ca8f99-3a17-4e17-bacc-459a626d0fbd"
            }
          ]
        },
        {
          "id": "1c6f7be7-c056-492d-aed6-2f12b76a6856",
          "name": "getCampaignById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/campaigns/:id.json"
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
            "description": "Returns the Campaign identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ba93f9b-e5df-4077-8d96-99572e70e25c"
            }
          ]
        },
        {
          "id": "cedfc458-f046-4bf7-be26-1e922f754e7f",
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
              "id": "e757751d-9ebe-4f15-9bf2-ea65abec0e07"
            }
          ]
        },
        {
          "id": "d69dc302-2083-4da9-b4ce-5bd818099a8a",
          "name": "renders-the-list-of-mediaitems-associated-with-the-campaign-identified-by-the-id-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/campaigns/:id/syndicate.json"
              ],
              "query": [
                {
                  "key": "displayMethod",
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
            "description": "Renders the list of MediaItems associated with the Campaign identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c741fb20-075f-428c-9a15-04a4f7f92d60"
            }
          ]
        },
        {
          "id": "31e4e150-1638-4cf0-aeae-f5b719409983",
          "name": "getLanguages",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/languages.json?max=%7B%7D&offset=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list Languages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ffd4fe0-ce9e-4db9-9270-5f49551d8467"
            }
          ]
        },
        {
          "id": "d979b9a5-5dee-428f-889e-17186ec273c6",
          "name": "getLanguageById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/languages/:id.json"
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
            "description": "Returns the Language identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de5c0a73-84f8-40f5-9908-fe0e5d5e98ca"
            }
          ]
        },
        {
          "id": "16205fbd-af8e-4feb-9a3f-3a9cc9dc4da0",
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
              "id": "e88a87e2-b769-4406-9f29-c7decf676215"
            }
          ]
        },
        {
          "id": "cd8363c1-7f63-417e-a59d-dcf939e912e7",
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
              "id": "67179249-d51b-4cbb-bdcf-b5c8c2a9d23a"
            }
          ]
        },
        {
          "id": "46f97b51-99e2-407d-8903-9f753feb4b62",
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
              "id": "448b70c8-61e9-4339-9106-cc5341c73706"
            }
          ]
        },
        {
          "id": "007ca034-5713-42bd-b2be-7c8bbed034e0",
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
              "id": "8ad2f349-6eb8-49d5-b9df-bfc223eb1d38"
            }
          ]
        },
        {
          "id": "cc3925df-82b8-4dcd-8773-0ab08cad6d6f",
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
              "id": "f9b4d1f8-c8b8-42e9-85d9-8e60590b8c9d"
            }
          ]
        },
        {
          "id": "6a72c622-546c-4041-85a4-b7c01cfa1fe1",
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
              "id": "a153cc0b-652a-4b71-ba5b-0377f459c79b"
            }
          ]
        },
        {
          "id": "1a695816-f079-427b-b057-4bbd6fd9f47d",
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
              "id": "3482c2ed-87b3-41ec-a89d-7c0caeea4b74"
            }
          ]
        },
        {
          "id": "dac6f0c1-a6c1-41cf-b7f0-f351d707eea0",
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
              "id": "8534b69f-27bc-4889-a862-5c1db25ecd90"
            }
          ]
        },
        {
          "id": "ef2b6f36-159a-4959-93c5-fe7a46a747d1",
          "name": "getMediaRatingsById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id/ratings.json"
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
            "description": "Get the Ratings (number of 'likes') for the MediaItem identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "609772bd-e50c-4cd0-8b49-5b601d6cacdd"
            }
          ]
        },
        {
          "id": "7e27dd5d-d77f-4b28-bd61-a7e1c51ec1cc",
          "name": "getRelatedMediaById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id/relatedMedia.json"
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
            "description": "Returns the list of MediaItems related to the MediaItem identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29a73b8f-c4a5-4918-96ee-29d2ff71bc5f"
            }
          ]
        },
        {
          "id": "2af9ee8b-2e1d-4999-abdb-6bc544da0ab9",
          "name": "getMediaSyndicateById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id/syndicate.json"
              ],
              "query": [
                {
                  "key": "autoplay",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "cssClass",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "font-size",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "imageFloat",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "imageMargin",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rel",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "stripBreaks",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "stripClasses",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "stripImages",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "stripScripts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "stripStyles",
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
            "description": "Returns the syndicated content for a given MediaItem in the specified 'format' (HTML or JSON)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6833bf4e-5151-487a-9364-cfa1ba8b37bc"
            }
          ]
        },
        {
          "id": "8579427d-d333-47ae-96f1-f452180c5fd1",
          "name": "getMediaThumbnailById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id/thumbnail.jpg"
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
            "description": "Returns the JPG thumbnail, where applicable, for the MediaItem identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5185307-4c26-40bb-9b2a-8235900c3eae"
            }
          ]
        },
        {
          "id": "3d11144c-f7bb-4eae-8d96-1782fff2b572",
          "name": "getMediaYoutubeMetaDataById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/media/:id/youtubeMetaData.json"
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
            "description": "Returns the Youtube metadata, where applicable, for the MediaItem identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "728aeaf1-004b-48bf-b0aa-ac4522dc5055"
            }
          ]
        },
        {
          "id": "9cb4ffe7-c272-4b58-bcc4-a40d5efc9ea5",
          "name": "getMediaTypes",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/mediaTypes.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of available MediaTypes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "590d6c90-d477-41a3-8968-84c3805ad2fc"
            }
          ]
        },
        {
          "id": "b8fb551a-e566-4558-bb93-e851e6fecec7",
          "name": "getSources",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/sources.json?max=%7B%7D&offset=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of Sources."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b36c323-d00a-474d-b644-bb142498a5d3"
            }
          ]
        },
        {
          "id": "0154c486-bfdd-4cbe-a74e-6c3e4ed74c0d",
          "name": "getSourceById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/sources/:id.json"
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
            "description": "Returns the Source identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ae12a03-5513-4cb4-9e29-4ba1767ad858"
            }
          ]
        },
        {
          "id": "ce7d2a66-a7ee-4b8e-a643-863315a44aab",
          "name": "renders-the-list-of-mediaitems-associated-with-the-source-identified-by-the-id-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/sources/:id/syndicate.json"
              ],
              "query": [
                {
                  "key": "displayMethod",
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
            "description": "Renders the list of MediaItems associated with the Source identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d2c610a-2e10-4183-8d3a-c54e24c51117"
            }
          ]
        },
        {
          "id": "a86ace24-fd64-4f68-bd8a-f7ae664e5a3e",
          "name": "getTags",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/tags.json?max=%7B%7D&mediaId=%7B%7D&name=%7B%7D&nameContains=%7B%7D&offset=%7B%7D&sort=%7B%7D&typeId=%7B%7D&typeName=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of Tags matching the specified query parameters in the specified 'format'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8efbc50-0a08-417a-a58e-4209d58ce665"
            }
          ]
        }
      ]
    }
  ]
}