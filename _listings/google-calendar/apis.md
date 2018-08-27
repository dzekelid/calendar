---
name: Google Calendar
x-slug: google-calendar
description: The Calendar API lets you display, create and modify calendar events
  as well as work with many other calendar-related objects, such as calendars or access
  controls. This document describes how to use RESTful calls and client libraries
  for various programming languages (Java, PHP, .NET, JavaScript, NodeJs, Ruby, Python,
  Go, Android, iOS).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-calendar-icon-66527.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Calendar
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/calendar/master/_listings/google-calendar/apis.md
specificationVersion: "0.14"
apis:
- name: Google Calendar - Create Calendar
  x-api-slug: calendars-post
  description: Creates a secondary calendar.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-calendar-icon-66527.png
  humanURL: https://developers.google.com/google-apps/calendar/
  baseURL: https://www.googleapis.com//calendar/v3
  tags: Calendar, Google APIs, Stack Network, Stack, Productivity, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/calendar/master/_listings/google-calendar/calendars-post-openapi.md
- name: Google Calendar - CreaDeletete Calendar
  x-api-slug: calendarscalendarid-delete
  description: Deletes a secondary calendar. Use calendars.clear for clearing all
    events on primary calendars.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-calendar-icon-66527.png
  humanURL: https://developers.google.com/google-apps/calendar/
  baseURL: https://www.googleapis.com//calendar/v3
  tags: Calendar, Google APIs, Stack Network, Stack, Productivity, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/calendar/master/_listings/google-calendar/calendarscalendarid-delete-openapi.md
- name: Google Calendar - Get Calendar
  x-api-slug: calendarscalendarid-get
  description: Returns metadata for a calendar.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-calendar-icon-66527.png
  humanURL: https://developers.google.com/google-apps/calendar/
  baseURL: https://www.googleapis.com//calendar/v3
  tags: Calendar, Google APIs, Stack Network, Stack, Productivity, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/calendar/master/_listings/google-calendar/calendarscalendarid-get-openapi.md
- name: Google Calendar - Update Calendar
  x-api-slug: calendarscalendarid-patch
  description: Updates metadata for a calendar. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-calendar-icon-66527.png
  humanURL: https://developers.google.com/google-apps/calendar/
  baseURL: https://www.googleapis.com//calendar/v3
  tags: Calendar, Google APIs, Stack Network, Stack, Productivity, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/calendar/master/_listings/google-calendar/calendarscalendarid-patch-openapi.md
- name: Google Calendar - Update Calendar
  x-api-slug: calendarscalendarid-put
  description: Updates metadata for a calendar.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-calendar-icon-66527.png
  humanURL: https://developers.google.com/google-apps/calendar/
  baseURL: https://www.googleapis.com//calendar/v3
  tags: Calendar, Google APIs, Stack Network, Stack, Productivity, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/calendar/master/_listings/google-calendar/calendarscalendarid-put-openapi.md
- name: Google Calendar - Clear Primary Calendar
  x-api-slug: calendarscalendaridclear-post
  description: Clears a primary calendar. This operation deletes all events associated
    with the primary calendar of an account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-calendar-icon-66527.png
  humanURL: https://developers.google.com/google-apps/calendar/
  baseURL: https://www.googleapis.com//calendar/v3
  tags: Calendar, Google APIs, Stack Network, Stack, Productivity, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/calendar/master/_listings/google-calendar/calendarscalendaridclear-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.books.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.calendar.stack.network
- type: x-code
  url: https://developers.google.com/google-apps/calendar/downloads
- type: x-documentation
  url: https://developers.google.com/google-apps/calendar/v3/reference/
- type: x-website
  url: https://developers.google.com/google-apps/calendar/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---