# Building Navigator Docker Environment

Development docker environment for building navigator with Nodejs and [tenforce/virtuoso](https://hub.docker.com/r/tenforce/virtuoso/)

# Setup

Clone [Building Navigator](https://github.com/AKSW/building-navigator/) and this repo and download the datadump [places.n3](https://github.com/AKSW/transform-bvl-pages-to-csv-file). Adjust the volume to the building navigator folder and the data dump in `docker-compose.yml`.

# Run

Run `docker-compose up` to start the node and db container.

## Enable Virtuoso CORS:

Visit the virtuoso conductor at http://localhost:8890 in you browser, login width dba:dba and got to "Web Application Server" -> "Virtual Domains & Directories". Click on the (blue) 0.0.0.0 default web site folder icon and _Edit_ the `/sparql` path. Enter "*" (without quotes) in the "Cross-Origin Resource Sharing" field and save changes.

Guide: http://vos.openlinksw.com/owiki/wiki/VOS/VirtTipsAndTricksCORsEnableSPARQLURLs

The building navigator should accessible at http://localhost:8080.

## Development

See [Building Navigator](https://github.com/AKSW/building-navigator/) readme to get more information about development.

## Resources:

Building Navigator: https://github.com/AKSW/building-navigator/

Data dump: https://github.com/AKSW/transform-bvl-pages-to-csv-file
