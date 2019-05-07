# ![LOGO](logo.png) Peel Tune-in API **flow**ground Connector

## Description

A generated **flow**ground connector for the Peel Tune-in API API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/peel-ci.com/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:41+03:00

## API Description

The machine learning service APIs utilize hashtags from Twitter to find related, trending shows, related Twitter hashtags in real time and to generate direct tune-in URLs.

## Authorization

This API does not require authorization.

## Actions

### Gets related hashtags for a show.

> Returns any official hashtag and any hashtags which were learned within the most recent time window for the show.

*Tags:* `hashtag`

#### Input Parameters
* `showID` - _required_ - Unique ID for a show
* `timeWindow` - _optional_ - Time window in seconds (default is 2 hours)

### Gets trending shows.

*Tags:* `hashtag`

#### Input Parameters
* `limit` - _optional_ - Number of trending shows (default is 20)
* `timeWindow` - _optional_ - Time window in seconds (default is 2 hours)

### Gets tunein URLs (links) from either a tweet, hashtags, @mentions, or show ID.

> Either use <b>tweet</b>, <b>hashtags</b>, or <b>showID</b> as the parameter. The tunein URLs that match best are returned in order of best match.<br/><br/>A <b>tweet</b> in this context is shorthand for text from a social networking conversation, e.g., it could be from Facebook, Twitter, LinkedIn, etc., and be greater than 140 characters.

*Tags:* `hashtag`

#### Input Parameters
* `tweet` - _optional_ - Text from a social networking conversation
* `hashtags` - _optional_ - Comma separated list of hashtags and @mentions
* `showID` - _optional_ - Unique ID for a show

### Get health of Tune-in service (which includes its uptime).

*Tags:* `health`

### Gets the last 100 statuses for this show.

> For Twitter, statuses are synonymous with tweets.

*Tags:* `status`

#### Input Parameters
* `showID` - _required_ - Unique ID for a show

## License

**flow**ground :- Telekom iPaaS / peel-ci-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
