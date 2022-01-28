# Prometheus/Alertmanager/Grafana Integration Demo for PagerDuty

![License MIT](https://img.shields.io/badge/license-MIT-blue.svg)

Docker Compose file uses the following images:
* [prom/prometheus](https://hub.docker.com/r/prom/prometheus)
* [prom/alertmanager](https://hub.docker.com/r/prom/alertmanager)
* [grafana/grafana](https://hub.docker.com/r/grafana/grafana)

## Setup

Open `alertmanager/alertmanager.yml` and update line 4 with your PagerDuty integration key (see [Event Orchestration](https://support.pagerduty.com/docs/event-orchestration)).

## Usage

Start the Docker containers:

    docker-compose up -d

## Prometheus

View in a browser at: http://localhost:9000/alerts

## Alertmanager

View in a browser at: http://localhost:9093/#/alerts

## Grafana

View in a browser at: http://localhost:3000/

Username: `admin`

Password: `admin`