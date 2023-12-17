# Datalift Helm Chart
[![Artifact HUB](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/datalift)](https://artifacthub.io/packages/search?page=1&org=datalift)

This repository contains the official Datalift Helm chart for installing
and configuring Datalift on Kubernetes.

## Prerequisites

To use the charts here, [Helm](https://helm.sh/) must be installed in your
Kubernetes cluster. Setting up Kubernetes and Helm and is outside the scope
of this README. Please refer to the Kubernetes and Helm documentation.

The versions required are:

  * **Helm 3.0+** - This is the earliest version of Helm tested. It is possible
    it works with earlier versions but this chart is untested for those versions.
  * **Kubernetes 1.20+** - This is the earliest version of Kubernetes tested.
    It is possible that this chart works with earlier versions but it is
    untested.

In addition to Helm, you must also have a:

  * **Datalift API Token**

## Usage

#### Install the Helm Chart

Before installing the chart, you must create two Kubernetes secrets:

To use the charts, you must add the Datalift Helm Chart repository.

```shell
$ helm repo add datalift https://charts.datalift.io
"datalift" has been added to your repositories

$ helm install datalift datalift/datalift
```

Please see the many options supported in the `values.yaml` file. These are also
fully documented directly on the [Datalift website](https://datalift.io/docs/helm)
along with more detailed installation instructions.
