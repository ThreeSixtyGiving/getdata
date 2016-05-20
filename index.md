---
layout: page
title: Home
permalink: /
---

A list of all known data in the 360Giving format can be found on the website at: [http://www.threesixtygiving.org/get-involved/data/](http://www.threesixtygiving.org/get-involved/data/)

A JSON feed of this data can be found at the following endpoint: 
[http://data.threesixtygiving.org/datastore/](http://data.threesixtygiving.org/datastore/)

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
     "publisher": {
        "name":"Name of the organisation publishing this dataset",
        "website":"Should be a valid URL to a website of that publisher",
        "logo":"Should be a valid URL to a logo for that publisher. 
                You may not necessarily have permission to use this 
                logo for your own purposes."
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


## Credits
This site uses Jekyll and the base Jekyll theme.  
You can find the source code for the Jekyll new theme at:
{% include icon-github.html username="jglovier" %} /
[jekyll-new](https://github.com/jglovier/jekyll-new)  
You can find the source code for Jekyll at
{% include icon-github.html username="jekyll" %} /
[jekyll](https://github.com/jekyll/jekyll)
