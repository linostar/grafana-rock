# grafana-rock

[![Open a PR to OCI Factory](https://github.com/canonical/grafana-rock/actions/workflows/rock-release-oci-factory.yaml/badge.svg)](https://github.com/canonical/grafana-rock/actions/workflows/rock-release-oci-factory.yaml)
[![Publish to GHCR:dev](https://github.com/canonical/grafana-rock/actions/workflows/rock-release-dev.yaml/badge.svg)](https://github.com/canonical/grafana-rock/actions/workflows/rock-release-dev.yaml)
[![Update ROCK](https://github.com/canonical/grafana-rock/actions/workflows/rock-update.yaml/badge.svg)](https://github.com/canonical/grafana-rock/actions/workflows/rock-update.yaml)

[ROCKs](https://canonical-rockcraft.readthedocs-hosted.com/en/latest/) for [Grafana](https://grafana.com/).  
This repository holds all the necessary files to build ROCKs for the upstream versions we support. The Grafana ROCK is used by the [grafana-k8s-operator](https://github.com/canonical/grafana-k8s-operator) charm.

The ROCKs on this repository are built with [OCI Factory](https://github.com/canonical/oci-factory/), which also takes care of periodically rebuilding the images.

Automation takes care of:
* validating PRs, by simply trying to build the ROCK;
* pulling upstream releases, creating a PR with the necessary files to be manually reviewed;
* releasing to GHCR at [ghcr.io/canonical/grafana:dev](https://ghcr.io/canonical/grafana:dev), when merging to main, for development purposes.

