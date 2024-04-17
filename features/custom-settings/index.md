---
title: Custom settings
---

Glitch-soc provides various ways to customize Mastodon's behavior

In Glitch-soc you can set various enviroment variables to change Mastodon's behavior. These variables must be set on your system or on the `.env` file

### Supported variables

#### Maximum allowed character count
`MAX_TOOT_CHARS` changes the maximum allowed characters that the user can use.

Example:

`MAX_TOOT_CHARS=500`

#### Maximum allowed hashtags to follow in a feed column
`MAX_FEED_HASHTAGS`changes the maximum number of hashtags that a user can use in a post.

Note: that setting this value higher may cause a significant database load

Example:

`MAX_FEED_HASHTAGS=4`

#### Maximum hashtags to display
`MAX_TRENDING_TAGS` changes the number of hashtags shown on the 'Explore' page.

Example:

`MAX_TRENDING_TAGS=10`

#### Maximum number of pinned posts
`MAX_PINNED_TOOTS` changes the maximum number of pinned posts that a user can set on their profile.

Example:

`MAX_PINNED_TOOTS=5`

#### Maximum allowed bio characters
`MAX_BIO_CHARS` changes the maximum number of characters allowed on the user bio.

Example:

`MAX_BIO_CHARS=500`

#### Maximum number of profile fields allowed
`MAX_PROFILE_FIELDS` changes the maximum number of profile fields that a user can have on their profile.

Example:

`MAX_PROFILE_FIELDS=4`

#### Maximum allowed display name characters
`MAX_DISPLAY_NAME_CHARS` changes the maximum allowed display name characters for a user account. This is not related to the user handle (@username).

Example:

`MAX_DISPLAY_NAME_CHARS=30`

#### Maximum allowed poll options
`MAX_POLL_OPTIONS` changes the maximum allowed poll options that the user could add to their post.

Example:

`MAX_POLL_OPTIONS=5`

#### Maximum allowed poll option characters
`MAX_POLL_OPTION_CHARS` changes the maximum allowed characters in a poll option that the user could use.

Example:

`MAX_POLL_OPTION_CHARS=100`

#### Maximum image and video/audio upload sizes
`MAX_IMAGE_SIZE` the maximum image upload size.

(Units are in bytes. 1048576 bytes equals 1 megabyte.)

Example:

`MAX_IMAGE_SIZE=8388608`

#### Maximum image and video/audio upload sizes
`MAX_VIDEO_SIZE` changes the maximum image upload size.

(Units are in bytes. 1048576 bytes equals 1 megabyte.)

Example:

`MAX_VIDEO_SIZE=41943040`

### Maximum custom emoji file sizes
`MAX_EMOJI_SIZE` and `MAX_REMOTE_EMOJI_SIZE`

Note: If undefined or smaller than `MAX_EMOJI_SIZE`, the value of `MAX_EMOJI_SIZE` will be used for `MAX_REMOTE_EMOJI_SIZE`

(Units are in bytes. 1048576 bytes equals 1 megabyte.)

Example:

`MAX_EMOJI_SIZE=262144`

`MAX_REMOTE_EMOJI_SIZE=262144`

#### Maximum search results to display
`MAX_SEARCH_RESULTS` changes the maximum number of search results displayed to the user.

(Only relevant when ElasticSearch is installed)

Example:

`MAX_SEARCH_RESULTS=20`
