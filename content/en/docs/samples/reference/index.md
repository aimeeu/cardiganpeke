---
title: Reference Samples
linkTitle: Reference
description: >
  This page contains samples of reference material that I wrote while working for Armory.
---

## Armory Continuous Deployment-as-a-Service

{{< readfile file="/includes/caveat.md" >}}

Armory Continuous Deployment-as-a-Service didn't have an exposed REST API. It did have a CLI, and we decided to build the documentation into the CLI's help. I worked with the engineers on language and reviewed all pull requests that contained user-facing output.

The Armory Continuous Deployment-as-a-Service reference material detailed the sections of the deployment config file.

{{< figure src="ref-artifacts-provider.png" width="80%" height="80%" >}}

## Armory Scale Agent

The docs team worked with the engineers to add comments to the REST API code and then generate a Swagger JSON file upon product release. The docs then displayed the content using the Docsy theme's [swaggerui](https://www.docsy.dev/docs/adding-content/shortcodes/#swaggerui) tag. We ultimately decided not to include the REST API reference content in that format. Instead, we manually created the REST API reference.

{{< figure src="scale-agent-rest-api.png" width="80%" height="80%" >}}
