---
swagger: "2.0"
x-collection-name: HHS Media Services
x-complete: 0
info:
  title: HHS Media Services Get related MediaItems by ID
  description: Returns the list of MediaItems related to the MediaItem identified
    by the 'id'.
  termsOfService: http://www.hhs.gov/web/socialmedia/policies/tos.html#ready
  version: "2"
host: api.digitalmedia.hhs.gov
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /resources.json:
    get:
      summary: Get Resources by search query
      description: Returns the list of Resources matching the search query 'q'.The
        search query 'q' is a Lucene query.The syntax for a Lucene query can be found
        here.
      operationId: getResources
      x-api-path-slug: resources-json-get
      parameters:
      - in: query
        name: q
        description: The search query supplied by the user
      responses:
        200:
          description: OK
      tags:
      - Resources
  /resources/campaigns.json:
    get:
      summary: Get Campaigns
      description: Returns the list of Campaigns.
      operationId: getCampaigns
      x-api-path-slug: resourcescampaigns-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: '* Set of fields to sort the records by'
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Campaigns
  /resources/campaigns/{id}.json:
    get:
      summary: Get Campaign by ID
      description: Returns the Campaign identified by the 'id'.
      operationId: getCampaignById
      x-api-path-slug: resourcescampaignsid-json-get
      parameters:
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Campaigns
      - Id
  /resources/campaigns/{id}/media.json:
    get:
      summary: Get MediaItems by Campaign ID
      description: Returns the list of MediaItems for the Campaign identified by the
        'id'.
      operationId: getMediaByCampaignId
      x-api-path-slug: resourcescampaignsidmedia-json-get
      parameters:
      - in: path
        name: id
        description: The id of the campaign to find media items for
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: The name of the property to which sorting will be applied
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Campaigns
      - Id
      - Media
  /resources/campaigns/{id}/syndicate.json:
    get:
      summary: Get MediaItems for Campaign
      description: Renders the list of MediaItems associated with the Campaign identified
        by the 'id'.
      operationId: renders-the-list-of-mediaitems-associated-with-the-campaign-identified-by-the-id-
      x-api-path-slug: resourcescampaignsidsyndicate-json-get
      parameters:
      - in: query
        name: displayMethod
        description: Method used to render an html request
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Campaigns
      - Id
      - Syndicate
  /resources/languages.json:
    get:
      summary: Get Languages
      description: Returns the list Languages.
      operationId: getLanguages
      x-api-path-slug: resourceslanguages-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: '* Set of fields to sort the records by'
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Languages
  /resources/languages/{id}.json:
    get:
      summary: Get Language by ID
      description: Returns the Language identified by the 'id'.
      operationId: getLanguageById
      x-api-path-slug: resourceslanguagesid-json-get
      parameters:
      - in: path
        name: id
        description: The id of the language to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Languages
      - Id
  /resources/media.json:
    get:
      summary: Get MediaItems
      description: Returns the list of MediaItems matching the specified query parameters.
      operationId: getMedia
      x-api-path-slug: resourcesmedia-json-get
      parameters:
      - in: query
        name: collectionId
        description: Restrict filtering to media items in a specific collection
      - in: query
        name: contentAuthoredBeforeDate
        description: Find all media items authored before the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentAuthoredInRange
        description: Find all media items authored between the provided start and
          end days (RFC 3339, comma separated, time ignored)
      - in: query
        name: contentAuthoredSinceDate
        description: Find all media items authored since the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentPublishedBeforeDate
        description: Find all media items published before the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentPublishedInRange
        description: Find all media items published between the provided start and
          end days (RFC 3339, comma separated, time ignored)
      - in: query
        name: contentPublishedSinceDate
        description: Find all media items published since the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentReviewedBeforeDate
        description: Find all media items reviewed before the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentReviewedInRange
        description: Find all media items reviewed between the provided start and
          end days (RFC 3339, comma separated, time ignored)
      - in: query
        name: contentReviewedSinceDate
        description: Find all media items reviewed since the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentUpdatedBeforeDate
        description: Find all media items updated before the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentUpdatedInRange
        description: Find all media items updated between the provided start and end
          days (RFC 3339, comma separated, time ignored)
      - in: query
        name: contentUpdatedSinceDate
        description: Find all media items updated since the provided day (RFC 3339,
          time ignored)
      - in: query
        name: createdBy
        description: Find all media items containing the createdBy value
      - in: query
        name: customThumbnailUrl
        description: Find all media items which have the provided customThumbnailUrl,
          case insensitive
      - in: query
        name: customThumbnailUrlContains
        description: Find all media items which contain the provided partial customThumbnailUrl,
          case insensitive
      - in: query
        name: dateContentAuthored
        description: Find all media items authored on the provided day (RFC 3339,
          time ignored)
      - in: query
        name: dateContentPublished
        description: Find all media items published on the provided day (RFC 3339,
          time ignored)
      - in: query
        name: dateContentReviewed
        description: Find all media items reviewed on the provided day (RFC 3339,
          time ignored)
      - in: query
        name: dateContentUpdated
        description: Find all media items updated on the provided day (RFC 3339, time
          ignored)
      - in: query
        name: dateSyndicationCaptured
        description: Find all media items authored on the provided day (RFC 3339,
          time ignored)
      - in: query
        name: dateSyndicationUpdated
        description: Find all media items updated on the provided day, (RFC 3339,
          time ignored)
      - in: query
        name: descriptionContains
        description: Find all media items containing the provided partial description,
          case insensitive
      - in: query
        name: hash
        description: Find all media items which match the provided hash, case insensitive
      - in: query
        name: hashContains
        description: Find all media items which match the provided partial hash, case
          insensitive
      - in: query
        name: languageId
        description: Find all media items written in the language specified by Id
      - in: query
        name: languageIsoCode
        description: Find all media items written in the language specified by 639-2
          isoCode , case insensitive
      - in: query
        name: languageName
        description: Find all media items written in the language specified by name,
          case insensitive
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: mediaTypes
        description: Find all media items belonging to the specified media type[s]
      - in: query
        name: name
        description: Find all media items containing the provided name, case insensitive
      - in: query
        name: nameContains
        description: Find all media items containing the partial name, case insensitive
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: order
        description: '* The ascending or descending order'
      - in: query
        name: restrictToSet
        description: Find only media from within the supplied list of Ids
      - in: query
        name: sort
        description: '* Set of fields to sort the records by'
      - in: query
        name: sourceAcronym
        description: Find all media items that belong to the source specified by acronym,
          case insensitive
      - in: query
        name: sourceAcronymContains
        description: Find all media items that belong to the source specified by partial
          acronym, case insensitive
      - in: query
        name: sourceId
        description: Find all media items that belong to the source specified by Id
      - in: query
        name: sourceName
        description: Find all media items that belong to the source specified by name,
          case insensitive
      - in: query
        name: sourceNameContains
        description: Find all media items that belong to the source specified by partial
          name, case insensitive
      - in: query
        name: sourceUrl
        description: Find all media items which have the provided sourceUrl, case
          insensitive
      - in: query
        name: sourceUrlContains
        description: Find all media items which contain the provided partial sourceUrl,
          case insensitive
      - in: query
        name: syndicationCapturedBeforeDate
        description: Find all media items authored before the provided day (RFC 3339,
          time ignored)
      - in: query
        name: syndicationCapturedInRange
        description: Find all media items authored between the provided start and
          end days (RFC 3339, comma separated, time ignored)
      - in: query
        name: syndicationCapturedSinceDate
        description: Find all media items authored since the provided day (RFC 3339,
          time ignored)
      - in: query
        name: syndicationUpdatedBeforeDate
        description: Find all media items updated before the provided day, (RFC 3339,
          time ignored)
      - in: query
        name: syndicationUpdatedInRange
        description: Find all media items updated between the provided start and end
          days, (RFC 3339, comma separated, time ignored)
      - in: query
        name: syndicationUpdatedSinceDate
        description: Find all media items updated since the provided day, (RFC 3339,
          time ignored)
      - in: query
        name: syndicationVisibleBeforeDate
        description: Find all media items visible before the provided day, (RFC 3339,
          time ignored)
      - in: query
        name: syndicationVisibleInRange
        description: Find all media items visible between the provided start and end
          days, (RFC 3339, comma separated, time ignored)
      - in: query
        name: syndicationVisibleSinceDate
        description: Find all media items visible since the provided day, (RFC 3339,
          time ignored)
      - in: query
        name: tagIds
        description: Find only media items tagged with the specified tag Ids
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
  /resources/media/featured.json:
    get:
      summary: Get the list of featured content in the syndication system
      description: Get the list of featured content in the syndication system
      operationId: getFeaturedMedia
      x-api-path-slug: resourcesmediafeatured-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: How many records to offset the query by
      - in: query
        name: sort
        description: '* Set of fields to sort the records by'
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Featured
  /resources/media/mostPopularMedia.json:
    get:
      summary: Get MediaItems by popularity
      description: Returns the list of MediaItems with the highest ratings.
      operationId: getMostPopularMedia
      x-api-path-slug: resourcesmediamostpopularmedia-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - MostPopularMedia
  /resources/media/searchResults.json:
    get:
      summary: Get MediaItems by search query
      description: Returns the list of MediaItems matching the search query 'q'.The
        search query 'q' is a Lucene query.The syntax for a Lucene query can be found
        here
      operationId: searchMedia
      x-api-path-slug: resourcesmediasearchresults-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: q
        description: The search query supplied by the user
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - SearchResults
  /resources/media/{id}.json:
    get:
      summary: Get MediaItem by ID
      description: Returns the MediaItem identified by the 'id'.
      operationId: getMediaById
      x-api-path-slug: resourcesmediaid-json-get
      parameters:
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
  /resources/media/{id}/content:
    get:
      summary: Get content for MediaItem
      description: Returns the raw content (html, image, etc...) for the MediaItem
        identified by the 'id'.
      operationId: getMediaContentById
      x-api-path-slug: resourcesmediaidcontent-get
      parameters:
      - in: query
        name: calledByBuild
        description: The method that called this method
      - in: path
        name: id
        description: The id of the media to show content for
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - Content
  /resources/media/{id}/embed.json:
    get:
      summary: Get embed code for MediaItem
      description: Returns the javascript or iframe embed code for the MediaItem identified
        by 'id'.
      operationId: getMediaEmbedById
      x-api-path-slug: resourcesmediaidembed-json-get
      parameters:
      - in: query
        name: displayMethod
        description: Method used to render an html request
      - in: query
        name: divId
        description: Should the div to insert content into have a specific name?
      - in: query
        name: excludeDiv
        description: Should the div to insert content into be omitted?
      - in: query
        name: excludeJquery
        description: Should a reference to the JQuery Library be omitted?
      - in: query
        name: flavor
        description: Currently supports iframe, defaults to javascript
      - in: query
        name: height
        description: The height of the generated iframe
      - in: path
        name: id
        description: The id of the media to get embed code for
      - in: query
        name: iframeName
        description: The name of the iframe element
      - in: query
        name: width
        description: The width of the generated iframe
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - Embed
  /resources/media/{id}/preview.jpg:
    get:
      summary: Get JPG preview for MediaItem
      description: Returns the JPG preview, where applicable, for the MediaItem identified
        by the 'id'.
      operationId: getMediaPreviewById
      x-api-path-slug: resourcesmediaidpreview-jpg-get
      parameters:
      - in: path
        name: id
        description: The id of the media to get a preview for
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - Preview
      - Jpg
  /resources/media/{id}/ratings.json:
    get:
      summary: Get Ratings for MediaItem
      description: Get the Ratings (number of 'likes') for the MediaItem identified
        by the 'id'.
      operationId: getMediaRatingsById
      x-api-path-slug: resourcesmediaidratings-json-get
      parameters:
      - in: path
        name: id
        description: The ID of the media item to like
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - Ratings
  /resources/media/{id}/relatedMedia.json:
    get:
      summary: Get related MediaItems by ID
      description: Returns the list of MediaItems related to the MediaItem identified
        by the 'id'.
      operationId: getRelatedMediaById
      x-api-path-slug: resourcesmediaidrelatedmedia-json-get
      parameters:
      - in: path
        name: id
        description: The id of the media item to get related media for
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: Which field to sort the records by
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - RelatedMedia
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---