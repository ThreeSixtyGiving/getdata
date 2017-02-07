---
layout: page
title: Home
permalink: /
---

A list of all known data in the 360Giving format can be found on the website at: [http://www.threesixtygiving.org/data/find-data/](http://www.threesixtygiving.org/data/data-registry/)

A JSON feed of this data can be found at the following endpoint: 
[http://data.threesixtygiving.org/data.json](http://data.threesixtygiving.org/data.json)

Requests to the endpoint will return a JSON file that contains a number of records about data sets.

The JSON is an array of objects in the following format:

~~~json

[
  {
     "title":"Title of the dataset",
     "description":"Description about the dataset",
     "identifier":"An internal identifier for this dataset from our 
                  storage system",
     "license":"A link to the license information for this dataset. 
                  Should be a valid URL",
     "license_name":"A human readable title of the license given in 
                      the license field",
     "publisher": {
        "name":"Name of the organisation publishing this dataset",
        "website":"Should be a valid URL to a website of that publisher",
        "logo":"Should be a valid URL to a logo for that publisher. 
                You may not necessarily have permission to use this 
                logo for your own purposes.",
        "prefix":"The unique 360Giving prefix used by this publisher
                  to identify the grants they publish."
     },
     "distribution":[ {
        "downloadURL":"A valid URL to directly access the data",
        "accessURL": "A valid URL, usually to a web page, where access 
                      to the downloadURL can be found. The web page 
                      usually has other useful information about the data",
        "title":"Title of the dataset"}
     ]
  },
]

~~~

## Changelog

**2016-06-28** - Adds the `prefix` field to the publisher list

**2016-06-07** - Changes links to list of all known data and to the JSON feed.

**2016-05-24** - Added the `license_name` field

**2016-05-22** - Documentation first created

## Credits
This site uses Jekyll and the base Jekyll theme.  
You can find the source code for the Jekyll new theme at:
{% include icon-github.html username="jglovier" %} /
[jekyll-new](https://github.com/jglovier/jekyll-new)  
You can find the source code for Jekyll at
{% include icon-github.html username="jekyll" %} /
[jekyll](https://github.com/jekyll/jekyll)
