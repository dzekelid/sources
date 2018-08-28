{
  "info": {
    "name": "HHS Media Services Get MediaItems for Tag",
    "_postman_id": "fd057dc5-37fc-4723-963c-ffd9d9ebd752",
    "description": "Renders the list of MediaItems associated with the Tag identified by the 'id'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "fafd2176-ee2a-4ded-af1a-819a0f1cc46f",
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
              "id": "2d837b53-0b7f-400b-84f8-83867c7559e2"
            }
          ]
        },
        {
          "id": "18b0ac45-6d5b-4f66-b5ae-1010b823624e",
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
              "id": "1dd4e534-d068-48c9-9479-db2aed58cff0"
            }
          ]
        },
        {
          "id": "561c7e34-1c5e-4492-934b-73da79d26bd1",
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
              "id": "7936ec50-bca9-4014-bf5a-00211bdbd50f"
            }
          ]
        },
        {
          "id": "d77e9a98-893a-4ab0-a26f-9fe33e2c7c99",
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
              "id": "3bad846e-dc26-4635-b4bf-3652a98fa49e"
            }
          ]
        },
        {
          "id": "d9990879-568a-436c-9484-2794327a996d",
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
              "id": "289303e5-1f9c-4527-ad09-97559b5d332a"
            }
          ]
        },
        {
          "id": "5c203515-a10c-4415-910f-6aa7e8a6682f",
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
              "id": "defb15f4-4bd0-44e8-94ea-6882df1a249a"
            }
          ]
        },
        {
          "id": "12d08b83-d4ee-4955-80de-9adc34e46ea1",
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
              "id": "08fb9cac-616c-4a9d-a281-5455f0eb18c2"
            }
          ]
        },
        {
          "id": "b666f990-b936-46ce-aabb-d490efb9ed96",
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
              "id": "7db4e68a-3363-4b8c-b6c8-5e45422bf90b"
            }
          ]
        },
        {
          "id": "3fa378e8-dfa5-40d1-a807-6cf02f248d39",
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
              "id": "256c4646-ad42-41f5-adcd-eea05c526ef7"
            }
          ]
        },
        {
          "id": "205bf5cc-08a7-4c0b-8463-3cb17b38893f",
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
              "id": "cc3ab520-8692-4b85-acd3-7679b78a7258"
            }
          ]
        },
        {
          "id": "c22cd5ef-2b34-498f-9014-197d26a22402",
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
              "id": "f7694f45-ba40-4d37-872e-5f5c189fcb00"
            }
          ]
        },
        {
          "id": "722281af-64f5-4d66-a24a-2e3833475a07",
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
              "id": "e267f961-60ae-482e-a82f-4d341808d503"
            }
          ]
        },
        {
          "id": "1ae321d5-4936-4d2f-bf68-26d3f98ccc18",
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
              "id": "1309c6be-6cea-421d-85c6-0d6655dc4076"
            }
          ]
        },
        {
          "id": "ece295e1-cf57-484b-b7b1-484e6a1f5037",
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
              "id": "7f1111d0-d2d9-4eaf-9ef5-2c08fab4a0cf"
            }
          ]
        },
        {
          "id": "10e4bdd0-c6c9-42fb-b9f5-0af32b1eaddd",
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
              "id": "5b92322d-e17b-4b24-9ec4-b9ee555e75a4"
            }
          ]
        },
        {
          "id": "07ca402a-678a-4926-a27f-d9b914aca1f6",
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
              "id": "15dbeb37-52dc-4f1e-8c11-7debdae517d1"
            }
          ]
        },
        {
          "id": "df9adce8-8e0a-41e3-9c37-e0405d976d79",
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
              "id": "c1dc94c3-1fc5-4245-8e00-9e8199baae73"
            }
          ]
        },
        {
          "id": "fc91d292-8954-4d12-a479-aadc0f5421ef",
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
              "id": "26c5c38e-118b-4be6-825c-a7e24a3bd7a4"
            }
          ]
        },
        {
          "id": "36a7c372-6f1e-48bd-84e6-e27339e9771d",
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
              "id": "b427aab2-30c7-4aa3-8c77-8c8324da1731"
            }
          ]
        },
        {
          "id": "683de306-b727-471b-9a1d-ed7a9edab3b5",
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
              "id": "8b0eb729-5476-4613-b746-720c3e65b937"
            }
          ]
        },
        {
          "id": "b9bf0cbe-07c6-4a3f-b924-e6f9e9300329",
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
              "id": "2135de83-1ab4-4e96-8b76-9eb1acbe4297"
            }
          ]
        },
        {
          "id": "fc311661-7d7c-4610-8477-f91ac6bb17e6",
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
              "id": "0204beba-c1d8-4c6d-a4db-e09e2b85907e"
            }
          ]
        },
        {
          "id": "edd38ba9-5d7a-4685-a1c1-20ca02857a3f",
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
              "id": "0f40d3e0-846c-4719-a01c-4dc04eb2fbf8"
            }
          ]
        },
        {
          "id": "c89d2040-9ae8-46f4-9951-0a75ffa6f5f1",
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
              "id": "1c45e9b5-5d74-427a-a9c3-e469ead38971"
            }
          ]
        },
        {
          "id": "8f6ed65d-6403-4248-926e-5de6b717ac2a",
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
              "id": "952c9e2f-66fc-4abf-9215-473ca98779d0"
            }
          ]
        },
        {
          "id": "def0525d-42e0-418a-9da2-618ad4995409",
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
              "id": "82e7eb85-36af-408e-b62f-ad4db10b0ade"
            }
          ]
        },
        {
          "id": "45c9a823-02c5-481c-b6ee-63f3fd3f4370",
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
              "id": "b31a256e-0246-4186-b403-bb8500c6b164"
            }
          ]
        },
        {
          "id": "ff7f8de9-66e1-412d-a063-7b8fb7dd974a",
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
              "id": "40ea2946-059c-4496-8e95-115511934de0"
            }
          ]
        },
        {
          "id": "6b8db93c-fd9a-4fe4-bef8-6cf579321163",
          "name": "getMediaByTagId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/tags/:id/media.json"
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
            "description": "Returns the list of MediaItems associated with the Tag identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48c93f8f-65c5-443c-be75-1bfa6c2da023"
            }
          ]
        },
        {
          "id": "848cd4c9-8580-49a7-a035-404b366bc566",
          "name": "getRelatedTagsById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/tags/:id/related.json"
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
            "description": "Returns the list of Tags related to the Tag identified by the 'id' in the specified format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65003837-c68c-4b5f-878f-d2f4e3a136fc"
            }
          ]
        },
        {
          "id": "9ddffc91-a916-4824-bd63-4cd4eb687e70",
          "name": "renders-the-list-of-mediaitems-associated-with-the-tag-identified-by-the-id-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.digitalmedia.hhs.gov",
              "path": [
                "api",
                "v2",
                "resources/tags/:id/syndicate.json"
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
            "description": "Renders the list of MediaItems associated with the Tag identified by the 'id'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "864db5bd-5cb6-487b-9340-3007af520ac2"
            }
          ]
        }
      ]
    }
  ]
}