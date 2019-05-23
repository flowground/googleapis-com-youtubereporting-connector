# ![LOGO](logo.png) YouTube Reporting **flow**ground Connector

## Description

A generated **flow**ground connector for the YouTube Reporting API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/youtubereporting/v1/swagger.json<br/>
Generated at: 2019-05-23T12:13:51+03:00

## API Description

Schedules reporting jobs containing your YouTube Analytics data and downloads the resulting bulk data reports in the form of CSV files.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists jobs.

*Tags:* `jobs`

#### Input Parameters
* `includeSystemManaged` - _optional_ - If set to true, also system-managed jobs will be returned; otherwise only
user-created jobs will be returned. System-managed jobs can neither be
modified nor deleted.
* `onBehalfOfContentOwner` - _optional_ - The content owner's external ID on which behalf the user is acting on. If
not set, the user is acting for himself (his own channel).
* `pageSize` - _optional_ - Requested page size. Server may return fewer jobs than requested.
If unspecified, server will pick an appropriate default.
* `pageToken` - _optional_ - A token identifying a page of results the server should return. Typically,
this is the value of
ListReportTypesResponse.next_page_token
returned in response to the previous call to the `ListJobs` method.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates a job and returns it.

*Tags:* `jobs`

#### Input Parameters
* `onBehalfOfContentOwner` - _optional_ - The content owner's external ID on which behalf the user is acting on. If
not set, the user is acting for himself (his own channel).
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Deletes a job.

*Tags:* `jobs`

#### Input Parameters
* `jobId` - _required_ - The ID of the job to delete.
* `onBehalfOfContentOwner` - _optional_ - The content owner's external ID on which behalf the user is acting on. If
not set, the user is acting for himself (his own channel).
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Gets a job.

*Tags:* `jobs`

#### Input Parameters
* `jobId` - _required_ - The ID of the job to retrieve.
* `onBehalfOfContentOwner` - _optional_ - The content owner's external ID on which behalf the user is acting on. If
not set, the user is acting for himself (his own channel).
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists reports created by a specific job.<br/>
> Returns NOT_FOUND if the job does not exist.

*Tags:* `jobs`

#### Input Parameters
* `createdAfter` - _optional_ - If set, only reports created after the specified date/time are returned.
* `jobId` - _required_ - The ID of the job.
* `onBehalfOfContentOwner` - _optional_ - The content owner's external ID on which behalf the user is acting on. If
not set, the user is acting for himself (his own channel).
* `pageSize` - _optional_ - Requested page size. Server may return fewer report types than requested.
If unspecified, server will pick an appropriate default.
* `pageToken` - _optional_ - A token identifying a page of results the server should return. Typically,
this is the value of
ListReportsResponse.next_page_token
returned in response to the previous call to the `ListReports` method.
* `startTimeAtOrAfter` - _optional_ - If set, only reports whose start time is greater than or equal the
specified date/time are returned.
* `startTimeBefore` - _optional_ - If set, only reports whose start time is smaller than the specified
date/time are returned.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Gets the metadata of a specific report.

*Tags:* `jobs`

#### Input Parameters
* `jobId` - _required_ - The ID of the job.
* `onBehalfOfContentOwner` - _optional_ - The content owner's external ID on which behalf the user is acting on. If
not set, the user is acting for himself (his own channel).
* `reportId` - _required_ - The ID of the report to retrieve.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Method for media download. Download is supported<br/>
> on the URI `/v1/media/{+name}?alt=media`.

*Tags:* `media`

#### Input Parameters
* `resourceName` - _required_ - Name of the media that is being downloaded.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists report types.

*Tags:* `reportTypes`

#### Input Parameters
* `includeSystemManaged` - _optional_ - If set to true, also system-managed report types will be returned;
otherwise only the report types that can be used to create new reporting
jobs will be returned.
* `onBehalfOfContentOwner` - _optional_ - The content owner's external ID on which behalf the user is acting on. If
not set, the user is acting for himself (his own channel).
* `pageSize` - _optional_ - Requested page size. Server may return fewer report types than requested.
If unspecified, server will pick an appropriate default.
* `pageToken` - _optional_ - A token identifying a page of results the server should return. Typically,
this is the value of
ListReportTypesResponse.next_page_token
returned in response to the previous call to the `ListReportTypes` method.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-youtubereporting-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
