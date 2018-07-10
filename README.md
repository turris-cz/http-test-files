This repository contains files that are deployed as a static content on http/https
server. They are used for download tests in updater (as part of the unit tests)
and can be used potentially for same purpose in other projects.

These files should be deployed on server that has HTTPS and is signed with let's
encrypt certificate. That is because we are testing certificate pinning and we are
expecting let's encrypt. Another requirement is that HTTP requests should return
HTTP 3xx message with redirect to HTTPS. The reason is that we have to have way to
test redirect.

This repository contains simple index file with explanation of server purpose.
Then one short and one long text file for download testing.
