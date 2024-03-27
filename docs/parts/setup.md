<!-- See https://squidfunk.github.io/mkdocs-material/reference/ -->
# Part 1: Setup

To run this workshop you will need access to an Equinix Fabric Account or create a new one following step 1 below.

> **_Note:_**  You are responsible for the cost of resources created in your Equinix Fabric account while running this workshop.

## Pre-requisites

The following tools will be needed on your local development environment where you will be running most of the commands in this guide.

* [pulumi](https://www.pulumi.com/docs/install/)
* [python](https://www.python.org/downloads/)
* Optional (but recommended): [Google Cloud CLI](https://cloud.google.com/sdk/docs/install?hl=es-419)

## Steps

### 1. Create Equinix Fabric credentials - Access Token

If you have never used Equinix Fabric API before, please follow the [Getting Access Token](https://developer.equinix.com/docs?page=/dev-docs/fabric/overview) instructions.

### 2. Configure Google Cloud credentials (if installed)

Pulumi can authenticate to Google Cloud via several methods: Google Cloud CLI, OpenID Connect (OIDC), Service account. Whether you choose to use the CLI or another method, please follow the [Installation & Configuration](https://www.pulumi.com/registry/packages/gcp/installation-configuration/#authentication-methods) instructions.

### 2. Clone the template repository

To create a Pulumi project from a specific source control location, you need to pass the url to the `pulumi new` command:

```shell
$ pulumi new https://github.com/equinix-labs/pulumi-equinix-fabric-cloud-router-gcp
```

This command not only will download the template but will walk you through creating a new [Pulumi project](https://www.pulumi.com/docs/concepts/projects/#projects), creating a new [Pulumi stack](https://www.pulumi.com/docs/concepts/stack/#stacks), will create a python virtual environment and install the dependencies defined in the repository requirements.txt file.

### 3. Verify

If everything worked correctly, the output should look like this:

```shell
Finished installing dependencies

Your new project is ready to go! ✨

To perform an initial deployment, run `pulumi up`

warning: A new version of Pulumi is available. To upgrade from version '3.100.0' to '3.111.1', run 
   $ curl -sSL https://get.pulumi.com | sh
or visit https://pulumi.com/docs/install/ for manual instructions and release notes.
```

## Discussion

Before proceeding to the next part let's take a few minutes to discuss what we did. Here are some questions to start the discussion.

* In what scenarios do you believe the limitations of Pulumi providers, as highlighted in the introduction, might pose significant challenges during real-world infrastructure deployments? How might you mitigate these challenges?
