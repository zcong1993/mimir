---
title: "Deploying the Grafana Mimir monitoring mixin"
menuTitle: "Deploying the monitoring mixin"
description: "Learn how to deploy the Grafana Mimir monitoring mixin."
weight: 20
---

# Deploying the Grafana Mimir monitoring mixin

Grafana Mimir exposes a `/metrics` endpoint returning Prometheus metrics.
The endpoint is exposed on the Mimir HTTP server address / port which can be customized through `-server.http-listen-address` and `-server.http-listen-port` CLI flags or their respective YAML [config options]({{< relref "../configuring/reference-configuration-parameters/index.md" >}}).

## Dashboards and alerts

Grafana Mimir is shipped with a comprehensive set of production-ready Grafana dashboards and alerts to monitor the state and health of a Mimir cluster.

Dashboards provide both a high-level and in-depth view of every aspect of a Grafana Mimir cluster.
You can take a look at all the available dashboards in [this overview]({{< relref "dashboards/_index.md" >}}).

Alerts allow you to monitor the health of a Mimir cluster. For each alert, we provide detailed [playbooks](https://github.com/grafana/mimir/blob/main/operations/mimir-mixin/docs/playbooks.md) to further investigate and fix the issue.

The [requirements documentation]({{< relref "requirements.md" >}}) lists prerequisites for using the Grafana Mimir dashboards and alerts.

The [installation instructions]({{< relref "installing-dashboards-and-alerts.md" >}}) show available options to install Grafana Mimir dashboards and alerts.
