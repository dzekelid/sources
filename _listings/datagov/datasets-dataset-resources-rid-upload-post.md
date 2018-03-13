---
swagger: "2.0"
info:
  title: Data.gov API
  description: The data.gov catalog is powered by CKAN, a powerful open source data
    platform that includes a robust API. Please be aware that data.gov and the data.gov
    CKAN API only contain metadata about datasets. This metadata includes URLs and
    descriptions of datasets, but it does not include the actual data within each
    dataset.
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /datasets/{dataset}/resources/{rid}/upload/:
    post:
      summary: Add Datasets Dataset Resources R Upload
      description: Upload a file related to a given resource on a given dataset
      operationId: postDatasetsDatasetResourcesRUpload
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: path
        name: rid
        description: The resource unique identifier
      responses:
        200:
          description: OK
      tags:
      - datasets
      - dataset
      - resources
      - r
      - upload
definitions:
  Activity:
    properties:
      created_at:
        description: This is a default description.
        type: string
      icon:
        description: This is a default description.
        type: string
      key:
        description: This is a default description.
        type: string
      kwargs:
        description: This is a default description.
        type: string
      label:
        description: This is a default description.
        type: string
      related_to:
        description: This is a default description.
        type: string
      related_to_id:
        description: This is a default description.
        type: string
      related_to_kind:
        description: This is a default description.
        type: string
      related_to_url:
        description: This is a default description.
        type: string
  ActivityPage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  ApiKey:
    properties:
      apikey:
        description: This is a default description.
        type: string
  Badge:
    properties:
      kind:
        description: This is a default description.
        type: string
  BaseReference:
    properties:
      class:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
  Checksum:
    properties:
      type:
        description: This is a default description.
        type: string
      value:
        description: This is a default description.
        type: string
  CommunityResourcePage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  Crontab:
    properties:
      day_of_month:
        description: This is a default description.
        type: string
      day_of_week:
        description: This is a default description.
        type: string
      hour:
        description: This is a default description.
        type: string
      minute:
        description: This is a default description.
        type: string
      month_of_year:
        description: This is a default description.
        type: string
  Dataset:
    properties:
      badges:
        description: This is a default description.
        type: string
      community_resources:
        description: This is a default description.
        type: string
      created_at:
        description: This is a default description.
        type: string
      deleted:
        description: This is a default description.
        type: string
      description:
        description: This is a default description.
        type: string
      extras:
        description: This is a default description.
        type: string
      featured:
        description: This is a default description.
        type: string
      frequency:
        description: This is a default description.
        type: string
      frequency_date:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
  DatasetFullPage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  DatasetPage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  DatasetPreview:
    properties:
      badges:
        description: This is a default description.
        type: string
      community_resources:
        description: This is a default description.
        type: string
      created_at:
        description: This is a default description.
        type: string
      deleted:
        description: This is a default description.
        type: string
      description:
        description: This is a default description.
        type: string
      extras:
        description: This is a default description.
        type: string
      featured:
        description: This is a default description.
        type: string
      frequency:
        description: This is a default description.
        type: string
      frequency_date:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
  DatasetSuggestion:
    properties:
      id:
        description: This is a default description.
        type: string
      image_url:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      score:
        description: This is a default description.
        type: string
      slug:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
  Discussion:
    properties:
      class:
        description: This is a default description.
        type: string
      closed:
        description: This is a default description.
        type: string
      closed_by:
        description: This is a default description.
        type: string
      created:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      subject:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
      url:
        description: This is a default description.
        type: string
  DiscussionMessage:
    properties:
      content:
        description: This is a default description.
        type: string
      posted_on:
        description: This is a default description.
        type: string
  DiscussionPage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  DiscussionResponse:
    properties:
      close:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  Follow:
    properties:
      id:
        description: This is a default description.
        type: string
      since:
        description: This is a default description.
        type: string
  FollowPage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  Frequency:
    properties:
      id:
        description: This is a default description.
        type: string
      label:
        description: This is a default description.
        type: string
  GeoGranularity:
    properties:
      id:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
  GeoJSON:
    properties:
      coordinates:
        description: This is a default description.
        type: string
      type:
        description: This is a default description.
        type: string
  GeoJSONFeature:
    properties:
      id:
        description: This is a default description.
        type: string
      properties:
        description: This is a default description.
        type: string
      type:
        description: This is a default description.
        type: string
  GeoJSONFeatureCollection:
    properties:
      features:
        description: This is a default description.
        type: string
      type:
        description: This is a default description.
        type: string
  GeoLevel:
    properties:
      id:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
      parents:
        description: This is a default description.
        type: string
  HarvestBackend:
    properties:
      id:
        description: This is a default description.
        type: string
      label:
        description: This is a default description.
        type: string
  HarvestError:
    properties:
      created_at:
        description: This is a default description.
        type: string
      details:
        description: This is a default description.
        type: string
      message:
        description: This is a default description.
        type: string
  HarvestItem:
    properties:
      args:
        description: This is a default description.
        type: string
      created:
        description: This is a default description.
        type: string
      ended:
        description: This is a default description.
        type: string
      errors:
        description: This is a default description.
        type: string
      kwargs:
        description: This is a default description.
        type: string
      remote_id:
        description: This is a default description.
        type: string
      started:
        description: This is a default description.
        type: string
      status:
        description: This is a default description.
        type: string
  HarvestItemPreview:
    properties:
      args:
        description: This is a default description.
        type: string
      created:
        description: This is a default description.
        type: string
      ended:
        description: This is a default description.
        type: string
      errors:
        description: This is a default description.
        type: string
      kwargs:
        description: This is a default description.
        type: string
      remote_id:
        description: This is a default description.
        type: string
      started:
        description: This is a default description.
        type: string
      status:
        description: This is a default description.
        type: string
  HarvestJob:
    properties:
      created:
        description: This is a default description.
        type: string
      ended:
        description: This is a default description.
        type: string
      errors:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      items:
        description: This is a default description.
        type: string
      source:
        description: This is a default description.
        type: string
      started:
        description: This is a default description.
        type: string
      status:
        description: This is a default description.
        type: string
  HarvestJobPage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  HarvestJobPreview:
    properties:
      created:
        description: This is a default description.
        type: string
      ended:
        description: This is a default description.
        type: string
      errors:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      items:
        description: This is a default description.
        type: string
      source:
        description: This is a default description.
        type: string
      started:
        description: This is a default description.
        type: string
      status:
        description: This is a default description.
        type: string
  HarvestSource:
    properties:
      active:
        description: This is a default description.
        type: string
      backend:
        description: This is a default description.
        type: string
      config:
        description: This is a default description.
        type: string
      created_at:
        description: This is a default description.
        type: string
      deleted:
        description: This is a default description.
        type: string
      description:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
      url:
        description: This is a default description.
        type: string
  HarvestSourceValidation:
    properties:
      comment:
        description: This is a default description.
        type: string
      "on":
        description: This is a default description.
        type: string
      state:
        description: This is a default description.
        type: string
  Interval:
    properties:
      every:
        description: This is a default description.
        type: string
      period:
        description: This is a default description.
        type: string
  Issue:
    properties:
      class:
        description: This is a default description.
        type: string
      closed:
        description: This is a default description.
        type: string
      closed_by:
        description: This is a default description.
        type: string
      created:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      subject:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
      url:
        description: This is a default description.
        type: string
  IssueMessage:
    properties:
      content:
        description: This is a default description.
        type: string
      posted_on:
        description: This is a default description.
        type: string
  IssuePage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  IssueResponse:
    properties:
      close:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  Job:
    properties:
      args:
        description: This is a default description.
        type: string
      description:
        description: This is a default description.
        type: string
      enabled:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      kwargs:
        description: This is a default description.
        type: string
      last_run_at:
        description: This is a default description.
        type: string
      last_run_id:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
      schedule:
        description: This is a default description.
        type: string
      task:
        description: This is a default description.
        type: string
  License:
    properties:
      flags:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      maintainer:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
      url:
        description: This is a default description.
        type: string
  Member:
    properties:
      role:
        description: This is a default description.
        type: string
  MembershipRequest:
    properties:
      comment:
        description: This is a default description.
        type: string
      created:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      status:
        description: This is a default description.
        type: string
  Metric:
    properties:
      date:
        description: This is a default description.
        type: string
      level:
        description: This is a default description.
        type: string
      object_id:
        description: This is a default description.
        type: string
      values:
        description: This is a default description.
        type: string
  MyMetrics:
    properties:
      datasets_count:
        description: This is a default description.
        type: string
      datasets_org_count:
        description: This is a default description.
        type: string
      followers_count:
        description: This is a default description.
        type: string
      followers_org_count:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      resources_availability:
        description: This is a default description.
        type: string
  Notification:
    properties:
      created_on:
        description: This is a default description.
        type: string
      details:
        description: This is a default description.
        type: string
      type:
        description: This is a default description.
        type: string
  Organization:
    properties:
      acronym:
        description: This is a default description.
        type: string
      badges:
        description: This is a default description.
        type: string
      created_at:
        description: This is a default description.
        type: string
      deleted:
        description: This is a default description.
        type: string
      description:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      last_modified:
        description: This is a default description.
        type: string
      logo:
        description: This is a default description.
        type: string
      members:
        description: This is a default description.
        type: string
      metrics:
        description: This is a default description.
        type: string
  OrganizationPage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  OrganizationSuggestion:
    properties:
      acronym:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      image_url:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      score:
        description: This is a default description.
        type: string
      slug:
        description: This is a default description.
        type: string
  Post:
    properties:
      content:
        description: This is a default description.
        type: string
      created_at:
        description: This is a default description.
        type: string
      credit_to:
        description: This is a default description.
        type: string
      credit_url:
        description: This is a default description.
        type: string
      datasets:
        description: This is a default description.
        type: string
      headline:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      image:
        description: This is a default description.
        type: string
      last_modified:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
  PostPage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  RefuseMembership:
    properties:
      comment:
        description: This is a default description.
        type: string
  Resource:
    properties:
      created_at:
        description: This is a default description.
        type: string
      description:
        description: This is a default description.
        type: string
      filesize:
        description: This is a default description.
        type: string
      filetype:
        description: This is a default description.
        type: string
      format:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      is_available:
        description: This is a default description.
        type: string
      last_modified:
        description: This is a default description.
        type: string
      metrics:
        description: This is a default description.
        type: string
      mime:
        description: This is a default description.
        type: string
  Reuse:
    properties:
      badges:
        description: This is a default description.
        type: string
      created_at:
        description: This is a default description.
        type: string
      datasets:
        description: This is a default description.
        type: string
      deleted:
        description: This is a default description.
        type: string
      description:
        description: This is a default description.
        type: string
      featured:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      image:
        description: This is a default description.
        type: string
      last_modified:
        description: This is a default description.
        type: string
      metrics:
        description: This is a default description.
        type: string
  ReusePage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  ReuseSuggestion:
    properties:
      id:
        description: This is a default description.
        type: string
      image_url:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      score:
        description: This is a default description.
        type: string
      slug:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
  ReuseType:
    properties:
      id:
        description: This is a default description.
        type: string
      label:
        description: This is a default description.
        type: string
  Site:
    properties:
      id:
        description: This is a default description.
        type: string
      metrics:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
  SpatialCoverage:
    properties:
      granularity:
        description: This is a default description.
        type: string
      zones:
        description: This is a default description.
        type: string
  Task:
    properties:
      exc:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      result:
        description: This is a default description.
        type: string
      status:
        description: This is a default description.
        type: string
      traceback:
        description: This is a default description.
        type: string
  TemporalCoverage:
    properties:
      end:
        description: This is a default description.
        type: string
      start:
        description: This is a default description.
        type: string
  TerritorySuggestion:
    properties:
      code:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      keys:
        description: This is a default description.
        type: string
      level:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
      score:
        description: This is a default description.
        type: string
  Topic:
    properties:
      created_at:
        description: This is a default description.
        type: string
      datasets:
        description: This is a default description.
        type: string
      deleted:
        description: This is a default description.
        type: string
      description:
        description: This is a default description.
        type: string
      featured:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      last_modified:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      private:
        description: This is a default description.
        type: string
  TopicPage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  Transfer:
    properties:
      comment:
        description: This is a default description.
        type: string
      created:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      reponse_comment:
        description: This is a default description.
        type: string
      responded:
        description: This is a default description.
        type: string
      status:
        description: This is a default description.
        type: string
  TransferRequest:
    properties:
      comment:
        description: This is a default description.
        type: string
  TransferResponse:
    properties:
      comment:
        description: This is a default description.
        type: string
      response:
        description: This is a default description.
        type: string
  UploadedImage:
    properties:
      image:
        description: This is a default description.
        type: string
      success:
        description: This is a default description.
        type: string
  UploadedResource:
    properties:
      created_at:
        description: This is a default description.
        type: string
      description:
        description: This is a default description.
        type: string
      filesize:
        description: This is a default description.
        type: string
      filetype:
        description: This is a default description.
        type: string
      format:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      is_available:
        description: This is a default description.
        type: string
      last_modified:
        description: This is a default description.
        type: string
      metrics:
        description: This is a default description.
        type: string
      mime:
        description: This is a default description.
        type: string
  User:
    properties:
      about:
        description: This is a default description.
        type: string
      avatar:
        description: This is a default description.
        type: string
      first_name:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      last_name:
        description: This is a default description.
        type: string
      organizations:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      roles:
        description: This is a default description.
        type: string
      since:
        description: This is a default description.
        type: string
      slug:
        description: This is a default description.
        type: string
  UserPage:
    properties:
      data:
        description: This is a default description.
        type: string
      facets:
        description: This is a default description.
        type: string
      next_page:
        description: This is a default description.
        type: string
      page:
        description: This is a default description.
        type: string
      page_size:
        description: This is a default description.
        type: string
      previous_page:
        description: This is a default description.
        type: string
      total:
        description: This is a default description.
        type: string
  UserSuggestion:
    properties:
      avatar_url:
        description: This is a default description.
        type: string
      first_name:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      last_name:
        description: This is a default description.
        type: string
      score:
        description: This is a default description.
        type: string
      slug:
        description: This is a default description.
        type: string
x-collection-name: Data.Gov
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