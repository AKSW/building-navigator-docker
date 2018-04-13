# Building Navigator Docker Environment

Development docker environment for building navigator with [k000ni/docker-nodejs-environment](https://hub.docker.com/r/k00ni/docker-nodejs-environment/) and [tenforce/virtuoso](https://hub.docker.com/r/tenforce/virtuoso/)

# Setup

Clone [Building Navigator](https://github.com/AKSW/building-navigator/) and this repo and download the datadump (places.n3)(https://github.com/AKSW/transform-bvl-pages-to-csv-file). Adjust the volume to the building navigator folder and the data dump in `docker-compose.yml`.

# Run

Run `docker-compose up` and visit http://localhost:8080 in you browser.

## Development

See [Building Navigator](https://github.com/AKSW/building-navigator/) readme to get more information about development.

## Resources:

Building Navigator: https://github.com/AKSW/building-navigator/

Data dump: https://github.com/AKSW/transform-bvl-pages-to-csv-file
