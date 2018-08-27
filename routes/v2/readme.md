# `api/v2` Endpoints

**Note**: When requested with a master token, an additional parameter (`_uid`) is required in the data payload so the hytest API can execute the requested action under the correct user context.
This limitation means that certain actions only work with a specific uid. For example, `PUT /:uid` updates a user's profile information, but is only accessible by the uid of the user itself, or
an administrative uid. All other uids passed in will result in an error.

**Migrating from v1?** Take a look at the migration info at the bottom of this page.