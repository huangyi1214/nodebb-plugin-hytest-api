# `api/v1` Endpoints

**Note**: When requested with a master token, an additional parameter (`_uid`) is required in the data payload so the Write API can execute the requested action under the correct user context.
This limitation means that certain actions only work with a specific uid. For example, `PUT /:uid` updates a user's profile information, but is only accessible by the uid of the user itself, or
an administrative uid. All other uids passed in will result in an error.
