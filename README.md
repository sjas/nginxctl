# nginxctl
apachectl, but for nginx

Original from https://github.com/rackerlabs/nginxctl but that repo is rather dead.

Patched to work with python3 and to omit color output when used in shell pipes. ( https://github.com/rackerlabs/nginxctl/pull/9/commits/dda07fae58c8cc0ebb8602299b37af8895ffd981 )

Patched to work properly with ipv6 addresses, so these cases work, too:
- lowercase [a-f] / uppercase [A-F] lettering
- standard / compressed notation (the latter containing '::')

Known Bugs:
- seems to not handle *server* statements missing a **listen** directive
