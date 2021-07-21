---
title: Add Static HTML and Empty Upstream
description: How and when to use empty upstreams as part of the Built Tools setup process.
categories: [get-started]
tags: [upstreams, site]
reviewed: "2021-07-21"
---

UPDATE THIS! Select the site's framework during the [site creation process](/create-sites). Pantheon Upstreams provide default installations of WordPress, Drupal 9, Drupal 8, and Drupal 7.

[Custom Upstreams](/custom-upstream) are available to team members when the organization is associated during site creation.

## What Is an Empty Upstream and When Do I  Use It?

An empty upstream is a repository that is devoid of all content. It is appropriate to use an upstream in situations where a Pantheon site will be created through a build step (refer to the [Terminus Build Tools Plugin](https://github.com/pantheon-systems/terminus-build-tools-plugin)) and managed completely by [Composer](https://pantheon.io/docs/composer). Typically, the build step should completely replace the content provided by the upstream.

If this upstream is used to install a site that does not have a build step, then you will not be able to install or use your site. In that event, the best thing to do would be to delete it and start over, either by selecting a different upstream, or by using the Terminus Build Tools Plugin `terminus build-env:create-project` command to set up a build server.

## More on How Pantheon Uses Empty Upstream Here:

- [Switch Upstreams](/terminus/examples#switch-upstreams)
- [Drupal 8 and Composer on Pantheon Without Continuous Integration](/guides/drupal-8-composer-no-ci#creating-the-pantheon-site)