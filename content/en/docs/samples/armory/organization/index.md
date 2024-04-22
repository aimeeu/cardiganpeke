---
title: Content organization
linkTitle: Content organization
description: >
  This page shows examples of different approaches to organizing content.
---

## How to organize content

Very early in Armory's history, the engineers created the Armory Continuous Deployment docs site. They organized content into varies guides, such as admin and installation. That organization had been in place for 3 years when Armory hired tech writers, so we left the organization as it was.

The docs team and I had more leeway with new content. The examples on this page show content organization decisions I made, and these decisions were approved by the team and product managers.

I used Snagit’s scrolling feature to capture the screenshots. The main body content is correct, but you do see duplicate left and right menus due to the scrolling capture.

## DITA-based approach

Since Armory's users were familiar with the [Kubernetes](https://kubernetes.io/docs/home/) and [Spinnaker](https://spinnaker.io/docs/) docs, I created the Scale Agent organization based on the approached used by those docs sets.

Original public repo: https://github.com/armory/docs/tree/master/content/en/plugins

Original public site: https://docs.armory.io/plugins/scale-agent/tasks/dynamic-accounts/manage-accounts/

{{< figure src="scale-agent-org.png"  >}}

## Feature-based approach

I had originally used the Concepts and Guides sections approach with the Armory Continuous Deployment-as-a-Service docs. 

- **Situation**: After the docs site had been live for about a year, the software engineers developing the product expressed that they couldn’t find anything on the docs site. The customer feedback had been “great content” with no feedback on the navigation. The content was divided into Concepts, Guides, Troubleshooting, Tutorials, Reference. Concepts and Guides sections were organized by features.
- **Task**: My task was to ask for feedback from design partners and possibly change site navigation.
- **Action**: I talked to the design partners, who reiterated how good the content was. When asked specifically about site navigation, they admitted sometimes it took too many clicks to find what they were looking for. So I did the initial reorganization on paper and then met with the PM to finalize.
- **Result**: The feedback from design partners was again positive. They liked that concepts and guides were grouped by feature. The PMs liked that users could see all the features in a single glance.

Original public repo: https://www.github.com/armory/docs-cdaas/

{{< figure src="cdaasLandingPage1.jpg" >}}

{{< figure src="cdaasLandingPage2.jpg"  >}}