# nginxctl

`apachectl`, but for nginx.

Original from https://github.com/rackerlabs/nginxctl - sadly that repo is rather dead.

- patched to work with python3
- FWIW python2 should still work
- will use `/usr/bin/env python`
- omits colored output when used in shell pipes. ( https://github.com/rackerlabs/nginxctl/pull/9/commits/dda07fae58c8cc0ebb8602299b37af8895ffd981 )
- patched to work properly with ipv6 addresses (**[A-F]** vs. **[a-f]** if need be, existence of double colons)

Known Bugs:
- seems to not handle *server* statements missing a **listen** directive
