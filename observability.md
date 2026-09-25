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
    - check whether it's on by going to the `/challenge` path of an application
    - You can also see current logs in the nomad UI
    - You should be able to see it in the load balancer UI as the first upstream defined for any application that's using it
    - the [signoz logs](https://signoz.lib.princeton.edu/logs/logs-explorer?relativeTime=3d&compositeQuery=%257B%2522queryType%2522%253A%2522builder%2522%252C%2522builder%2522%253A%257B%2522queryData%2522%253A%255B%257B%2522dataSource%2522%253A%2522logs%2522%252C%2522queryName%2522%253A%2522A%2522%252C%2522aggregateOperator%2522%253A%2522count%2522%252C%2522aggregateAttribute%2522%253A%257B%2522id%2522%253A%2522----%2522%252C%2522dataType%2522%253A%2522%2522%252C%2522key%2522%253A%2522%2522%252C%2522type%2522%253A%2522%2522%257D%252C%2522timeAggregation%2522%253A%2522rate%2522%252C%2522spaceAggregation%2522%253A%2522sum%2522%252C%2522filter%2522%253A%257B%2522expression%2522%253A%2522service.name%2520in%2520%255B%27traefik%27%255D%2522%257D%252C%2522aggregations%2522%253A%255B%257B%2522expression%2522%253A%2522count%28%29%2520%2522%257D%255D%252C%2522functions%2522%253A%255B%255D%252C%2522filters%2522%253A%257B%2522items%2522%253A%255B%257B%2522id%2522%253A%25224f96be3c-58a8-4eef-9f3e-20fd08c631fd%2522%252C%2522op%2522%253A%2522in%2522%252C%2522key%2522%253A%257B%2522id%2522%253A%2522service.name%2522%252C%2522key%2522%253A%2522service.name%2522%252C%2522dataType%2522%253A%2522string%2522%252C%2522type%2522%253A%2522resource%2522%257D%252C%2522value%2522%253A%2522traefik%2522%257D%255D%252C%2522op%2522%253A%2522AND%2522%257D%252C%2522expression%2522%253A%2522A%2522%252C%2522disabled%2522%253Afalse%252C%2522stepInterval%2522%253Anull%252C%2522having%2522%253A%257B%2522expression%2522%253A%2522%2522%257D%252C%2522limit%2522%253Anull%252C%2522orderBy%2522%253A%255B%255D%252C%2522groupBy%2522%253A%255B%255D%252C%2522legend%2522%253A%2522%2522%252C%2522reduceTo%2522%253A%2522avg%2522%252C%2522source%2522%253A%2522%2522%257D%255D%252C%2522queryFormulas%2522%253A%255B%255D%252C%2522queryTraceOperator%2522%253A%255B%255D%257D%252C%2522promql%2522%253A%255B%257B%2522name%2522%253A%2522A%2522%252C%2522query%2522%253A%2522%2522%252C%2522legend%2522%253A%2522%2522%252C%2522disabled%2522%253Afalse%257D%255D%252C%2522clickhouse_sql%2522%253A%255B%257B%2522name%2522%253A%2522A%2522%252C%2522legend%2522%253A%2522%2522%252C%2522disabled%2522%253Afalse%252C%2522query%2522%253A%2522%2522%257D%255D%252C%2522id%2522%253A%2522b378226f-23dd-418b-8bad-87e83b644932%2522%252C%2522unit%2522%253A%2522%2522%257D&options=%7B%22selectColumns%22%3A%5B%7B%22name%22%3A%22timestamp%22%2C%22signal%22%3A%22logs%22%2C%22fieldContext%22%3A%22log%22%2C%22fieldDataType%22%3A%22%22%2C%22isIndexed%22%3Afalse%7D%2C%7B%22name%22%3A%22body%22%2C%22signal%22%3A%22logs%22%2C%22fieldContext%22%3A%22log%22%2C%22fieldDataType%22%3A%22%22%2C%22isIndexed%22%3Afalse%7D%5D%2C%22maxLines%22%3A1%2C%22format%22%3A%22raw%22%2C%22fontSize%22%3A%22small%22%7D) for traefik show the request's protected path, and the series of nginx config stanzas that request passed through as well as the VM that ultimately served the request.
