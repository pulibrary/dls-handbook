# Development Tooling

In addition to this handbook page, we also have a document [How-to for core and
common
tasks](https://docs.google.com/document/d/1PRgujNUnLNklfXjWeQ4TeyxG3sULDCVfKR1x29HH9j0/edit#) which we encourage team members to add to.

## Standard DLS development tools
Make sure these are installed for your individual setup. Many / most of these are also used on other PUL IT teams

* [homebrew](https://brew.sh/) for package management on macs
  * When projects have required dependencies, homebrew install instructions are provided in the readme
* [asdf](https://asdf-vm.com/) for language version management
  * All DLS projects include the `.tool-versions` configuration files for asdf
* [docker desktop](https://www.docker.com/products/docker-desktop/) for development dependencies
  * DLS projects are set up using lando (see below) which requires docker
* git for version control
  * You'll also need a [Github](https://github.com/pulibrary) account
* [Lastpass](https://informationsecurity.princeton.edu/LastPass) for shared passwords

## Standard project tooling

The tools we use to configure, support, and monitor our applications

* Use [dls-github-labeler](https://github.com/pulibrary/dls-github-labeler) to generate an initial set of labels
* [CircleCI](https://circleci.com/gh/pulibrary) for CI
* [Bixby](https://github.com/samvera-labs/bixby) ruby style enforcement that wraps [Rubocop](https://github.com/bbatsov/rubocop) and provides defaults determined by the Samvera open source community
* [Lando](https://lando.dev/) for running service dependencies like solr and postgres
* [HoneyBadger](https://www.honeybadger.io/), [DataDog](https://app.datadoghq.com/), and [Sensu](https://lib-monitor.princeton.edu/dashboard) for error tracking and monitoring
* [VPN](https://princeton.service-now.com/snap?sys_id=6023&id=kb_article) for connecting to our staging applications
* [SignalSciences](https://dashboard.signalsciences.net/) for analyzing incoming web traffic and identifying/blocking attacks
* tmux is on all our servers to allow us to run long tasks without risking
  connection loss. Several of us use it locally with vim.

## Individual Tools

* __Editors__: Use what you're comfortable with. VSCode is a good choice. Several members of DLS use vim. Many other editors are used on various development teams.
* __Wireframing and Diagraming__
  * We have institutional access to Adobe XD and Lucid Charts
  * websequencediagrams.com lets you code your diagram with text and then export
    it as an image
  * Try [Mermaid](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/) for markdown-based diagrams that will live on github.
* For __Browser testing__ we have a few licenses for BrowserStack.
* __Other tools__ used by members of our team include
  * [thoughtbot's dotfiles](https://github.com/thoughtbot/dotfiles)
    * which uses [rcm dotfiles management](https://github.com/thoughtbot/rcm)
  * zsh and [oh my zsh](https://ohmyz.sh/)
  * [github command line interface](https://github.com/cli/cli)

We frequently share new tooling discoveries and tips between teams at our all-hands
meetings and on our #devs slack channel.
