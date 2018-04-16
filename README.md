# Building Navigator Docker Environment

Development docker environment for building navigator with Nodejs and [tenforce/virtuoso](https://hub.docker.com/r/tenforce/virtuoso/)

# Setup

Clone [Building Navigator](https://github.com/AKSW/building-navigator/) and this repo and download the datadump [places.n3](https://github.com/AKSW/transform-bvl-pages-to-csv-file). Adjust the volume to the building navigator folder and the data dump in `docker-compose.yml`.

# Run

Run `docker-compose up` to start the container.

Visit the virtuoso conductor at http://localhost:8890 in you browser, login width dba:dba and enable CORS requests. (follow [this guide](https://virtuoso.openlinksw.com/dataspace/doc/dav/wiki/Main/VirtTipsAndTricksCORsEnableSPARQLURLs)

The building navigator is accessible at http://localhost:8080.

## Development

See [Building Navigator](https://github.com/AKSW/building-navigator/) readme to get more information about development.

## Resources:

Building Navigator: https://github.com/AKSW/building-navigator/

Data dump: https://github.com/AKSW/transform-bvl-pages-to-csv-file
