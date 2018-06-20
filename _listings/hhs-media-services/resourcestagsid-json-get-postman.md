{
  "info": {
    "name": "HHS Media Services Get Tag by ID",
    "_postman_id": "79742d0b-8fef-4683-aedc-4bf0d42efea5",
    "description": "Returns the Tag identified by the 'id' in the specified 'format'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "5cee737f-4da1-4135-ad5e-a38fc56a1be0",
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
              "id": "9a083333-61ef-4d7c-9ac1-a140f49b690c"
            }
          ]
        },
        {
          "id": "f09fbba5-f432-4843-8d5f-79fae7b567ed",
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
              "id": "04c12f49-ff65-4090-8a5e-e5b58a4350b5"
            }
          ]
        },
        {
          "id": "8e9ac25a-2988-4ed9-bad0-e4d781273c02",
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
              "id": "65306d61-2b54-4371-9547-4fa57851d4e4"
            }
          ]
        },
        {
          "id": "f8d09bbb-c73d-4ea3-8a23-264cd336a1c0",
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
              "id": "a37d225b-8263-4411-a7ac-37f47ca17537"
            }
          ]
        },
        {
          "id": "a7c1515a-e19c-4d00-8a8f-14390e33d778",
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
              "id": "05d331a7-ae91-4906-a3b1-8d8155984fd4"
            }
          ]
        },
        {
          "id": "46bc436a-a7f9-4c1f-b218-210a8e4f6bd3",
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
              "id": "1c3797db-d69e-467d-89ee-b1fc153c4749"
            }
          ]
        },
        {
          "id": "ec305365-10d1-4396-9b41-4e9d90bc1936",
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
              "id": "ab1b571b-6f6a-47e5-b05d-695d1d0a5fca"
            }
          ]
        },
        {
          "id": "3a9ac749-53f0-4ef3-abaf-b0de6c3d6403",
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
              "id": "6ca5a35d-8ee5-46b4-903c-403e49347861"
            }
          ]
        },
        {
          "id": "f55c8027-9f0c-4153-8ede-50a9a6966c95",
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
              "id": "d58d8ed4-4ca1-41d1-aaa1-c59ebc58ec73"
            }
          ]
        },
        {
          "id": "f2b56978-9ee8-480b-b817-5b848fd65c2b",
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
              "id": "b21dc3c0-2549-42d0-b866-5435f4ca9390"
            }
          ]
        },
        {
          "id": "7e754794-9367-431d-883c-a371311f40c6",
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
              "id": "1cf02332-0c96-4183-b6fa-32b5d964fe81"
            }
          ]
        },
        {
          "id": "006017db-bd4e-4283-a314-9362e62ae498",
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
              "id": "ec3fdc0f-9dcf-44c4-938e-7b2922a6898e"
            }
          ]
        },
        {
          "id": "a996d523-9f2d-4d36-9a67-2b44b63299bd",
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
              "id": "afdcab99-f5fb-4951-8f80-450c679e3579"
            }
          ]
        },
        {
          "id": "fc690275-36d4-447b-a0cf-ad788818e83d",
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
              "id": "2c32a8ee-ee44-4313-8c19-fcf19d79345b"
            }
          ]
        },
        {
          "id": "1e330de9-9130-41dd-a709-8a907de0551f",
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
              "id": "0b0d9e64-7cc8-466b-bb49-0f0694160cd4"
            }
          ]
        },
        {
          "id": "25f056e9-e165-498e-a71c-5ae9f54fa695",
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
              "id": "2c1893de-c63a-4f9a-be31-dfd208ffb093"
            }
          ]
        },
        {
          "id": "0ae99764-fb43-41a6-a2ba-51a456ebb9c1",
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
              "id": "c0c358cf-cdb3-4e37-83db-1843d0ec540a"
            }
          ]
        },
        {
          "id": "b290861b-f513-4c2e-8a07-98cf06348bbb",
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
              "id": "9449e529-3962-445c-90b8-f54e3855ba6b"
            }
          ]
        },
        {
          "id": "5908cf3d-fe40-405d-9591-fe0e5faed7dc",
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
              "id": "07ffe034-23ad-4849-afb0-fedcd9a4944f"
            }
          ]
        },
        {
          "id": "5963885f-b050-4839-96ff-f61793d18ac0",
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
              "id": "a75c8f2c-d415-45e4-b018-fbc287efe6d5"
            }
          ]
        },
        {
          "id": "d2a7828f-9d5f-44f5-bee1-034455f64a10",
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
              "id": "7cf841e0-49aa-4a27-9e3e-3d3bdbe3498d"
            }
          ]
        },
        {
          "id": "0539bd32-ff4e-4c3c-ba13-704403c690ca",
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
              "id": "0c0f2725-bb25-4cf5-8201-98c0ac3df3fe"
            }
          ]
        },
        {
          "id": "7934f0f0-2370-4e3a-9aa2-6339776f1301",
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
              "id": "2a915a25-7117-47b6-aa8d-897c0775f3bf"
            }
          ]
        },
        {
          "id": "32171db4-bc23-4e54-aa64-44a5b78f0b0f",
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
              "id": "a4d97ca3-6bbf-4eca-83bb-ab2ba8946873"
            }
          ]
        },
        {
          "id": "605c13ca-de8e-46cf-ae0c-d6e28a42e423",
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
              "id": "6df6a836-3188-4c5c-a2ec-d128b019bdd2"
            }
          ]
        },
        {
          "id": "5eb606eb-230b-4ccb-b59c-e78d5f5b1c1b",
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
              "id": "e5ecc4f4-981f-46a9-aef8-ce63f38667c2"
            }
          ]
        },
        {
          "id": "ffb11dc5-8196-4f39-b287-81c2fb4638c1",
          "name": "getTagTypes",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/tags/tagTypes.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of TagTypes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c6c4506-2b56-4aee-a15c-f96839b0e922"
            }
          ]
        },
        {
          "id": "08117d36-7bb6-4d3b-b636-6ff7b04557f1",
          "name": "getTagById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/tags/:id.json"
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
            "description": "Returns the Tag identified by the 'id' in the specified 'format'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d72e3d5f-02dc-4de5-81a7-e75df68ab51a"
            }
          ]
        }
      ]
    }
  ]
}