---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Describe Event Categories
  version: 1.0.0
  description: Displays a list of categories for all event source types, or, if specified,
    for a specified source type.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeEvents:
    get:
      summary: Describe Events
      description: Returns events related to DB instances, DB security groups, DB
        snapshots, and DB parameter groups for the past 14 days.
      operationId: describeevents
      x-api-path-slug: actiondescribeevents-get
      parameters:
      - in: query
        name: Duration
        description: The number of minutes to retrieve events for
        type: string
      - in: query
        name: EndTime
        description: The end of the time interval for which to retrieve events,        specified
          in ISO 8601 format
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: A list of event categories that trigger notifications for a event
          notification subscription
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeEvents
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: SourceIdentifier
        description: The identifier of the event source for which events will be returned
        type: string
      - in: query
        name: SourceType
        description: The event source to retrieve events for
        type: string
      - in: query
        name: StartTime
        description: The beginning of the time interval to retrieve events for,        specified
          in ISO 8601 format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
  /?Action=CreateEventSubscription:
    get:
      summary: Create Event Subscription
      description: Creates an RDS event notification subscription.
      operationId: createeventsubscription
      x-api-path-slug: actioncreateeventsubscription-get
      parameters:
      - in: query
        name: Enabled
        description: A Boolean value; set to true to activate the subscription, set
          to false to create the subscription but not active it
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: A list of event categories for a SourceType that you want to
          subscribe to
        type: string
      - in: query
        name: SnsTopicArn
        description: The Amazon Resource Name (ARN) of the SNS topic created for event
          notification
        type: string
      - in: query
        name: SourceIds.SourceId.N
        description: The list of identifiers of the event sources for which events
          will be returned
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the subscription
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=DeleteEventSubscription:
    get:
      summary: Delete Event Subscription
      description: Deletes an RDS event notification subscription.
      operationId: deleteeventsubscription
      x-api-path-slug: actiondeleteeventsubscription-get
      parameters:
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription you want
          to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=DescribeEventCategories:
    get:
      summary: Describe Event Categories
      description: Displays a list of categories for all event source types, or, if
        specified, for a specified source type.
      operationId: describeeventcategories
      x-api-path-slug: actiondescribeeventcategories-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Categories
  /?Action=DescribeEventSubscriptions:
    get:
      summary: Describe Event Subscriptions
      description: Lists all the subscription descriptions for a customer account.
      operationId: describeeventsubscriptions
      x-api-path-slug: actiondescribeeventsubscriptions-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeOrderableDBInstanceOptions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription you want
          to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=ModifyEventSubscription:
    get:
      summary: Modify Event Subscription
      description: Modifies an existing RDS event notification subscription.
      operationId: modifyeventsubscription
      x-api-path-slug: actionmodifyeventsubscription-get
      parameters:
      - in: query
        name: Enabled
        description: A Boolean value; set to true to activate the subscription
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: A list of event categories for a SourceType that you want to
          subscribe to
        type: string
      - in: query
        name: SnsTopicArn
        description: The Amazon Resource Name (ARN) of the SNS topic created for event
          notification
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
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