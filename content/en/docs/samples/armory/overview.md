---
title: Overview
weight: 1
description: >
  This page details what I worked on while employed by Armory.
---

## My time at Armory

I started as a Technical Writer on December 2, 2019, joining Brian Le, who was hired in August of 2019. I ended as a Principal Technical Writer. I wore many hats and performed many duties beyond writing content.

When Harness acquired Armory, I had been the sole tech writer for 20 months, so I was responsible for all aspects of Armory product documentation across all product lines.

## Armory Continuous Deployment-as-a-Service (CDaaS)

* [Website](https://developer.armory.io/)
* Public GitHub [repo](https://github.com/armory/docs-cdaas)

I was the sole tech writer for this product and created the vast majority of the content with minimal input from the engineers. 

This site started out with a DITA-based navigation consisting of Get Started, Concepts, Guides, Reference, Tutorials, Troubleshooting, and Release Notes. However, CDaaS end users preferred feature-based navigation, so the Product Manager and I refactored to serve our readers. Each feature directory contains separate concept and task material. Tutorials remained in the Tutorials section.

>The GitHub repo shows many contributors. That is not correct and is the result of how I created the repo. The CDaaS content was originally part of the Armory Continuous Deployment Self-Hosted `docs` repo. To create the CDaaS repo, I copied the `docs` repo and then [ripped out all but the CDaaS content](https://github.com/armory/docs-cdaas/pull/8) in the new `docs-cdaas` repo. The `docs-cdaas` repo therefore retained the commit history from the `docs` repo. In hindsight, I should have not created the `docs-repo` that way. Lesson learned.

## Armory Continuous Deployment Self-Hosted (CDSH)

* [Website](https://docs.armory.io/continuous-deployment/)
* Public GitHub [repo](https://github.com/armory/docs/)

Engineers created much of the CDSH content in the three years before I arrived at Armory. After my arrival, the small docs team never had the bandwidth to update existing content to match the style and content guides I wrote, or to ensure content was up-to-date.

I created product installation and plugin creation guides.

## Spinnaker Plugins

* [Website](https://docs.armory.io/plugins/)
* Public GitHub [repo](https://github.com/armory/docs/)

I created this top-level section and moved the existing plugin content from the main CDSH docs to this new section. We then added new plugin material.

I created content based on user stories, technical design docs, and collaboration with engineers who were not native English speakers.

Each plugin should have three installation options: Armory CDSH, Spinnaker – Operator, and Spinnaker- Halyard. I created the install YAML since the engineers often forgot to include it. Then I asked for technical reviews to ensure the content was correct.

The Scale Agent plugin content illustrates DITA-based navigation. The Product Manager and I had started planning for refactoring to a feature-based navigation when Armory was acquired.  
