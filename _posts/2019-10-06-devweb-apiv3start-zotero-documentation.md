---
ID: 584
post_title: 'dev:web api:v3:start [Zotero Documentation]'
author: gicomadmin
post_excerpt: ""
layout: post
permalink: >
  http://guillaumeisabelle.com/blogging/2019/10/06/devweb-apiv3start-zotero-documentation/
published: true
post_date: 2019-10-06 13:13:09
---
<!-- wp:heading -->

## API Implementations {#api_implementations}

<!-- /wp:heading -->

<!-- wp:paragraph -->

Known client libraries for the Zotero API (all versions) include:

<!-- /wp:paragraph -->

<!-- wp:list -->

*   <https://github.com/fcheslack/libZotero> (PHP and Python)
*   <https://github.com/shazino/SZNZotero> (Objective-C)
*   <https://github.com/urschrei/pyzotero> (Python)
*   <https://github.com/clioweb/phpZotero> (PHP, no longer maintained)
*   <https://github.com/scholarpress/scholarpress-workshop>

<!-- /wp:list -->

<!-- wp:paragraph -->

The API‌ forms a fundamental part of several projects, including:

<!-- /wp:paragraph -->

<!-- wp:list -->

*   The online library view at zotero.org, which is built using the same API‌
*   [Zotpress][1], a WordPress plugin for including citations to items in your Zotero library in blog posts. The plugin makes extensive use of the read API and implements both key-based and OAuth for access control.
*   [Biblio Bouts][2], an game where participants compete to collect high quality sources online. The game uses the API‌ to see what items participants have saved.
*   [phpZoteroWebDAV][3], a WebDAV implementation in PHP which allows users to sync their attachments to their own webservers, including an online library and attachment view building off the read API. (AGPL)
*   [Scanner for Zotero][4], Android app which saves items to Zotero libraries using the write API (Java, GPL-licensed)
*   [Zandy][5] Android app using the read and write APIs to provide full access to Zotero libraries (Java, AGPL-licensed)
*   [ZotPad][6] iPad/iPhone app using the read and file upload APIs to provide read access to Zotero libraries and read/write access to attachment files. Write access is planned. (Objective C, GPL-licensed)
*   [Zotero Reader][7] Browser app that provides read access to Zotero library and read/write access to PDF attachments. (Javascript/PHP)
*   [ZotSpip][8], a SPIP plugin to synchronise a Zotero library with SPIP (a content management system). References can be presented in web pages and searched through a dedicated webpage. A complementary plugin (BiblioCheck) allows a research unit to manage corrections to apply to the unit bibliography. (PHP)
*   [BibBase][9] A web service that makes it possible to embed a list of Zotero publications in a web page (e.g., for personal publications pages).
*   [Kerko][10] A web application component for the Flask framework that synchronizes with a Zotero library to provide a user-friendly yet powerful search and browsing interface for an online bibliography. (Python, GPL-licensed)

<!-- /wp:list -->

> API Implementations Known client libraries for the Zotero API (all versions) include: https://github.com/fcheslack/libZotero (PHP and Python) https://github.com/shazino/SZNZotero (Objective-C) https://github.com/urschrei/pyzotero (Python) https://github.com/clioweb/phpZotero (PHP, no longer maintained) https://github.com/scholarpress/scholarpress-workshop The API‌ forms a fundamental part of several projects, including: The online library view at zotero.org, which is built using the same API‌ Zotpress, a

Source: *[dev:web api:v3:start [Zotero Documentation]][11]*

 [1]: http://wordpress.org/extend/plugins/zotpress/
 [2]: http://www.bibliobouts.org/
 [3]: https://github.com/krueschan/phpZoteroWebDAV
 [4]: https://github.com/jmschanck/Scanner-For-Zotero
 [5]: https://github.com/ajlyon/zandy
 [6]: http://www.zotpad.com/
 [7]: http://www.zoteroreader.com/
 [8]: http://plugins.spip.net/zotspip.html
 [9]: http://bibbase.org/
 [10]: https://github.com/whiskyechobravo/kerko
 [11]: https://www.zotero.org/support/dev/web_api/v3/start#api_implementations