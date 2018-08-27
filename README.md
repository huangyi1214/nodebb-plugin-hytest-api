# Write API

This plugin exposes a *write enabled API interface* for NodeBB. It is useful if you would like to supplment the built-in *read-only* API, in order to push items/actions/events to NodeBB.

For example, without this plugin, one can easily retrieve the contents of a post by prefixing `api/` to the corresponding route. (e.g. https://community.nodebb.org/api/topic/687/help-translate-nodebb/2).

With this plugin, however, you can create content on NodeBB externally (new topics, new posts, etc), which comes in handy when third-party applications want deeper integration with NodeBB.

# Installation

**Install this plugin via the plugins page in the ACP.**

Alternatively:

```
$ cd /path/to/nodebb/node_modules
$ git clone git@github.com:julianlam/nodebb-plugin-write-api.git
$ cd nodebb-plugin-write-api
$ npm i

# Then start NodeBB and activate the plugin