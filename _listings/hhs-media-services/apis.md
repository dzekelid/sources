---
name: HHS Media Services
x-slug: hhs-media-services
description: Use this API platform to create sites with text and multimedia content
  for syndication. CDC, FDA, HHS, and NIH have built syndication sites using this
  platform, which is available in Java and .NET.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Sources
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/apis.md
specificationVersion: "0.14"
apis:
- name: HHS Media Services Get Resources by search query
  x-api-slug: hhs-media-services
  description: Returns the list of Resources matching the search query 'q'.The search
    query 'q' is a Lucene query.The syntax for a Lucene query can be found here.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources.json
  tags: Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resources-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resources-json-get-openapi.md
- name: HHS Media Services Get Campaigns
  x-api-slug: hhs-media-services
  description: Returns the list of Campaigns.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/campaigns.json
  tags: Resources,Campaigns
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcescampaigns-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcescampaigns-json-get-openapi.md
- name: HHS Media Services Get Campaign by ID
  x-api-slug: hhs-media-services
  description: Returns the Campaign identified by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/campaigns/{id}.json
  tags: Resources,Campaigns,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcescampaignsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcescampaignsid-json-get-openapi.md
- name: HHS Media Services Get MediaItems by Campaign ID
  x-api-slug: hhs-media-services
  description: Returns the list of MediaItems for the Campaign identified by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/campaigns/{id}/media.json
  tags: Resources,Campaigns,Id,Media
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcescampaignsidmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcescampaignsidmedia-json-get-openapi.md
- name: HHS Media Services Get MediaItems for Campaign
  x-api-slug: hhs-media-services
  description: Renders the list of MediaItems associated with the Campaign identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/campaigns/{id}/syndicate.json
  tags: Resources,Campaigns,Id,Syndicate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcescampaignsidsyndicate-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcescampaignsidsyndicate-json-get-openapi.md
- name: HHS Media Services Get Languages
  x-api-slug: hhs-media-services
  description: Returns the list Languages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/languages.json
  tags: Resources,Languages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourceslanguages-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourceslanguages-json-get-openapi.md
- name: HHS Media Services Get Language by ID
  x-api-slug: hhs-media-services
  description: Returns the Language identified by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/languages/{id}.json
  tags: Resources,Languages,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourceslanguagesid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourceslanguagesid-json-get-openapi.md
- name: HHS Media Services Get MediaItems
  x-api-slug: hhs-media-services
  description: Returns the list of MediaItems matching the specified query parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media.json
  tags: Resources,Media
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmedia-json-get-openapi.md
- name: HHS Media Services Get the list of featured content in the syndication system
  x-api-slug: hhs-media-services
  description: Get the list of featured content in the syndication system
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/featured.json
  tags: Resources,Media,Featured
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediafeatured-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediafeatured-json-get-openapi.md
- name: HHS Media Services Get MediaItems by popularity
  x-api-slug: hhs-media-services
  description: Returns the list of MediaItems with the highest ratings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/mostPopularMedia.json
  tags: Resources,Media,MostPopularMedia
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediamostpopularmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediamostpopularmedia-json-get-openapi.md
- name: HHS Media Services Get MediaItems by search query
  x-api-slug: hhs-media-services
  description: Returns the list of MediaItems matching the search query 'q'.The search
    query 'q' is a Lucene query.The syntax for a Lucene query can be found here
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/searchResults.json
  tags: Resources,Media,SearchResults
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediasearchresults-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediasearchresults-json-get-openapi.md
- name: HHS Media Services Get MediaItem by ID
  x-api-slug: hhs-media-services
  description: Returns the MediaItem identified by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/{id}.json
  tags: Resources,Media,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaid-json-get-openapi.md
- name: HHS Media Services Get content for MediaItem
  x-api-slug: hhs-media-services
  description: Returns the raw content (html, image, etc...) for the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/{id}/content
  tags: Resources,Media,Id,Content
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidcontent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidcontent-get-openapi.md
- name: HHS Media Services Get embed code for MediaItem
  x-api-slug: hhs-media-services
  description: Returns the javascript or iframe embed code for the MediaItem identified
    by 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/{id}/embed.json
  tags: Resources,Media,Id,Embed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidembed-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidembed-json-get-openapi.md
- name: HHS Media Services Get JPG preview for MediaItem
  x-api-slug: hhs-media-services
  description: Returns the JPG preview, where applicable, for the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/{id}/preview.jpg
  tags: Resources,Media,Id,Preview,Jpg
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidpreview-jpg-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidpreview-jpg-get-openapi.md
- name: HHS Media Services Get Ratings for MediaItem
  x-api-slug: hhs-media-services
  description: Get the Ratings (number of 'likes') for the MediaItem identified by
    the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/{id}/ratings.json
  tags: Resources,Media,Id,Ratings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidratings-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidratings-json-get-openapi.md
