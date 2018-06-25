---
name: Stripe
x-slug: stripe
description: Online payment processing for internet businesses. Stripe is a suite
  of payment APIs that powers commerce for online businesses of all sizes, including
  fraud prevention, and subscription management. Use Stripes payment platform to accept
  and process p...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
x-kinRank: "10"
x-alexaRank: "1914"
tags: Sources
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/apis.md
specificationVersion: "0.14"
apis:
- name: Stripe Get Customers Customer Sources
  x-api-slug: stripe
  description: Get Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/sources
  tags: Customers, Customer, Sources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/customerscustomersources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/customerscustomersources-get-openapi.md
- name: Stripe Add Customers Customer Sources
  x-api-slug: stripe
  description: Post Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/sources
  tags: Customers, Customer, Sources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/customerscustomersources-post-openapi.md
- name: Stripe Delete Customers Customer Sources
  x-api-slug: stripe
  description: Delete Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/sources/{id}
  tags: Customers, Customer, Sources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/customerscustomersourcesid-delete-openapi.md
- name: Stripe Get Customers Customer Sources
  x-api-slug: stripe
  description: Get Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/sources/{id}
  tags: Customers, Customer, Sources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/customerscustomersourcesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/customerscustomersourcesid-get-openapi.md
- name: Stripe Add Customers Customer Sources
  x-api-slug: stripe
  description: Post Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/sources/{id}
  tags: Customers, Customer, Sources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/customerscustomersourcesid-post-openapi.md
- name: Stripe Add Customers Customer Sources  Verify
  x-api-slug: stripe
  description: Post Customers, Customer, Sources, , Verify
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/sources/{id}/verify
  tags: Customers, Customer, Sources, , Verify
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/customerscustomersourcesidverify-post-openapi.md
- name: Stripe Add Sources
  x-api-slug: stripe
  description: Creates a new source object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///sources
  tags: Sources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sources-post-openapi.md
- name: Stripe Get Sources Source
  x-api-slug: stripe
  description: Retrieves an existing source object. Supply the unique source ID from
    a source creation request and Stripe will return the corresponding up-to-date
    source object information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///sources/{source}
  tags: Sources, Source
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sourcessource-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sourcessource-get-openapi.md
- name: Stripe Add Sources Source
  x-api-slug: stripe
  description: Updates the specified source by setting the values of the parameters
    passed. Any parameters not provided will be left unchanged.This request accepts
    the metadata and owner as arguments. It is also possible to update type specific
    information for selected payment methods. Please refer to our payment method guides
    for more detail.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///sources/{source}
  tags: Sources, Source
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sourcessource-post-openapi.md
- name: Stripe Get Sources Source Mandate Notifications Mandate Notification
  x-api-slug: stripe
  description: Get Sources, Source, Mandate, Notifications, Mandate, Notification
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///sources/{source}/mandate_notifications/{mandate_notification}
  tags: Sources, Source, Mandate, Notifications, Mandate, Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sourcessourcemandate-notificationsmandate-notification-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sourcessourcemandate-notificationsmandate-notification-get-openapi.md
- name: Stripe Get Sources Source Source Transactions
  x-api-slug: stripe
  description: Get Sources, Source, Source, Transactions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///sources/{source}/source_transactions
  tags: Sources, Source, Source, Transactions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sourcessourcesource-transactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sourcessourcesource-transactions-get-openapi.md
- name: Stripe Get Sources Source Source Transactions Source Transaction
  x-api-slug: stripe
  description: Retrieve an existing source transaction object. Supply the unique source
    ID from a source creation request and the source transaction ID and Stripe will
    return the corresponding up-to-date source object information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///sources/{source}/source_transactions/{source_transaction}
  tags: Sources, Source, Source, Transactions, Source, Transaction
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sourcessourcesource-transactionssource-transaction-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sourcessourcesource-transactionssource-transaction-get-openapi.md
- name: Stripe Add Sources Source Verify
  x-api-slug: stripe
  description: Post Sources, Source, Verify
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///sources/{source}/verify
  tags: Sources, Source, Verify
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/sourcessourceverify-post-openapi.md
- name: Stripe
  x-api-slug: stripe
  description: Web and mobile payments, built for developers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Sources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/stripe/openapi.md
x-common:
- type: x-base
  url: https://api.stripe.com/
- type: x-blog
  url: https://stripe.com/blog
- type: x-blog-rss
  url: https://stripe.com/blog/feed.rss
- type: x-change-log
  url: https://stripe.com/docs/upgrades
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stripe
- type: x-crunchbase
  url: https://crunchbase.com/organization/stripe
- type: x-email
  url: info@stripe.com
- type: x-email
  url: privacy@stripe.com
- type: x-email
  url: atlas@stripe.com
- type: x-email
  url: notices@stripe.com
- type: x-email
  url: jane.diaz@stripe.com
- type: x-email
  url: nonprofit@stripe.com
- type: x-email
  url: support@stripe.com
- type: x-email
  url: dpo@stripe.com
- type: x-github
  url: https://github.com/stripe
- type: x-linkedin
  url: https://www.linkedin.com/company/stripe/
- type: x-pricing
  url: https://stripe.com/us/pricing
- type: x-twitter
  url: https://twitter.com/stripe
- type: x-website
  url: https://stripe.com/
- type: x-website
  url: http://stripe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---