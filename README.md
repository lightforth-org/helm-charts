# Lightforth Generic Helm Chart
This is a generic helm chart for lightforth infra, this chart can be used for any types of deployment.

## Features
A generic Helm chart offers several key features that make it a powerful tool for managing Kubernetes applications:

1. **Deployment Speed**: You can deploy applications quickly using pre-configured charts available in the Helm repository.
2. **Prebuilt Configurations**: Helm charts come with community-supported configurations, making it easier to deploy complex applications without needing to write extensive Kubernetes manifests.
3. **Easy Rollbacks**: Helm allows you to roll back to previous versions of your application if something goes wrong during deployment.
4. **Version Control**: Helm charts are versioned, allowing you to pin specific versions and track changes over time.
5. **Modularity**: Helm charts can have dependencies and sub-charts, which are automatically managed during deployment.
6. **Customization**: You can modify existing charts or create your own to suit specific application requirements.
7. **Reusable Templates**: Helm uses templates to define Kubernetes resources, making it easier to manage and reuse configurations.

## How To Use Lightforth Generic Helm Chart

Add The Helm Repo

`helm repo add lightforth https://helm.lightforth.org`

## Modify The Custom Values File
From the repo, there's an override file called `custom-values.yaml`, modify this with your values.

## Deploy Services With The Helm Chart
To make deployment

```helm install <projectname> lightforth/lightforth -f custom-values.yaml -n <namespace> --create-namespace```

**Examples**

```helm install ms-resume-stage lightforth/lightforth -f custom-values.yaml -n ms-resume-stage --create-namespace```
