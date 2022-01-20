# DLS Applications

[Architecture diagram](https://docs.google.com/drawings/d/1qqHoceL4nahv8wmhK_QltL8f1StdBJ5GYFpIa6JQ3PA/edit)

## DPUL (Digital PUL)
Spotlight exhibits for showcasing Figgy content
  * [DPUL production](https://dpul.princeton.edu/), [DPUL staging](https://dpul-staging.princeton.edu/)
  * [Github repository](https://github.com/pulibrary/dpul)
  * [Zenhub board](https://app.zenhub.com/workspaces/dpul-5cc9dbb2262a972347170639/board?repos=49439415&showEstimates=false&showReleases=false)
  * Technical liaison: [Anna](https://github.com/hackmastera)
  * Product owner: [Kim](https://github.com/kelea99)
  * Technical slack channel: #figgy
  * User-centered slack channel: #digital_library

## Figgy
Internal application for managing digital object ingest and metadata workflows and providing IIIF manifests to other applications
  * [Figgy production](https://figgy.princeton.edu), [Figgy staging](https://figgy-staging.princeton.edu)
  * [Github repository](https://github.com/pulibrary/figgy)
  * [Zenhub board](https://app.zenhub.com/workspaces/figgystudio-5c06d2e24b5806bc2bfa890b/board)
  * Technical liaison: [Trey](https://github.com/tpendragon)
  * Product owner: [Kim](https://github.com/kelea99)
  * Technical slack channel: #figgy
  * User-centered slack channel: #digital_library

## IIIF image server
  * Production host name: iiif-cloud.princeton.edu
  * [Github repository](https://github.com/pulibrary/serverless-iiif)
  * Technical liaison: TBD
  * Product owner: TBD
  * Technical slack channel: #figgy
  * User-centered slack channel: #digital_library

## LAE-Blacklight
Latin American Ephemera frontend
  * [LAE production](https://lae.princeton.edu)
  * [Github repository](https://github.com/pulibrary/lae-blacklight)
  * Technical liaison: [Trey](https://github.com/tpendragon), transfer to [Eliot](https://github.com/eliotjordan)
  * Technical slack channel: #figgy
  * User-centered slack channel: #digital_library

## Maps Portal, aka PULMap
GeoBlacklight app for maps and geo data discovery and access
  * [PULMap production](https://maps.princeton.edu)
  * [Github repository](https://github.com/pulibrary/pulmap)
  * [Zenhub board](https://app.zenhub.com/workspaces/pulmap-5cf5538c08e7e9307cd79c45/board?repos=26446857)
  * Technical liaison: [Eliot](https://github.com/eliotjordan)

## TiTiler AWS
Amazon CDK configurations for deploying TiTiler, a map tile server
  * production: map-tiles.princeton.edu
  * [Github repository](https://github.com/pulibrary/titiler-aws)

## Finding Aids, aka PULFALight
Local instance of arclight
  * [Finding Aids production](https://findingaids.princeton.edu)
  * [Github repository](https://github.com/pulibrary/pulfalight)
  * [Zenhub board](https://app.zenhub.com/workspaces/pulfalight-5da4b7d9f037f100019dba23/board?repos=157741631)
  * Technical liaison: [Shaun](https://github.com/sdellis)
  * Product owners: [Faith](https://github.com/faithc) and [Amanda](https://github.com/apferrar)
  * Slack channel: #pulfalight


## Our Tooling Repositories
* [dls-handbook](https://github.com/pulibrary/dls-handbook)
* [dls-github-labeler](https://github.com/pulibrary/dls-github-labeler)
* [rails-template](https://github.com/pulibrary/rails-template)


## Cross-team Applications

Some applications cross teams or organizations and are central to our work.

* [Lux](https://github.com/pulibrary/lux)
* [PULBot](https://github.com/pulibrary/pulbot) and [Heaven](https://github.com/pulibrary/heaven) - Slack bot for deployments
  * Slack channels: #robots, #devs
* [PUL-Solr](https://github.com/pulibrary/pul_solr) - Central repository of solr configs for our apps
  * Slack channel: #solr
* [Princeton Ansible](https://github.com/pulibrary/princeton_ansible) -
  playbooks for all of our server provisioning
* [Valkyrie](https://github.com/samvera-labs/valkyrie) - samvera persistence
  layer on which Figgy is built

## Related Applications and Services

* [CAS](https://www.princeton.edu/cas) - authentication
* [GeoServer](http://geoserver.org/) - Geo data server
* [Cantaloupe](https://github.com/medusa-project/cantaloupe) - IIIF image API server
* Isilon - storage
* Nginx+ - load balancer
* [Kakadu](http://kakadusoftware.com/downloads/) - for generating JP2s
* [Tesseract](https://github.com/tesseract-ocr/tesseract) - OCR software
* Characterization tools
  * [FITS](https://projects.iq.harvard.edu/fits) - default Samvera/Hyrax characterization
  * [Tika](https://tika.apache.org/) - (part of FITS) Apache text analysis/parsing framework
  * [JHove](https://github.com/openpreserve/jhove) - (part of FITS) good TIFF validation
