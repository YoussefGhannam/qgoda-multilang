---
virtual: 1
---
<!--QGODA-NO-XGETTEXT-->
[% USE q = Qgoda %]

[% IF !asset.parent %]
  [% FOREACH year IN q.llistPosts().vmap('date.year').unique() %]
    [% FOREACH imonth IN q.llistPosts('date.year' = year).vmap('date.imonth').unique() %]
      [% location = q.sprintf("/%s/archive/%04u/%02u/index.html", 
                              asset.lingua, year, imonth) %]
      [% q.clone(location => location
                 plocation => location
                 title => q.sprintf(gtx.xgettext("Posts from {date}",
                                                 gtx.gettext("%04u/%02u"),
                                                 year, imonth)), 
                 year => year imonth => imonth
                 start => 0) %]
    [% END %]
  [% END %]
[% ELSE %]
  [% filters = { 'date.year' = year 'date.imonth' = imonth } %]
  [% INCLUDE components/listing.html filters = filters %]
[% END %]
<!--/QGODA-NO-XGETTEXT-->
