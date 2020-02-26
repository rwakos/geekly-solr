#Geekly Workshop | DB Search Engines with Solr
##Examples

1.- How to fetch all data
`q=*.*`

2.- How to limit the results
`q=*.*&rows=10`

3.- How to search in texts by partials
`q=quote:insp*&rows=10`

4.- How to search in texts by words
`q=quote:book&rows=10`

5.- Find words at least two words apart
`quote:"enjoyed writing"~2`

6.- Filter against a numeric type
`page:2`

7.- Filter against a range of numeric type
`page:[1 TO 5]`

8.- Highlight a searched word "enjoyed"
`hl.fl=quote&hl.simple.post=<%2Fstrong>&hl.simple.pre=<strong>&hl=on&q=quote%3Aenjoyed&rows=5`

9.- Highlight a searched partial word "enjoy*"
`hl.fl=quote&hl.simple.post=<%2Fstrong>&hl.simple.pre=<strong>&hl=on&q=quote%3Aenjoyed&rows=5`

10.- Facets by the field tag
`facet.field=tags&facet=on&q=*%3A*&rows=0`

11.- Facets by the field page
`facet.field=page&facet=on&q=*%3A*&rows=0`

12.- Facet range by year
`q=*:*&rows=0&facet=on&facet.range=quoted_at&facet.range.start=NOW-10YEAR&facet.range.end=NOW&facet.range.gap=%2B1YEAR`

13.- Spatial search within a radius


14.- Sorting by distance


###References
Quotes taken from: https://www.goodreads.com/quotes/tag/books
Cities with geolocations: https://simplemaps.com/data/world-cities
