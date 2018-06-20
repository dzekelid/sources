{
  "info": {
    "name": "HHS Media Services Get TagTypes",
    "_postman_id": "8aacf0d5-d724-46d9-9b39-0a3bb985b5ad",
    "description": "Returns the list of TagTypes",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "5857ddfa-7bf9-4a52-a2f6-d55afb4314c3",
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
              "id": "4c065a65-0ad3-4021-aee8-d3deb2706faa"
            }
          ]
        },
        {
          "id": "da258446-7b9e-4dc7-97cb-ee854ce4371f",
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
              "id": "6b0ad2d4-37ff-4243-814f-5825f41265d7"
            }
          ]
        },
        {
          "id": "fa1986d6-65b8-4ac5-9588-6b3b610d17c0",
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
              "id": "2094005d-8cba-4232-a178-d739e3e85ce7"
            }
          ]
        },
        {
          "id": "0458f5ed-e120-4234-934d-62f1d983d9f4",
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
              "id": "2da63c11-53ee-4138-ba17-3ff11bf9a763"
            }
          ]
        },
        {
          "id": "b787e949-0bb9-4c3c-a6cb-6aa06d10fe6c",
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
              "id": "69e06e42-868a-45e1-a75b-459d88caacef"
            }
          ]
        },
        {
          "id": "4f01cf7f-9fd9-42d8-8fc1-8de1a5e73bdf",
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
              "id": "20ead690-ac55-4a07-891f-fbde834bfa8c"
            }
          ]
        },
        {
          "id": "9efb1d90-1c5d-442f-9393-1377db8b0537",
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
              "id": "dd645839-5535-4354-a5cc-0ef41158a57c"
            }
          ]
        },
        {
          "id": "b8915be1-fc9d-4bcf-8ebc-0dde52eb4fae",
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
              "id": "3ef57ba4-fd63-436e-9982-39e94c18e228"
            }
          ]
        },
        {
          "id": "d4da257f-c52e-4e3b-bf28-724989304776",
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
              "id": "aa6a2817-ecd5-42bb-9935-0297fecd8329"
            }
          ]
        },
        {
          "id": "35047904-76fd-416d-9935-904e8e4ea74b",
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
              "id": "bf518534-c961-45f0-893a-31b269d7565a"
            }
          ]
        },
        {
          "id": "7571a430-cceb-441f-b07f-3a7bb8d6bdef",
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
              "id": "07a2d366-a679-493a-8d23-584071ec3938"
            }
          ]
        },
        {
          "id": "78a61dab-923b-478e-86b1-eff401a6b3eb",
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
              "id": "855c23fe-5da6-48f3-a4ac-bda33b72a780"
            }
          ]
        },
        {
          "id": "8ce95352-777d-4527-8be1-00c7dc54c0d0",
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
              "id": "b6f12e65-ee4a-49f6-a457-ad900da2290f"
            }
          ]
        },
        {
          "id": "0f6cc5a4-71a7-4f23-80a7-ee45627d0965",
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
              "id": "012a35bc-93db-410c-b403-834b9c817ce9"
            }
          ]
        },
        {
          "id": "28b5adab-f295-4bef-a645-02cb0b3478ee",
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
              "id": "3fb30266-da38-4dac-9788-3c38f110cffe"
            }
          ]
        },
        {
          "id": "28d03c3a-e0e1-4c99-9589-2b038e51a20d",
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
              "id": "f03ab53d-34c8-4ab8-abc7-e75c2cf06dff"
            }
          ]
        },
        {
          "id": "45902497-f1c5-4921-8150-b0ffdcf2497c",
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
              "id": "3e30ba4c-529c-4614-b957-a4e8416f8444"
            }
          ]
        },
        {
          "id": "0862281b-e203-4d08-a128-9622ecdc4c72",
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
              "id": "9f8789fb-694c-4bda-ab87-3374b2959375"
            }
          ]
        },
        {
          "id": "f508389c-03d9-47b2-b672-7a70d2239d98",
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
              "id": "01ad87e8-267d-4c41-ae88-a376d7f33f69"
            }
          ]
        },
        {
          "id": "c159d48a-6d5e-4bfb-a08e-1080dd5c6f1d",
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
              "id": "fccc7eed-95e7-479b-8ba3-5c9e55acaab5"
            }
          ]
        },
        {
          "id": "1e100b41-454d-4f63-9963-7ce8f303eca6",
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
              "id": "92735419-7670-43ee-ae6a-77706320c4f1"
            }
          ]
        },
        {
          "id": "75b7db8a-4fec-4d9a-8e01-e8035c0cd1da",
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
              "id": "6fd7e278-d7ef-4f71-8277-842e2ef9f20a"
            }
          ]
        },
        {
          "id": "ab92e047-27bc-4fd8-a54c-11c83b33ba6a",
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
              "id": "2dd74bbf-2533-40dd-aca1-c4a6d5e3aefd"
            }
          ]
        },
        {
          "id": "24e695eb-f7db-4cc0-8dfb-5607891dfa3c",
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
              "id": "1b455862-27f7-47fa-bd21-13fe18cb6fe1"
            }
          ]
        },
        {
          "id": "430b63f7-12f7-4068-aafd-3a78b77734ee",
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
              "id": "75919665-0e2a-4f42-ac62-0fab68a4700a"
            }
          ]
        },
        {
          "id": "f609f2d6-24b7-4c4b-bce5-a2645319de5f",
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
              "id": "a5a15e9c-7ebb-47df-9e19-c6844ed339ce"
            }
          ]
        },
        {
          "id": "c2a88a92-35d8-4060-9ddd-252f24613a0a",
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
              "id": "43924987-3bb4-4bd1-98f9-ab712717bc26"
            }
          ]
        }
      ]
    }
  ]
}