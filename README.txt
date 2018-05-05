
Copyright 2017 Hussein El-hussein


Description
-----------
This module allows mapping to Paragraphs fields.

Features:
---------
* Mapping to "Text" & "Long Text"
* Mapping to "Interval" field (Interval Module)
* Mapping to "Text List" & "Integer List"
* Mapping to all numeric fields
* Mapping to boolean field
* Mapping to image field
* Mapping to file field
* Mapping to list of type taxonomy terms
* Note: currently it only maps a single value to a field, except for taxonomy terms.

Dependencies
-------------
This module requires the following modules:

* Feeds (https://drupal.org/project/feeds)
* Paragraphs (https://drupal.org/project/paragraphs)

Installation
------------
To install, copy the feeds_para_mapper directory and all its contents to your modules
directory.

Configuration
-------------
It has no configuration page.
To enable this module, visit administer -> modules, and enable Paragraphs Mapper.

Usage
-------------
* For mapping multiple taxonomy terms, the terms must be separated by comma.
* For mapping to a boolean field, the value must be numeric (0 or 1), or string (true,false).
* For mapping to a file field, the value must be link to a local file (public://file.pdf), or remote file (http://example.com/file.pdf).
* Same goes for image field.
Note: in case you had issue grabbing remote files, search for this line in php.ini:
allow_url_fopen = Off
then edit it so it becomes like this:
allow_url_fopen = On
restart apache afterwards

Author
------
Hussein El-hussein (function.op@gmail.com)
