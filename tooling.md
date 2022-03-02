# Development Tooling

## Shared Tools

* [Github](https://github.com/pulibrary) for code
  * Use [dls-github-labeler](https://github.com/pulibrary/dls-github-labeler) to generate an initial set of labels
* [CircleCI](https://circleci.com/gh/pulibrary) for CI
* [Rubocop](https://github.com/bbatsov/rubocop) for style guidelines enforcement
  * [Bixby](https://github.com/samvera-labs/bixby) for Samvera defaults
* [Lando](https://lando.dev/) for running service dependencies like solr and postgres
* [HoneyBadger](https://www.honeybadger.io/), [DataDog](https://app.datadoghq.com/) and [Sensu](https://lib-monitor.princeton.edu/dashboard) for error tracking and monitoring
* [VPN](https://princeton.service-now.com/snap?sys_id=6023&id=kb_article) for connecting to our staging applications
* [Lastpass](https://informationsecurity.princeton.edu/LastPass) for shared passwords
* [SignalSciences](https://dashboard.signalsciences.net/) for analyzing incoming web traffic and identifying/blocking attacks

## Individual Tools

* __Editors__: Use what you're comfortable with. Several members of DLS use vim. Many other editors are used on various development teams.
* __Language version management__: DLS projects include configuration files for asdf. princeton_ansible uses pipenv.
* __Terminal management__: We use tmux for terminal management on servers when needed, and many of us use it locally.
* __Wireframing and Diagraming__: We have institutional access to Adobe XD and Lucid Charts. Other tools we have used include Google Drawings and websequencediagrams.com. Try [Mermaid](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/) for markdown-based diagrams that will live on github.
* __Browser testing__: We have a few licenses for BrowserStack.
* __Other tools__ used by members of our team include: zsh, [rcm dotfiles management](https://github.com/thoughtbot/rcm), [thoughtbot's dotfiles](https://github.com/thoughtbot/dotfiles), [oh my zsh](https://ohmyz.sh/)

We frequently share new tooling discoveries and tips between teams at our all-hands
meetings.
