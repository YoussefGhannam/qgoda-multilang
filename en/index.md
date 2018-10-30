---
title: Qgoda Multi-Language Seed Project
name: home
location: /en/index.html
permalink: /en/
---
<!--QGODA-NO-XGETTEXT-->[% USE q = Qgoda %]<!--/QGODA-NO-XGETTEXXT-->

This is a project seed for [Qgoda](http://www.qgoda.net/).  The theme is
[multi-lingual]([% q.llink(name = 'multi-language') %]), comes with
module bundling via [webpack](https://webpack.js.org/) and advanced web
development features, a development web server, and it shows Qgoda best practices
and example code for almost all functionality available in Qgoda.

It is the last one in a series of Qgoda example themes:

* [Qgoda Minimal](https://github.com/gflohr/qgoda-minimal):
   The bare minimum for a Qgoda site.</dd>
* [Qgoda Essential](https://github.com/gflohr/qgoda-essential):
   A theme that shows the usage of all Qgoda features but no
   web development environment other than a development web server.
* [Qgoda Default](https://github.com/gflohr/qgoda-default):
  Like Qgoda Essential but with a minimal [Bootstrap](???) theme,
      module bundling via
      [webpack](https://webpack.js.org/).  It uses [Sass](???) for CSS
      pre-processing, [PostCSS](???) with
      [cssnext](???) for prefix-less CSS, [cssnano](???) for CSS minification,
      [font-magician](????), syntax-highlighting of code snippets with
      [PrismJS](???) and more.  Additionally, it shows how to integrate
      [CSS Modules](???) (modular, conflict-free CSS) with Qgoda.
* [Qgoda Multilang](https://github.com/gflohr/qgoda-essential):
  Like Qgoda Default but completely multi-langual.

See [https://github.com/[% config.theme_repo %]](https://github.com/[% config.theme_repo %])
for instructions on how to use this theme. The pages below give you a detailed
insight into the internals of the theme.  The default site serves its own documentation.

[% INCLUDE components/listing.html -%]
