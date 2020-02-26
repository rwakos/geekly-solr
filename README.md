# geekly-solr
Workshop Solr @Geekly

Create a folder called "data" inside the "solr" folder.

Do a `docker-compose up -d` to build and run the image.

After it finishes, go to a browser and type the url:

`http://127.0.0.1:8983`

If success, do a `docker-compose down`. Go to the folder "solr/config", and copy the file "managed-schema", and overwrite the file at "solr/data/phrases/conf", to replace the schema.

After that, start the container once more.

`docker-compose up -d`


### References
Quotes taken from: https://www.goodreads.com/quotes/tag/books

Cities with geolocations: https://simplemaps.com/data/world-cities