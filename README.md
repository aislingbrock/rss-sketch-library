# rss-sketch-library
Testing using RSS to update a Sketch library

## In the XML file
To push an update, the Pubdate and Sparkle version both need to be updated. 

`<pubDate>Tue, 15 Sep 2020 17:00:04 +0000</pubDate>`

`<enclosure url="https://github.com/aislingbrock/rss-sketch-library/blob/master/sketch-library.sketch?raw=true" type="application/octet-stream" sparkle:version="3"/>`

The URL for the library should be the raw url that contains `?raw=true`

Note: I had initially tried the version number as 0.2 and an update wasn't pushed so I'm not sure how it deals with decimals. We will need to test this further.

## Download the library

In your browser, go to (markdown doesn't seem to want to make it a link, something else to look into): 

`sketch://add-library?url=https%3A%2F%2Fgithub.com%2Faislingbrock%2Frss-sketch-library%2Fraw%2Fmaster%2Fsketch-library.xml`

## Resources

[The original article where most of this work originates](https://medium.com/sovanta-design-lab/autoupdate-sketch-libraries-via-rss-584687de5b12)
