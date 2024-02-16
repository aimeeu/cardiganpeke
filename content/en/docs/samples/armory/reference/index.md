---
title: Reference Samples
linkTitle: Reference
description: >
  This page contains samples of reference material that I wrote while working for Armory.
---

## CLI

{{< readfile file="/includes/caveat.md" >}}

**Product**: Armory Continuous Deployment-as-a-Service

Armory Continuous Deployment-as-a-Service didn't have an exposed REST API, but it did have two CLIs. I originally created CLI cheat sheets with the aim of moving to CLI docs generated when the CLI projects released a version. Instead, the PM, engineering team, and I decided to enhance the documentation in each CLI's help. I worked with the engineers on language and reviewed all pull requests that contained user-facing output.

## Deployment config file

**Product**: Armory Continuous Deployment-as-a-Service

The Armory Continuous Deployment-as-a-Service reference material detailed the sections of the deployment config file.

{{< figure src="ref-artifacts-provider.png" width="80%" height="80%" >}}

## REST API

**Product**: Armory Scale Agent

The docs team worked with the engineers to add comments to the REST API code and then generate a Swagger JSON file upon product release. The docs then displayed the content using the Docsy theme's [swaggerui](https://www.docsy.dev/docs/adding-content/shortcodes/#swaggerui) tag. We ultimately decided not to include the REST API reference content in that format. Instead, I manually created the REST API reference with help from the engineers.

Had Armory not been acquired, I would have investigated using a tool like [Stoplight](https://stoplight.io/) for API docs.

Original public repo: https://github.com/armory/docs/tree/master/content/en/plugins

Original public site: https://docs.armory.io/plugins/scale-agent/tasks/dynamic-accounts/manage-accounts/

{{< figure src="scale-agent-rest-api.png" width="80%" height="80%" >}}
