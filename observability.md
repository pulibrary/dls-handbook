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

## Scenarios

### Are our prod sites up?

You can look at the little [status page](https://status.hbuptime.com/BKASRM) honeybadger builds for us.

### Slow or intermittent site

Long load times or "bad gateway" errors

- Check APMs for large latency times for the page that's reported as slow
- Dashboards for CPU and Memory use (or run htop on boxes)
- Curl from localhost and from load balancer to check for network latency from various places
- Tigerdata mount point (for figgy): `ls /mnt/tigerdata`
- Passenger queue sizes: `sudo passenger-status`
    - if the queue is full, look at the requests `sudo passenger-status --show=requests > requests.txt`
- Search logs for patterns in requests
    - Is everything erroring or just some things?
    - There are logs from the load balancer, logs from the local web server, application logs, and traefik logs
    - note the status code isn't always correctly parsed from the log line
    - search for any unusual error messages you find - stackoverflow, the project's ticketing system, reddit
- Traefik
    - This [traefik Network diagram](https://github.com/pulibrary/princeton_ansible/tree/main/nomad/traefik-wall) is a helpful reference
    - Dashboard: [Traefik's view of server health](https://grafana-nomad.lib.princeton.edu/d/efk2tpxbeeccgc/service-uptime-percentage-over-time?from=now-30m&to=now&timezone=browser)
