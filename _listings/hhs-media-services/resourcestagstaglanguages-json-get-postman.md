{
  "info": {
    "name": "HHS Media Services Get TagLanguages",
    "_postman_id": "043f40f9-e043-4353-950c-dfdbdbc5939e",
    "description": "Returns the list of TagLanguages",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "8b9bcd43-42b1-4d9d-9cde-c46d6a5b6e61",
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
              "id": "fe9c3d03-a1e5-4b32-aca4-6a4f598ebf3f"
            }
          ]
        },
        {
          "id": "4e15bb77-be1a-499e-ac6b-9b01bd5eb269",
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
              "id": "7ca6a6a1-dfb4-4b6d-9da0-061712a0fcd4"
            }
          ]
        },
        {
          "id": "cc97d996-eec0-4bed-a8e8-b7e7e8ede8a7",
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
              "id": "a54f7991-e778-457a-b310-2a827d88fe6d"
            }
          ]
        },
        {
          "id": "202c0315-65ba-432c-a28f-357efe9ce6a0",
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
              "id": "7fee53ed-98a3-4093-b4c4-9b03c25e0d03"
            }
          ]
        },
        {
          "id": "8401ff68-b370-4e9a-8553-51e2139925a7",
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
              "id": "03407af8-cc4e-4340-8cff-e635f5e9ca24"
            }
          ]
        },
        {
          "id": "dc7a3699-a4ed-4c01-8817-bddac27aef48",
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
              "id": "1487fbdc-00c8-48cf-9621-9a72f65095de"
            }
          ]
        },
        {
          "id": "d1a5bed6-f04f-44ae-a98b-f80619a2eb11",
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
              "id": "cd18969e-47d4-4122-8525-e0b81041a68c"
            }
          ]
        },
        {
          "id": "28dcd573-5e13-49fc-94da-381c007b5317",
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
              "id": "bd155a08-8c46-4f75-8edd-01d3418bba4b"
            }
          ]
        },
        {
          "id": "5b7204fa-20d2-48b5-9b0b-d443a3d10f73",
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
              "id": "171c7341-32c4-461e-a5e9-c938908e62b8"
            }
          ]
        },
        {
          "id": "d9aab406-d681-4b53-aa69-7cd76527e433",
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
              "id": "384a24b6-e65b-4ca3-8cef-54d085263656"
            }
          ]
        },
        {
          "id": "136671c3-d78c-4871-8c35-97d0208f4ea6",
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
              "id": "4cc7576d-3347-442d-af38-5b612b4c9e65"
            }
          ]
        },
        {
          "id": "f0224299-b33d-4db5-ae28-d68315863310",
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
              "id": "62697bbd-54fb-4fbc-b52c-3a57a7fd964f"
            }
          ]
        },
        {
          "id": "dc752fd2-530c-4cef-98a2-92bcb2e4e132",
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
              "id": "a147e005-f9d1-4b57-a27d-bb2dd9f1bd68"
            }
          ]
        },
        {
          "id": "6d8352a6-f04a-441c-b07c-ff5098a6c121",
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
              "id": "32a8d22e-b997-4e92-9ac2-c202e1bdccd4"
            }
          ]
        },
        {
          "id": "1fefcd8a-571c-4543-904d-56c5d02b7083",
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
              "id": "66b312dc-c55b-46a4-a37c-da9ecd0fe770"
            }
          ]
        },
        {
          "id": "9208a238-45df-466c-ae92-c8739937b716",
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
              "id": "222fef89-50b7-40a7-a34d-f4fe0027ed73"
            }
          ]
        },
        {
          "id": "047ca044-08db-440a-a6cf-fdc3934f059f",
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
              "id": "5500050b-aead-419e-a4bc-08f81e85518b"
            }
          ]
        },
        {
          "id": "2781d969-04d5-4acf-8713-62bd47531332",
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
              "id": "218a0742-c7c7-4df2-9b0a-eacaab39e18e"
            }
          ]
        },
        {
          "id": "a9bdf55a-6cea-4a5e-98cd-83ed94a55522",
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
              "id": "c8831bc7-5ef5-4edc-a10b-63dea1fb881a"
            }
          ]
        },
        {
          "id": "a3b64587-0b47-43a0-8baa-be45b5440e3a",
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
              "id": "81bebad5-cee0-45f2-b739-d97e42e6d3de"
            }
          ]
        },
        {
          "id": "e80a4288-e1ee-4a1c-b51f-64c5ba2758b1",
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
              "id": "ad439251-d416-4eac-8b82-f0146d6a26d8"
            }
          ]
        },
        {
          "id": "34e4ea60-1253-46b9-9002-483b8c0277ed",
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
              "id": "1acc52f3-c15f-4a18-81fd-1efdb3b5a1b3"
            }
          ]
        },
        {
          "id": "b11c0eb8-5807-4526-99d6-4a8c69f39a93",
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
              "id": "9a87f551-2f7f-415e-8a5c-a4d05816a605"
            }
          ]
        },
        {
          "id": "ab696232-971c-4e7b-849a-c2697f3e0eb1",
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
              "id": "342a4b08-805a-4ed6-92f7-abfd8edd8214"
            }
          ]
        },
        {
          "id": "6d3386f1-e083-45ae-8a6e-a7ab735b04e2",
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
              "id": "eedeea3b-9400-40fd-a409-e3d6b0c3259f"
            }
          ]
        },
        {
          "id": "d3d25b1e-221e-4f9c-ae7c-fc1f9904a197",
          "name": "getTagLanguages",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/tags/tagLanguages.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of TagLanguages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b18043fe-12a2-4872-b846-e3e20748f221"
            }
          ]
        }
      ]
    }
  ]
}