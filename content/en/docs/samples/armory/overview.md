---
title: Overview
weight: 1
description: >
  This page details what I worked on while employed by Armory.
---

## My time at Armory

I started as a Technical Writer on December 2, 2019, joining Brian, who was hired in August of 2019. We reported to the VP of Product. The team grew to three tech writers and a manager. Eventually people moved on to other companies, and I was the sole tech writer for over a year. I was responsible for all aspects of Armory product documentation across all product lines. During my time at Armory, I wore many hats and performed many duties beyond writing content.

When Harness acquired Armory in late 2023, Harness effectively retired Armory products, transitioning users to Harness' products.

## Armory Continuous Deployment-as-a-Service (CDaaS)

* This public docs website is no longer available.
* Public GitHub [repo](https://github.com/armory/docs-cdaas) - view my [68 merged pull requests](https://github.com/armory/docs-cdaas/pulls?q=is%3Apr+is%3Amerged+author%3Aaimeeu+)

I was the sole tech writer for this product and created the vast majority of the content with minimal input from the engineers. However, engineers and product managers did review my pull requests for technical accuracy.

This site started out with a DITA-based navigation consisting of Get Started, Concepts, Guides, Reference, Tutorials, Troubleshooting, and Release Notes. However, CDaaS users preferred feature-based navigation, so the Product Manager and I refactored to serve our readers. Each feature directory contained separate concept and guide material. Tutorials remained in the Tutorials section.

>The GitHub repo shows many contributors. That is not correct and is the result of how I created the repo. The CDaaS content was originally part of the Armory Continuous Deployment Self-Hosted `docs` repo. To create the CDaaS repo, I copied the `docs` repo and then [ripped out all but the CDaaS content](https://github.com/armory/docs-cdaas/pull/8) in the new `docs-cdaas` repo. The `docs-cdaas` repo therefore retained the commit history from the `docs` repo. In hindsight, I should have not created the `docs-repo` that way. Lesson learned.

## Armory Continuous Deployment Self-Hosted (CDSH)

* [Website](https://docs.armory.io/continuous-deployment/)
* Public GitHub [repo](https://github.com/armory/docs/) - view my [422 merged pull requests](https://github.com/armory/docs/pulls?q=is%3Apr+is%3Amerged+author%3Aaimeeu+)

Engineers created much of the CDSH content in the three years before I arrived at Armory. After my arrival, the small docs team never had the bandwidth to update existing content to match the style and content guides I wrote, or to ensure content was up-to-date.

I created product installation and plugin creation guides.

The original Armory documentation was in the `armory/documentation` [repo](https://github.com/armory/documentation). I was instrumental in porting the docs from Jekyll to Hugo, which substantially improved build times, page loading, and reader experience. I contributed [15 pull requests](https://github.com/armory/documentation/pulls?q=is%3Apr+is%3Amerged+author%3Aaimeeu+) to the old repo before the docs team and I ported the content. Significant contributions to the old repo included [Installing Spinnaker in GKE using Operator](https://github.com/armory/documentation/pull/853/files) and also the [Operator reference docs](https://github.com/armory/documentation/pull/820).

### Spinnaker Plugins

The Spinnaker Plugins content is in the Armory Continuous Deployment Self-Hosted repo.

* [Website](https://docs.armory.io/plugins/)
* Public GitHub [repo](https://github.com/armory/docs/)

I created this top-level section and moved the existing plugin content from the main CDSH docs to this new section. We then added new plugin material.

I created content based on user stories, technical design docs, and collaboration with engineers who were not native English speakers. Additionally, without help from the engineers, I created instructions for installing the plugin on Spinnaker using either the Spinnaker Operator or Halyard, plus instruction for installing into CDSH using the `spinnaker-kustomize-repo`. Then I asked for technical reviews to ensure the content was correct.

The Scale Agent plugin content illustrates DITA-based navigation. The Product Manager and I had started planning for refactoring to a feature-based navigation when Armory was acquired.  
