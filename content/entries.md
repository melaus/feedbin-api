Entries
=======

Get Entries
-----------

Entries belong to feeds. To get all the entries for a feed use the `feed_id`. The entry attributes vary from the original feed in several ways. Links and image sources are rewritten to always point to the source. The created_at date is converted to UTC.

- `GET /v1/feeds/203/entries.json` will return all entries for feed `203`

```json
[
  {
    "id": 3648,
    "title": "Cleveland Drinkup February 6",
    "url": "https:\/\/github.com\/blog\/1398-cleveland-drinkup-february-6",
    "author": "juliamae",
    "content": "<p>Cleveland <img class=\"emoji\" title=\":metal:\" alt=\":metal:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/metal.png\" height=\"20\" width=\"20\" align=\"absmiddle\">! Let's <img class=\"emoji\" title=\":beers:\" alt=\":beers:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/beers.png\" height=\"20\" width=\"20\" align=\"absmiddle\"><img class=\"emoji\" title=\":cocktail:\" alt=\":cocktail:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/cocktail.png\" height=\"20\" width=\"20\" align=\"absmiddle\"><img class=\"emoji\" title=\":neckbeard:\" alt=\":neckbeard:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/neckbeard.png\" height=\"20\" width=\"20\" align=\"absmiddle\"><img class=\"emoji\" title=\":guitar:\" alt=\":guitar:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/guitar.png\" height=\"20\" width=\"20\" align=\"absmiddle\"><img class=\"emoji\" title=\":octocat:\" alt=\":octocat:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/octocat.png\" height=\"20\" width=\"20\" align=\"absmiddle\"> in one of Ohio's greatest cities, Cleveland!<\/p>\n\n<p>Join <a href=\"https:\/\/github.com\/asenchi\" class=\"user-mention\">@asenchi<\/a> and me Wednesday at the <a href=\"http:\/\/www.yelp.com\/biz\/great-lakes-brewing-company-cleveland-4\">Great Lakes Brewing Company Taproom<\/a>, drinks on GitHub.<\/p>\n\n<p><img src=\"https:\/\/f.cloud.github.com\/assets\/849\/119266\/79ef6bbe-6c9e-11e2-9150-47d7da0b85c9.jpg\" alt=\"Great Lakes Taproom\"><\/p>\n\n<p><strong>The Facts:<\/strong><\/p>\n\n<ul>\n<li>\n<a href=\"http:\/\/www.greatlakesbrewing.com\/brewpub\/around-the-brewpub\">Great Lakes Brewing Company<\/a> - <a href=\"https:\/\/maps.google.com\/?q=2516+Market+Ave,+Cleveland,+OH,+USA\">2516 Market Ave<\/a>\n<\/li>\n<li>Wednesday, February 6 at 8:00pm<\/li>\n<\/ul><p><a href=\"https:\/\/maps.google.com\/?q=2516+Market+Ave,+Cleveland,+OH,+USA\"><img src=\"https:\/\/f.cloud.github.com\/assets\/849\/119328\/c8cbb682-6ca0-11e2-81c8-246e4027f892.png\" alt=\"Screen Shot 2013-02-01 at 1 53 02 PM\"><\/a>          <\/p>",
    "summary": null,
    "created_at": "2013-02-01T19:02:43Z"
  },
  {
    "id": 3649,
    "title": "GitHub Enterprise 11.10.300 Release",
    "url": "https:\/\/github.com\/blog\/1392-github-enterprise-11-10-300-release",
    "author": "watsonian",
    "content": "<p>We're excited to announce the latest release of <a href=\"https:\/\/enterprise.github.com\">GitHub Enterprise<\/a>. We're shipping this version with <a href=\"https:\/\/github.com\/blog\/1347-issue-attachments\"><strong>Issue Attachments<\/strong><\/a>, <a href=\"https:\/\/github.com\/blog\/1360-introducing-contributions\"><strong>Contributions<\/strong><\/a>, and much more. Along with a variety of general improvements and adjustments, this new release brings the following features from GitHub.com:<\/p>\n\n<ul>\n<li><a href=\"https:\/\/github.com\/blog\/1375-task-lists-in-gfm-issues-pulls-comments\"><strong>Task Lists<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1379-zen-writing-mode\"><strong>Zen Writing Mode<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1327-creating-files-on-github\"><strong>Create files on GitHub<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1377-create-and-delete-branches\"><strong>Create and delete branches<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1335-tidying-up-after-pull-requests\"><strong>Delete merged branches from Pull Requests<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1369-restore-tidied-pull-requests\"><strong>Restore deleted branches from Pull Requests<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1387-viewing-past-contributions\"><strong>Viewing Past Contributions<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1378-view-long-running-pull-requests\"><strong>View Long-running Pull Requests<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1357-issue-autocompletion\"><strong>Issue Autocompletion<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1365-a-more-transparent-clipboard-button\"><strong>More Transparent Clipboard Buttons<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1386-closing-issues-via-commit-messages\"><strong>Closing Issues via Commit Comments<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1381-a-whole-new-code-search\"><strong>Improvements to Code Search<\/strong><\/a><\/li>\n<li><a href=\"https:\/\/github.com\/blog\/1320-command-bar-autocompletes-stars\"><strong>Command bar autocompletes stars<\/strong><\/a><\/li>\n<\/ul><p>In addition, we're also including several new Enterprise specific features:<\/p>\n\n<h2>Repository Archives<\/h2>\n\n<p>This has been a frequently requested feature since we launched GitHub\nEnterprise, and we're happy to announce that it's now available! Each\nrepository will have a link to download a zip archive of the master\nbranch, along with the ability to download tarball or zip archives of\nthe repository for any tags that have been set. This functionality is\nbacked by the same Nodeload service that serves these files for GitHub.com.\nYou can get more background information about Nodeload\n<a href=\"https:\/\/github.com\/blog\/678-meet-nodeload-the-new-download-server\">here<\/a>\nand <a href=\"https:\/\/github.com\/blog\/900-nodeload2-downloads-reloaded\">here<\/a>.<\/p>\n\n<p><img src=\"https:\/\/f.cloud.github.com\/assets\/244\/109621\/bbfcb172-6a89-11e2-99e8-6590def655f0.png\" alt=\"Screen 20Shot 202013-01-29 20at 202 40 01 20PM\"><\/p>\n\n<h2>Support for Multiple Admin SSH Keys<\/h2>\n\n<p>You can now add more than one SSH authorized key for the admin user on the\ninstallation. It will automatically detect any existing keys that are installed\nas well.<\/p>\n\n<p><img src=\"https:\/\/f.cloud.github.com\/assets\/244\/109622\/c741acfe-6a89-11e2-94f7-73a7a67b0c84.png\" alt=\"Screen 20Shot 202013-01-29 20at 202 21 57 20PM\"><\/p>\n\n<h2>Management Console API<\/h2>\n\n<p>A new API for managing GitHub Enterprise settings and maintenances has been\nadded. This new API allows you to update configuration settings, add admin\nSSH authorized keys, upgrade, and enable or disable maintenance mode. You\ncan find full documentation for the API\n<a href=\"https:\/\/support.enterprise.github.com\/entries\/23032152-management-console-api\">here<\/a>.\nThis API has actually existed since the 11.10.280 release, so anyone on 11.10.280\nor higher should be able to take advantage of the API. This will be especially\nuseful when you need to upgrade an Enterprise appliance on a remote network, so you\ndon't have to upload new GHPs over slow connections.<\/p>\n\n<h2>Updated Admin Tools Dashboard<\/h2>\n\n<p>The Admin Tools dashboard has had a major overhaul! It now has a look and feel\nthat better matches the rest of the site.<\/p>\n\n<p><img src=\"https:\/\/f.cloud.github.com\/assets\/244\/109623\/d6bd0480-6a89-11e2-8367-bc2417c21eba.png\" alt=\"Screen 20Shot 202013-01-29 20at 202 05 54 20PM\"><\/p>\n\n<h2>Faster Configuration Runs<\/h2>\n\n<p>Prior to 11.10.300, making any settings changes would cause a full\nconfiguration run. The config run would take around 10 minutes to complete, even for minor changes. Now only the initial configuration run and upgrades take the full amount of time. If\nyou're only making a settings change, runs can take 30 seconds or less now!<\/p>\n\n<h2>Deleted Repository Restoration<\/h2>\n\n<p>When a repository is deleted, it's now banished to purgatory. Repositories in purgatory wait in\nlimbo for a month before being fully deleted. While in purgatory, any admin can\nrestore the repository with the push of a single button -- including all issues,\npull requests, and any associated comments. Purgatory is accessible from the Admin\nTools view of any user on a GitHub Enterprise installation.<\/p>\n\n<p><img src=\"https:\/\/f.cloud.github.com\/assets\/244\/109626\/1c42edd0-6a8a-11e2-99de-b14fff805321.png\" alt=\"Screen 20Shot 202013-01-29 20at 202 16 23 20PM\"><\/p>\n\n<h2>Search Indexing API<\/h2>\n\n<p>With the addition of improvements to the search that shipped in this release, a\nnew API is now available to queue up repositories and users for indexing. You can\nuse this API to integrate into whatever other tools you use at your company.\nDocumentation for this API is available\n<a href=\"https:\/\/support.enterprise.github.com\/entries\/23050336-search-indexing-api\">here<\/a>.<\/p>\n\n<hr><p>We hope you enjoy these features as much as we do. Don't forget that there is more information available about GitHub Enterprise at <a href=\"https:\/\/enterprise.github.com\/\">https:\/\/enterprise.github.com\/<\/a>. You can also see the full release notes <a href=\"https:\/\/enterprise.github.com\/releases\/11.10.300\">here<\/a>.<\/p>",
    "summary": null,
    "created_at": "2013-01-31T17:29:32Z"
  }
]
```

