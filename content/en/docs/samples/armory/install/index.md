---
title: Product Installation Samples
linkTitle: Product Install Guides
description: >
  This page shows samples of installation guides that I wrote while working for Armory.
---

## Overview

Armory had two standalone product lines:

* Armory Continuous Deployment Self-Hosted (CDSH), an enterprise version of open source [Spinnaker](https://spinnaker.io/).

  * Engineers created the docs site and wrote the majority of content before Armory hired tech writers. I created content and style guides, but to be honest, the tech writing team never had the resources to review and update existing content.
  * Original docs website: https://docs.armory.io/continuous-deployment/
  * Original public GitHub repo: https://github.com/armory/docs/

* Spinnaker Plugins, feature plugins for Spinnaker and Armory Continuous Deployment Self-Hosted.

  * I created the _Spinnaker Plugins_ top-level directory and refactored some existing content into it. The engineers and I created the majority of the content in the plugins directory. When it made sense, I used a DITA-based organization. However, readers and product managers preferred a feature-based site navigation. The PMs and I were working on refactoring when Harness bought Armory.
  * Original docs website: https://docs.armory.io/plugins/
  * Original public GitHub repo: https://github.com/armory/docs/plugins/

I wrote these installation guides during my first two years at Armory.

I used Snagit’s scrolling feature to capture the screenshots. The main body content is correct, but you do see duplicate left and right menus due to the scrolling capture.

## Armory Continuous Deployment Self-Hosted install guides

### Install Operator and deploy Armory Continuous Deployment quickstart

>I created this guide without a demo, first draft, or notes from the engineers.

{{< figure src="cdsh-operator-quickstart.png" width="80%" height="80%" >}}

### Install from the AWS Marketplace

>I created this guide with notes from a sales engineer.

{{< figure src="install-from-aws-marketplace.png" width="80%" height="80%" >}}

### Air-gapped overview and installation

>I created this guide with notes from a sales engineer.

{{< figure src="air-gapped-overview.png" width="80%" height="80%" >}}

{{< figure src="air-gapped-install.png" width="80%" height="80%" >}}

## Spinnaker plugins

### Scale Agent

This example shows how to install the Scale Agent in Spinnaker using the Spinnaker Operator.

>A sales engineer provided notes and the Kubernetes manifests.

{{< figure src="scale-agent-spinnaker.png" width="80%" height="80%" >}}

{{< figure src="configure-scale-agent.png" width="80%" height="80%" >}}

### GitHub Integration plugin

This example shows how to install the GitHub Integration plugin in Spinnaker using Halyard.

>I created this using notes from an engineer.

{{< figure src="github-int-plugin-install-halyard.png" width="80%" height="80%" >}}

## Install Armory CDSH in AWS EC2 using K3s

I wrote this shortly after I started with Armory. It's based on notes I took while learning to use the product. One of the sales engineers provided instructions for configuring Lightweight Kubernetes to be publicly accessible when running on an EC2 instance.

This page became outdated and is no longer in production.

I should not have included instructions and screenshots for how to create an S3 bucket or IAM role. Instead, I should have stated what the user needs and then linked to relevant AWS docs.

{{< figure src="operator-k3s-ec2.png" width="80%" height="80%" >}}
