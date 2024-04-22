---
title: How-to guide samples
linkTitle: How-to guides
description: >
  This page shows samples of how-to guides that I wrote while working for Armory.
---


## Guides overview

- GitLab: Task
- Diátaxis : How-to guide

I used two approaches for structuring guides:

- Use a numbered list for steps.
- Use separate sections for steps. In this case, declare the objectives in a list in the **Overview** section and include links to the specific headings.

{{< readfile file="/includes/caveat.md" >}}

## Configure a temporary preview link to a deployed service

>I received brief notes from the engineer who implemented the feature. I then created the CD-as-a-Service deployment configuration YAML file and then used the Armory CLI to deploy the sample app that Armory engineers built for demos. 

This guide isn't strictly a guide. It's structured more like reference material in some parts. The original location was in the **Deployment** section, and through Hugo front matter magic, also appeared in the **Reference** section. This content needs to be updated for clarity.

{{< figure src="configure-preview-link.png" width="80%" height="80%" >}}

## Configure traffic management with Istio

>For this guide, I learned how to configure and deploy Istio to my Kubernetes cluster. Then I configured and deployed Istio's demo app. I did not receive a demo, first draft, or notes from the engineers.

{{< figure src="configure-istio.png" >}}

## Use Armory's GitHub Action to deploy your app using CD-as-a-Service

>I did not receive a demo, first draft, or notes from the engineers. The PM talked to me about this feature.

{{< figure src="use-github-action.png" >}}