**Parameters**

 - `page: optional` `GET /v1/feeds/203/entries.json?page=2` will get page two of the available entries
 - `since: optional` `GET /v1/feeds/203/entries.json?since=2013-02-02T14:07:33Z` will get all entries created after the iso 8601 timestamp.

**Status Codes**

- `200 OK` will be returned if found
- `404 Not Found` will be returned if no feed is found, or if the page number does not exist
- `403 Forbidden` will be returned if the user does not subscribe to this feed

Get Entry
---------

- `GET /v1/feeds/203/entries/3648.json` will return just entry `3648`

```json
{
  "id": 3648,
  "title": "Cleveland Drinkup February 6",
  "url": "https:\/\/github.com\/blog\/1398-cleveland-drinkup-february-6",
  "author": "juliamae",
  "content": "<p>Cleveland <img class=\"emoji\" title=\":metal:\" alt=\":metal:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/metal.png\" height=\"20\" width=\"20\" align=\"absmiddle\">! Let's <img class=\"emoji\" title=\":beers:\" alt=\":beers:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/beers.png\" height=\"20\" width=\"20\" align=\"absmiddle\"><img class=\"emoji\" title=\":cocktail:\" alt=\":cocktail:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/cocktail.png\" height=\"20\" width=\"20\" align=\"absmiddle\"><img class=\"emoji\" title=\":neckbeard:\" alt=\":neckbeard:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/neckbeard.png\" height=\"20\" width=\"20\" align=\"absmiddle\"><img class=\"emoji\" title=\":guitar:\" alt=\":guitar:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/guitar.png\" height=\"20\" width=\"20\" align=\"absmiddle\"><img class=\"emoji\" title=\":octocat:\" alt=\":octocat:\" src=\"https:\/\/a248.e.akamai.net\/assets.github.com\/images\/icons\/emoji\/octocat.png\" height=\"20\" width=\"20\" align=\"absmiddle\"> in one of Ohio's greatest cities, Cleveland!<\/p>\n\n<p>Join <a href=\"https:\/\/github.com\/asenchi\" class=\"user-mention\">@asenchi<\/a> and me Wednesday at the <a href=\"http:\/\/www.yelp.com\/biz\/great-lakes-brewing-company-cleveland-4\">Great Lakes Brewing Company Taproom<\/a>, drinks on GitHub.<\/p>\n\n<p><img src=\"https:\/\/f.cloud.github.com\/assets\/849\/119266\/79ef6bbe-6c9e-11e2-9150-47d7da0b85c9.jpg\" alt=\"Great Lakes Taproom\"><\/p>\n\n<p><strong>The Facts:<\/strong><\/p>\n\n<ul>\n<li>\n<a href=\"http:\/\/www.greatlakesbrewing.com\/brewpub\/around-the-brewpub\">Great Lakes Brewing Company<\/a> - <a href=\"https:\/\/maps.google.com\/?q=2516+Market+Ave,+Cleveland,+OH,+USA\">2516 Market Ave<\/a>\n<\/li>\n<li>Wednesday, February 6 at 8:00pm<\/li>\n<\/ul><p><a href=\"https:\/\/maps.google.com\/?q=2516+Market+Ave,+Cleveland,+OH,+USA\"><img src=\"https:\/\/f.cloud.github.com\/assets\/849\/119328\/c8cbb682-6ca0-11e2-81c8-246e4027f892.png\" alt=\"Screen Shot 2013-02-01 at 1 53 02 PM\"><\/a>          <\/p>",
  "summary": null,
  "created_at": "2013-02-01T19:02:43Z"
}
```

**Status Codes**

- `200 OK` will be returned if found
- `404 Not Found` will be returned if no entry is found
- `403 Forbidden` will be returned if the user does not subscribe to the feed this entry belongs to