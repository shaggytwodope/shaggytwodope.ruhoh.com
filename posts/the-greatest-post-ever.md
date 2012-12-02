---
title:
date: '2012-12-01'
description: This is a test run of the post stuff
categories: News Testing
---

Just a funky test of features and learning

Trying to learn how the formatting works, So using back ticks is totaly cool, gotta love markdown lol.

````
    #!/bin/bash
    gmail_login="login"
    gmail_password="password"

    nbmail="$(wget --secure-protocol=TLSv1 --timeout=3 -t 1 -q -O - \
    https://${gmail_login}:${gmail_password}@mail.google.com/mail/feed/atom \
    --no-check-certificate | grep 'fullcount' \
    | sed -e 's/.*<fullcount>//;s/<\/fullcount>.*//' 2>/dev/null)"

    if [ -z "$nbmail" ]; then
    echo "Error"
    else
      if [ $nbmail != 0 ]; then
        echo ""
        `mplayer2 ~/sounds/mailmf.wav`
      else
      echo ""
      fi
    fi
````

#The section#

The Section with actualy can output text for new mail or none, overever it's been edited out for use in conky.
Merely to give an audio sound.

````
      if [ $nbmail != 0 ]; then
        echo ""
        `mplayer2 ~/sounds/mailmf.wav`
      else
      echo ""
