About the module
================

The OData Support module for Drupal allows Drupal 7 site builders to add data
from one or more Open Data Protocol (OData) feeds to articles and other content
types.

What is OData?
==============

The Open Data Protocol (OData) is a Web protocol for querying and updating data
that provides a way to unlock your data and free it from silos that exist in
applications today. OData does this by applying and building upon Web
technologies such as HTTP, Atom Publishing Protocol and JSON to provide access
to information from a variety of applications, services, and stores.

Installation
============

1.  Upload the odata_support folder to your Drupal site.
2.  Open the module configuration page (admin/modules) and enable the module,
    click Save.
3.  Click the module’s Configure link, and add an endpoint:
    a.  Enter (for example) http://odata.netflix.com/v1/Catalog in Add an
        Endpoint.
    b.  Click Save and verify that NetflixCatalog now appears in the list of
        endpoints.
    c.  Optionally, change the default paging limit or set up a proxy to use
        when fetching results.

Usage
=====

Add a new article (or other content type) by clicking the Add Content link, and
add a title and some body text.  Scroll down to the OData section and use the
query builder to customize the OData query.
    *   Click values in the table to filter by that value, or click (expand)
        links to drill down into queries.
    *   Click undo to back up a step, or Reset to start over.
    *   Click Advanced to edit the query manually and $select certain columns or
        limit to so many $top results, etc. – see odata.org for syntax rules and
        available options.
    *   URLs and images in the query results are automatically linked.
    *   To add more than one data table to an article, click Add another item.

Once you’re satisfied with the query, scroll to the bottom of the form and click
Save.  You should see the data table below your post’s body. Each time the page
is displayed, live results are fetched from the OData endpoint.

