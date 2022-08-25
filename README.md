# Grafana Dataflow Dashboard

This chart template files are used from official grafana Helm chart.

Dataflow Dashboard JSON [dataflow-dashboard.json](./grafana/dashboards/dataflow-dashboard.json)

```
helm repo add grafana https://grafana.github.io/helm-charts
helm repo update 
```

## Prerequisites

- Stackdriver datasource in grafana
- Helm cli tool

## usage

### 1. Clone the repo

```
git clone https://github.com/knoldus/grafana-dataflow-dashboard
cd grafana-dataflow-dashboard
```

### 2. Deploy the chart

```
helm upgrade --install grafana grafana -f grafana/custom-values.yaml -n grafana --create-namespace
```

### 3. Add variables for your dataflow job & GCP project in dashboard