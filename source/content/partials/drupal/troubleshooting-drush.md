---
contenttype: [partial]
categories: [update]
cms: [drupal9]
product: [--]
integration: [drush]
tags: [--]
reviewed: ""
---

## Site-local Drush Is Required for Drupal Sites

Do not remove `drush/drush` from `composer.json`. If it is removed, `terminus drush` commands will fail with errors related to Twig.

