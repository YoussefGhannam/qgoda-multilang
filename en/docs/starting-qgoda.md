---
title: Starting Qgoda
name: starting-qgoda
date: 2018-03-31
tags: [ General, Installation ]
---
[% USE q = Qgoda %]

Starting Qgoda is as easy as typing `qgoda watch` in the [installed]([% q.llink(name = 'installation') %]) theme directory.  You can stop Qgoda by pressing `CTRL-C` or by closing the terminal window that it is running in.

The command `qgoda watch` will start Qgoda in *watch mode*.  Qgoda will then build the entire site, and then wait for changes that will trigger a rebuild.  The only reason to restart Qgoda is a change to the [configuration]([% q.llink(name = 'configuration') %]) file `_config.yaml`.  

You can also just build the site once with `qgoda build`.

Continue with [% q.lanchor(name = 'configuration') %].