- name: HHS Media Services Get related MediaItems by ID
  x-api-slug: hhs-media-services
  description: Returns the list of MediaItems related to the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/{id}/relatedMedia.json
  tags: Resources,Media,Id,RelatedMedia
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidrelatedmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidrelatedmedia-json-get-openapi.md
- name: HHS Media Services Get syndicated content for MediaItem
  x-api-slug: hhs-media-services
  description: Returns the syndicated content for a given MediaItem in the specified
    'format' (HTML or JSON).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/{id}/syndicate.json
  tags: Resources,Media,Id,Syndicate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidsyndicate-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidsyndicate-json-get-openapi.md
- name: HHS Media Services Get JPG thumbnail for MediaItem
  x-api-slug: hhs-media-services
  description: Returns the JPG thumbnail, where applicable, for the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/{id}/thumbnail.jpg
  tags: Resources,Media,Id,Thumbnail,Jpg
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidthumbnail-jpg-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidthumbnail-jpg-get-openapi.md
- name: HHS Media Services Get Youtube metadata for MediaItem
  x-api-slug: hhs-media-services
  description: Returns the Youtube metadata, where applicable, for the MediaItem identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/media/{id}/youtubeMetaData.json
  tags: Resources,Media,Id,YoutubeMetaData
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidyoutubemetadata-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediaidyoutubemetadata-json-get-openapi.md
- name: HHS Media Services Get MediaTypes
  x-api-slug: hhs-media-services
  description: Returns the list of available MediaTypes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/mediaTypes.json
  tags: Resources,MediaTypes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediatypes-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesmediatypes-json-get-openapi.md
- name: HHS Media Services Get Sources
  x-api-slug: hhs-media-services
  description: Returns the list of Sources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/sources.json
  tags: Resources,Sources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcessources-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcessources-json-get-openapi.md
- name: HHS Media Services Get Source by ID
  x-api-slug: hhs-media-services
  description: Returns the Source identified by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/sources/{id}.json
  tags: Resources,Sources,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcessourcesid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcessourcesid-json-get-openapi.md
- name: HHS Media Services Get MediaItems for Source
  x-api-slug: hhs-media-services
  description: Renders the list of MediaItems associated with the Source identified
    by the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/sources/{id}/syndicate.json
  tags: Resources,Sources,Id,Syndicate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcessourcesidsyndicate-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcessourcesidsyndicate-json-get-openapi.md
- name: HHS Media Services Get Tags
  x-api-slug: hhs-media-services
  description: Returns the list of Tags matching the specified query parameters in
    the specified 'format'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags.json
  tags: Resources,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestags-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestags-json-get-openapi.md
- name: HHS Media Services Get TagLanguages
  x-api-slug: hhs-media-services
  description: Returns the list of TagLanguages
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/tagLanguages.json
  tags: Resources,Tags,TagLanguages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagstaglanguages-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagstaglanguages-json-get-openapi.md
- name: HHS Media Services Get TagTypes
  x-api-slug: hhs-media-services
  description: Returns the list of TagTypes
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/tagTypes.json
  tags: Resources,Tags,TagTypes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagstagtypes-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagstagtypes-json-get-openapi.md
- name: HHS Media Services Get Tag by ID
  x-api-slug: hhs-media-services
  description: Returns the Tag identified by the 'id' in the specified 'format'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/{id}.json
  tags: Resources,Tags,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagsid-json-get-openapi.md
- name: HHS Media Services Get MediaItems for Tag
  x-api-slug: hhs-media-services
  description: Returns the list of MediaItems associated with the Tag identified by
    the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/{id}/media.json
  tags: Resources,Tags,Id,Media
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagsidmedia-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagsidmedia-json-get-openapi.md
- name: HHS Media Services Get related Tags by ID
  x-api-slug: hhs-media-services
  description: Returns the list of Tags related to the Tag identified by the 'id'
    in the specified format.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/{id}/related.json
  tags: Resources,Tags,Id,Related
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagsidrelated-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagsidrelated-json-get-openapi.md
- name: HHS Media Services Get MediaItems for Tag
  x-api-slug: hhs-media-services
  description: Renders the list of MediaItems associated with the Tag identified by
    the 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/tags/{id}/syndicate.json
  tags: Resources,Tags,Id,Syndicate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagsidsyndicate-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcestagsidsyndicate-json-get-openapi.md
- name: HHS Media Services Get UserMediaList by ID
  x-api-slug: hhs-media-services
  description: Get a specific user media list by 'id'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2//resources/userMediaLists/{id}.json
  tags: Resources,UserMediaLists,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesusermedialistsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/resourcesusermedialistsid-json-get-openapi.md
- name: HHS Media Services
  x-api-slug: hhs-media-services
  description: Use this API platform to create sites with text and multimedia content
    for syndication. CDC, FDA, HHS, and NIH have built syndication sites using this
    platform, which is available in Java and .NET.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/hhs-media-services.png
  humanURL: https://api.digitalmedia.hhs.gov/
  baseURL: https://api.digitalmedia.hhs.gov//api/v2
  tags: Sources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/hhs-media-services/openapi.md
x-common:
- type: x-website
  url: https://api.digitalmedia.hhs.gov/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---