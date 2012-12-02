---
title: Bash Scripts and Tricks
description: Some stuff for bash, parhaps some zsh stuff as well.
---

#Content Test#
Some Content


``

#!/bin/bash

echo `mplayer -fs -cookies -cookies-file /tmp/cookie.txt $(youtube-dl -g --cookies /tmp/cookie.txt "$@")`


``



`<code>` spans are delimited
by backticks.

You can include literal backticks
like `` `this` ``.