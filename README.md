
# Firefox Browser Architecture

## Vision

Build the world’s best web browser

## Strategy

Our top priority is to plan for where we want to go, but if we just think 5 years out, we’ll miss the dragon on the doorstep. So we need to look from both angles:

1. Look forward from where we are now: **Move faster**
2. Look backwards from where we want to get to: **Consciously plan our architecture**

## Our Conclusions

This is a list of our findings that we're reasonably happy with so far.

* [Documenting our output](text/0001-documenting-output.md) looks at how we’re going to communicate with the rest of Mozilla.
* [Extracting Necko](text/0002-extracting-necko.md) considers whether it's feasible or worthwhile to extract Necko — Gecko's C++ networking library — for use as a standalone component.
* [Problems with XUL](text/0003-problems-with-xul.md) aims to list the different kinds of problems that exist with XUL.
* [XBL and Web Components](text/0004-xbl-web-components.md) compares some old Mozilla technology (XBL) with modern Web Components.
* [Problems with XBL](text/0005-problems-with-xbl.md) aims to list the different kinds of problems that exist with XBL.
* [Roadmap Reviews](text/0006-roadmap-review-process.md) are healthy and we proposed a process for healthy reviews (**this document is incomplete and in-progress**).
* [Design Reviews](text/0007-design-review-process.md) are healthy and we proposed a process for healthy reviews (**this document is incomplete and in-progress**).

## Posts

We typically send our newsletters to [firefox-dev](https://www.mozilla.org/en-US/about/forums/#firefox-dev).

{% for post in site.categories.newsletter reversed %}
* [{{ post.title }}]({{ site.baseurl }}{{ post.url }}): {{ post.description }} [[mailing-list-post]({{ post.mailinglist }})]{% endfor %}

## Explorations and Experiments

To support our conclusions we occasionally perform explorations and experiments. The first exploration is designed to support the notion that we can create a sync and storage layer in Rust that we can deploy to Desktop, Android and iOS.

* [Deploying an Rust library on iOS](experiments/2017-09-06-rust-on-ios.md). A short tutorial describing how to build and deploy a rust library for use inside an iOS app.
