---
layout: default
title: Applications
---
# DLS Applications

[Architecture diagram](https://docs.google.com/drawings/d/1qqHoceL4nahv8wmhK_QltL8f1StdBJ5GYFpIa6JQ3PA/edit)

## Applications in active development

### DPUL (Digital PUL)
A digital exhibits and collections application for showcasing Figgy content, built on Spotlight.
  * [DPUL production](https://dpul.princeton.edu/), [DPUL staging](https://dpul-staging.princeton.edu/)
  * [Github repository](https://github.com/pulibrary/dpul)
  * [Zenhub board](https://app.zenhub.com/workspaces/dpul-5cc9dbb2262a972347170639/board?repos=49439415&showEstimates=false&showReleases=false)
  * Technical liaison: [Anna](https://github.com/hackartisan)
  * Product owner: [Kim](https://github.com/kelea99)
  * Technical slack channel: #figgy
  * User-centered slack channel: #digital_library

### Figgy
Our digital repository: a staff application for managing digital object ingest and metadata workflows. Figgy also provides IIIF manifests and viewers to other applications.
  * [Figgy production](https://figgy.princeton.edu), [Figgy staging](https://figgy-staging.princeton.edu)
  * [Github repository](https://github.com/pulibrary/figgy)
  * [Zenhub board](https://app.zenhub.com/workspaces/figgystudio-5c06d2e24b5806bc2bfa890b/board)
  * Technical liaison: [Trey](https://github.com/tpendragon)
  * Product owner: [Kim](https://github.com/kelea99)
  * Technical slack channel: #figgy
  * User-centered slack channel: #digital_library

### Maps Portal, aka PULMap
A discovery and access application for maps and geospatial data, built on GeoBlacklight.
  * [PULMap production](https://maps.princeton.edu)
  * [Github repository](https://github.com/pulibrary/pulmap)
  * [Zenhub board](https://app.zenhub.com/workspaces/pulmap-5cf5538c08e7e9307cd79c45/board?repos=26446857)
  * Technical liaison: [Eliot](https://github.com/eliotjordan)
  * Product owner: [Kim](https://github.com/kelea99)
  * Technical slack channel: #geo
  * User-centered slack channel: #geo

### Finding Aids, aka PULFALight
A discovery application for archival and special collections materials, built on Arclight
  * [Finding Aids production](https://findingaids.princeton.edu)
  * [Github repository](https://github.com/pulibrary/pulfalight)
  * [Zenhub board](https://app.zenhub.com/workspaces/pulfalight-5da4b7d9f037f100019dba23/board?repos=157741631)
  * Technical liaison: [Shaun](https://github.com/sdellis)
  * Product owners: [Faith](https://github.com/faithc) and [Christa](https://github.com/ccleeton)
  * Slack channel: #pulfalight

## Applications in active maintenance

### AbID
A staff-facing site for absolute ID management Application. Generates absolute identifiers and eases barcode entry for physical items managed in aspace.
  * [AbID production](https://abid.princeton.edu/), [AbID staging](https://abid-staging.princeton.edu/)
  * [GitHub repository](https://github.com/pulibrary/abid)
  * Technical slack channel: #pulfalight-tech
  * User-centered slack channel: #pulfalight

### Imagecat (aka the Supplementary Catalog)
A searchable collection of scanned catalog cards
  * [Imagecat production](https://imagecat.princeton.edu/), [Imagecat staging](https://imagecat-staging.princeton.edu/)
      * Note both are only accessible when on VPN
  * [Github repository](https://github.com/pulibrary/imagecat-rails)
  * Technical slack channel: #figgy
  * User-centered slack channel: #digital_library

### LAE-Blacklight
A discovery and access application for PUL's Latin American Ephemera collections
  * [LAE production](https://lae.princeton.edu)
  * [Github repository](https://github.com/pulibrary/lae-blacklight)
  * Technical liaison: [Trey](https://github.com/tpendragon), transfer to [Eliot](https://github.com/eliotjordan)
  * Technical slack channel: #figgy
  * User-centered slack channel: #digital_library


## Our Tooling Repositories
* [dls-handbook](https://github.com/pulibrary/dls-handbook)
* [dls-github-labeler](https://github.com/pulibrary/dls-github-labeler)
* [rails-template](https://github.com/pulibrary/rails-template)

## Cloud Services

We run a few services in the cloud, the following has information on where the
code is and which cloud they run on.

### IIIF image server
  * Production host name: iiif-cloud.princeton.edu
  * Cloud Service: AWS
  * [Github repository](https://github.com/pulibrary/serverless-iiif)
  * Technical liaison: TBD
  * Product owner: TBD
  * Technical slack channel: #figgy
  * User-centered slack channel: #digital_library

### TiTiler AWS
Amazon CDK configurations for deploying TiTiler, a map tile server
  * Production host name: map-tiles.princeton.edu
  * Cloud Service: AWS
  * [Github repository](https://github.com/pulibrary/geoservices-aws/blob/main/geoservices/titiler_service_stack.py)
  * Technical slack channel: #geo
  * User-centered slack channel: #geo

###  Geodata AWS
Amazon CDK configurations for deploying and providing access control for PMTiles vector data
  * Production host name: geodata.lib.princeton.edu
  * Cloud Service: AWS
  * [Github repository](https://github.com/pulibrary/geoservices-aws/blob/main/geoservices/geodata_stack.py)
  * Technical slack channel: #geo
  * User-centered slack channel: #geo

### Cloud Preservation Fixity Checker
Google cloud function to check the fixity for Figgy's preserved files and report
back.
  * Production host name: n/a
  * Cloud Service: Google
  * [Github repository](https://github.com/pulibrary/figgy/tree/main/cloud_fixity)
  * Technical slack channel: #figgy
  * User-centered slack channel: #digital_library

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
* [GeoServer](http://geoserver.org/) - Geo data server, in production at
  [https://geoserver.princeton.edu/geoserver/web/](https://geoserver.princeton.edu/geoserver/web/)
* [Cantaloupe](https://github.com/medusa-project/cantaloupe) - IIIF image API server
* Isilon - storage
* Nginx+ - load balancer
* [Kakadu](http://kakadusoftware.com/downloads/) - for generating JP2s
* [Tesseract](https://github.com/tesseract-ocr/tesseract) - OCR software
* Characterization tools
  * [FITS](https://projects.iq.harvard.edu/fits) - default Samvera/Hyrax characterization
  * [Tika](https://tika.apache.org/) - (part of FITS) Apache text analysis/parsing framework
  * [JHove](https://github.com/openpreserve/jhove) - (part of FITS) good TIFF validation
