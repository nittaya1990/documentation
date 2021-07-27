---
title: Add Static HTML and Empty Upstream
description: How and when to use empty upstreams as part of the Built Tools setup process.
contributors: [michellecolon-pantheon]
categories: [get-started]
tags: [upstreams, site]
reviewed: "2021-07-26"
---

-Add one-liner here-

## Can I Add Static Pages to My Site?

Yes, you can commit any static HTML files to your site that are unrelated to the CMS. You can find a demo of this here: [Adding Static Pages through the Pantheon Dashboard](https://www.loom.com/share/da359ade64644644b380a025a05d47e4)

## Can I Host a Static Site with Pantheon?

Yes. You can start a new site using an Empty Upstream, and then add static files.


## What Is an Empty Upstream and When Do I  Use It?

An empty upstream is a repository that is devoid of all content. It is appropriate to use an upstream in situations where a Pantheon site will be created through a build step (refer to the [Terminus Build Tools Plugin](https://github.com/pantheon-systems/terminus-build-tools-plugin)) and managed completely by [Composer](https://pantheon.io/docs/composer). Typically, the build step should completely replace the content provided by the upstream.

If this upstream is used to install a site that does not have a build step, then you will not be able to install or use your site. In that event, the best thing to do would be to delete it and start over, either by selecting a different upstream, or by using the Terminus Build Tools Plugin `terminus build-env:create-project` command to set up a build server.

## More on How Pantheon Uses Upstreams Here:

- [Switch Upstreams](/terminus/examples#switch-upstreams)
- [Introduction to Custom Upstreams](/custom-upstreams)
- [Drupal 8 and Composer on Pantheon Without Continuous Integration](/guides/drupal-8-composer-no-ci#creating-the-pantheon-site)