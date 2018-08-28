---
name: AWS Simple Queue Service
x-slug: aws-simple-queue-service
description: Amazon Simple Queue Service (SQS) is a fast, reliable, scalable, fully
  managed message queuing service. Amazon SQS makes it simple and cost-effective to
  decouple the components of a cloud application. You can use Amazon SQS to transmit
  any volume of data, without losing messages or requiring other services to be always
  available. Amazon SQS includesstandard queueswith high throughput and at-least-once
  processing, andFIFO queuesthat provide FIFO (first-in, first-out) delivery and exactly-once
  processing. With Amazon SQS, you can offload the administrative burden of operating
  and scaling a highly available messaging cluster, while paying a low price for only
  what you use.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Sources
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/aws-simple-queue-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Simple Queue Service API - List Dead Letter Source Queues
  x-api-slug: actionlistdeadlettersourcequeues-get
  description: Returns a list of your queues that have the RedrivePolicy queue attribute
    configured with a dead letter queue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
  humanURL: https://aws.amazon.com/sqs/
  baseURL: :///
  tags: Amazon Web Services, Jobs, Orchestration, Stack Network, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sources/master/_listings/aws-simple-queue-service/actionlistdeadlettersourcequeues-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.simple.notification.service.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.simple.queue.service.stack.network
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/Amazon-SQ
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/sqs/index.html
- type: x-console
  url: https://console.aws.amazon.com/sqs/
- type: x-documentation
  url: http://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/sqs/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=12
- type: x-getting-started
  url: https://aws.amazon.com/sqs/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/sqs/pricing/
- type: x-website
  url: https://aws.amazon.com/sqs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---