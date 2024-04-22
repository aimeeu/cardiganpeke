---
title: Tech writing philosophy
weight: 1
description: >
  This page contains my views on authoring and reviewing technical content.
---

## Authoring philosophy

I was a software developer as well as an end user, so I approach content creation from that viewpoint. I am as comfortable creating UML diagrams to illustrate concepts as I am creating tutorials and guides.

I strongly believe in separating long, explanatory content from guides and tutorials. You can read more about this approach on GitLab's [Documentation topic types (CTRT) page](https://docs.gitlab.com/ee/development/documentation/topic_types/index.html) and the [Diátaxis website](https://diataxis.fr/). 

| GitLab CTRT | Diátaxis |
| ------------ | ----------- |
| Concept      | Explanation |
| Task    | How-to guide |
| Reference    | Reference |
| Troubleshooting    | (not defined) |
| Tutorials    | Tutorials  |
| Get started    |  (not defined)  |

**However, I do follow the content and style guides of the company I'm working for or the open source community to which I'm contributing.**

### Content types

DITA (Darwin Information Typing Architecture) is a [method for organizing content](https://technicalwriterhq.com/writing/technical-writing/darwin-information-typing-architecture-dita/) as well as a [method for authoring content](https://www.oasis-open.org/committees/dita/faq.php).

Tom Johnson's [What is Diátaxis and should you be using it with your documentation?](https://idratherbewriting.com/blog/what-is-diataxis-documentation-framework) is an interesting read, especially since Tom compares Diátaxis to DITA, [Information Mapping](https://informationmapping.com/), and [The Good Docs Project](https://thegooddocsproject.dev/).

Here are a few presentations on Diátaxis:

* [Introducing the Diátaxis Approach to Technical Documentation](https://www.brighttalk.com/webcast/9273/594742) (2023)
* Two-part workshop (2022):
  * [Python Docs Community Workshop: Introduction to Diataxis](https://www.youtube.com/watch?v=710uQqIqsWk) 
  * [Python Docs Community Workshop: Getting Things Done](https://www.youtube.com/watch?v=ECXtMPx-4uQ)
* [Daniele Procida - Always complete, never finished](https://www.youtube.com/watch?v=Wc7n7uIg4AM) (2021)
* [What nobody tells you about documentation](https://www.youtube.com/watch?v=t4vKPhjcMZg)  (2017)

Although I have never authored content using DITA tools, I have organized content using a DITA approach. What I found was that users preferred feature-based or function-based navigation, so I put explanatory pages and guides within each feature folder but put Tutorials in a Tutorials section.

### Ordered lists versus headings in a task page

For basic guides, I generally try to follow the structure outlined in GitLab’s [Task topic type guide](https://docs.gitlab.com/ee/development/documentation/topic_types/task.html). However, some guides are more involved, with code snippets, bash output, and potentially screenshots in each step. In that case, I like to create each step as a header. The structure looks similar to this:

```markdown
## Overview plus objectives
   The objectives are in a list with each bullet point a link to the relevant heading.
   Do the following:
   1. [Do this](#do-this)
   2. [Do that](#do-that)
   3. [Do other things](#do-other-things)
## Prerequisites
	 unordered list
## Do this
	 step, config snippet, bash output
## Do that
## Do other things
## Related content   
```

The user can skip to a desired section by using the page navigation or by clicking on the objective in the overview section.

## Content review philosophy

Over the years, I've noticed that "good content" is highly subjective and varies considerably between tech writing teams. Software engineers and tech writers often have different ideas about what constitutes good documentation.

### **The three Cs**

Content should be clear, concise, and consistent.

I ask myself the following when analyzing content:

* Does the content meet the stated goal of the page? Does every section support the page’s purpose?
* Does the page title reflect the content type? This helps readers scan search results, whether in-app or from an internet search provider.
  * Tasks start with an active verb.
  * Tutorials start with an active verb and have “tutorial” in the title (provided that’s in the style or content guide). Again, this format is good for scanning search results.
  * Concept and reference start with a noun.
* Do the page headings follow a consistent format? 
  * For a task in which each step is a heading, the heading starts with a verb.
  * For a concept, the heading is a noun or noun phrase.
* Is the writing concise?
  * Does it use as few words as possible to convey meaning, so readers can easily scan the content? 
  * Is the content organized in a logical flow?
  * Are there long sentences which could be shorter or made less complex?
  * Is there long content that would be better presented as a bullet list or table?
  * Is there content that can be replaced with a diagram? (UML or other) A picture **is** worth a thousand words. 
* If there is a list, do the list elements have parallel syntax?
* If there are tables or lists of command line switches or configuration fields, in which all items have equal weight, are the items presented in alphabetical order? (easier to scan)
* Do global variables and terms have the same name as on other pages? 
* Is any content not 100% clear? (For example, is something optional vs required)
* If task or tutorial, do the steps work?
* Is the content technically correct?
* Can any of the content be presented in a tabbed component to save page space?

I have additional questions for when I review reference material such as API, CLI, and system config files because as a former software developer, I expect to see very specific content there.

If the team has content and style guides, my review ensures that the content follows those guides. If the team or open source project doesn't, I volunteer to contribute those guides.

By creating clear, concise, and consistent content that flows logically, tech writers produce documentation that meets or exceeds reader expectations.

### Site navigation

All items being of equal weight, is the left nav in alphabetical order? That makes navigation easier to scan.

### SEO review

https://developers.google.com/search/docs/beginner/seo-starter-guide for in-depth SEO guidelines and explanations.

#### Page file names

Use [simple, human-readable, and logical URL paths for your pages](https://developers.google.com/search/docs/advanced/guidelines/url-structure) and provide clear and direct internal links within the site.

#### Page titles

Google analyzes the content of the page, catalogs images and video files embedded on the page, and otherwise tries to understand the page.

When listing search results, Google truncates longer page titles but still finds keywords in the entire title when building the index.

**Create short, meaningful titles that accurately reflect the page content.** Include relevant keywords. Do not sacrifice accuracy (or keyword) for brevity. Armory's priority is accurate/descriptive page titles, but do your best to keep them a manageable length.

#### Guidelines

To improve search ranking placement, keep these in mind when editing and approving content:

* Title should be descriptive and contain keywords if possible. Use natural language and ensure that the content of the page is clearly expressed.
  * Titles should be no longer than _60 characters_  _maximum_. 55 is preferred.
  * Go from unbranded to branded terms as appropriate.
  * All titles should be unique.
  * The title should not be the same as a heading (H2) on the page.
* Front matter `description`  turns into a `meta` tag when compiled.
  * Description should be no longer than 160 characters and also contain keywords because search engines look for.
  * Make sure that the language is natural and clearly describes what the user finds on the page.
  * Do not make it a duplicate of the title.
  * Make it enticing and clear. For example, what you learn, what problems it solves,  etc.
* H2 and H3 tags should be contain keywords if it makes sense. Heading tags send valuable ranking signals to Google and provide context to bots.
  * "Overview of pipelines" rather than "Overview".
  * "Prerequisites for deploying to …" rather than "Prerequisites"  (Yes, it may be repetitive but SEO rankings are voodoo).
* Short intro sections directly below heading (1-2 sentences is enough) that include the keyword target.
* Link to other relevant content using keyword-focused anchor text.
  * Anchor text sends ranking signals to Google. When you use keywords in the anchor text, that reinforces the keyword targeting of the linked page. Plus, it can be clearer for users and shows them exactly what the link they're clicking focuses on.
  * In general, internal links between pages are powerful for SEO. When you link from a high-ranking, high-traffic page to another page, it passes some of that page's power on to other areas of the site.
* Page URLs
  * Ensure that the URL is human-readable and clearly conveys the page content. If/as applicable include the priority keyword in the url.
  * Use only lower case and hyphens.
* Images
  * Ensure that all images have alt tags that are clear descriptions of what the images express. Include keyword(s) if/as appropriate.
  * Ensure that the image name is human readable and conveys what the image is

### Best practices

**Reviewers**

* Be polite, helpful, and considerate of others.
* Comment on positive aspects of a PR, as well as changes.
* Be empathetic and mindful of how your changes or review may be received.
* Make sure your review comments are **con**structive not **de**structive.
* Ask clarifying questions if something in a PR is unclear.
* Assume positive intent.
* If you are an experienced contributor, consider pairing with new contributors whose work requires extensive changes.

**Approvers**

* Ask your fellow contributors how they work best and what communication style they prefer.
* If you are asking for a lot of changes on a review, make sure at least one comment is a positive one.
* Do not turn a review into a sparring match.
* Avoid changing content other than typos or broken links.
* Ask clarifying questions in a way that doesn't put the author on the defensive
* If you think there's a better way to present content, mention it in your review and then ask what the author thinks.
* If you notice style guide violations, politely point out the issue, or use the GitHub **Insert a suggestion** [functionality](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/commenting-on-a-pull-request#adding-line-comments-to-a-pull-request) to suggest a change, and then link to the relevant section in the style guide to explain why you are suggesting the change. The most common style guide violation is using passive voice instead of active voice.
