Jenkins Status Board
====================

An external status board for Jenkins Build statuses that can be used on dashboard apps that don't allow you to sign into Jenkins.

Useful for development shop TVs that display status widgets. index.php auto refreshes an iframe to avoid full widget refreshing.

Successful builds are green, cancelled builds are gray, failed builds are red. If there is a failure in any of your builds, the screen will pulse red to get your attention.

See example.html for an example that includes a failure.

Job Names
=========

This assumes you have multiple environments per job/project, and set up the Jenkins Job names like "$project-$environment". You can modify this to your liking.

Usage
=====

Set your user and url values at the top of status.php

Put index.php and status.php into a /status folder on your server, and point your widget to http://yourhost.com/path/to/status. It will auto-refresh inside an iframe every 5 minutes by default.
