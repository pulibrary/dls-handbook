# Observability

## List of platforms in use by PUL IT and/or DLS

* [HoneyBadger](https://www.honeybadger.io/)
    * see also [pulibrary/pul-it-handbook/services/honeybadger.md](https://github.com/pulibrary/pul-it-handbook/blob/main/services/honeybadger.md)
    * Used for error tracking per-project.
    * Also used for some uptime monitors, though TODO not sure if those are working / on?
* [DataDog](https://app.datadoghq.com/)
    * see also [pulibrary/pul-it-handbook/services/datadog.md](https://github.com/pulibrary/pul-it-handbook/blob/main/services/datadog.md)
    * Used for apm and log aggregation
    * VM-level metrics with dashboards (especially network volume, latency)
    * Service health metrics and dashboard, powered by data from our health endpoints
* [CheckMK](https://pulmonitor.princeton.edu/)
    * there's also a `/staging` instance
    * see also [pulibrary/pul-it-handbook/services/checkmk.md](https://github.com/pulibrary/pul-it-handbook/blob/main/services/checkmk.md)
    * Monitoring and alerts, especially lower-level metrics
* [SigNoz](https://signoz.lib.princeton.edu/login)
    * Currently in trial implementation
    * use "sign in with SSO"
    * provides log aggregation and APM
* [Grafana](https://grafana-nomad.lib.princeton.edu)
    * sign in with github
    * Set up by DLS to quickly implement project-specific metrics
    * Temporary home for some stats and dashboards that may move to signoz
    * Runs on nomad
