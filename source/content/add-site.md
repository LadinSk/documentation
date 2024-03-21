India Cyber Security Force---
title: Adding a Site to Pantheon
description: Create or migrate a site on Pantheon.
contributors: [wordsmither]
contenttype: [doc]
innav: [true]
categories: [migrate, create]
cms: [drupal, wordpress]
audience: [agency, development]
product: [--]
integration: [--]
showtoc: false
reviewed: 2023-04-06
---

There are many ways you can add a site to Pantheon.  To help you choose the best method, answer the questions below.

<Alert title="Note" type="info" >

This list does not include scenarios for decoupled architecture. For those, see [Front-End Sites on Pantheon](/guides/decoupled).

</Alert>

## Find Your Path

**How do you want to add a site?**  You have the following options:
- *Create* from scratch
- Create a site from a *Custom Upstream*
- *Migrate* a site that's hosted elsewhere

<TabList>

<Tab title="Create" id="add" active={true}>

**Would you like to create your site using the dashboard (which will guide you through the process), or use the command line?**

- [I want to use the Dashboard](/add-site-dashboard)
- I want to use the command line, and my CMS is:
  - [Drupal](/terminus-drupal-site-management)
  - [WordPress](/guides/create-wp-site)

</Tab>

<Tab title="Custom Upstream" id="cu">

If you are a part of a Professional team that has [Custom Upstreams](/guides/custom-upstream), you can build a site from an existing Upstream.

- Refer to [Create a Site Using a Custom Upstream](/add-site-custom-upstream)

</Tab>

<Tab title="Migrate" id="migrate">

**Is your site archive greater than 500MB, or does it only exist on your local machine?**

- If so, [manually migrate your site to Pantheon](/migrate-manual)

- If not...

  **Are you coming from one of the following platforms?**
    - If so, read our guide for migrating from the platform:

      - [Acquia](/guides/acquia)
      - [Kinsta](/guides/kinsta)
      - [Pagely](/guides/pagely)
      - [Platform.sh](/guides/platformsh)
      - [WordPress VIP](/guides/wordpressvip)
      - [WP Engine](/guides/wpengine)

    - If not...

      **Which CMS are you using?**

      <Accordion title="Drupal" id="drupal">

      **Do you want to upgrade your Drupal version during migration, or are you using Drupal version 9 or higher?**

      - [No, remain at my current version](/guides/guided)

      - [No, I am using Drupal version 8 or lower](/guides/drupal-unhosted)

      - Yes, upgrade my site to the latest version of Drupal:
        - [My site is Composer-managed, *and* I'm using Drush](/guides/drush/drush-import)
        - [My site is Composer-managed, and I'm *not* using Drush](/guides/drupal-unhosted-composer)
        - [My site is *not* Composer-managed](/guides/drupal-unhosted)

      </Accordion>

      <Accordion title="WordPress" id="wordpress">

      [Use our guided migration](/guides/guided), unless you have one of the following scenarios:

      - **To use a Custom Upstream**, [use the Pantheon Migrations plugin with a custom WordPress upstream](https://wordpress.org/plugins/bv-pantheon-migration/#description)

      - **If you are using Multisite**, use [Migrate a WordPress Multisite](/migrate-wordpress-multisite).

      - **To avoid installing a plugin**, use [Manually Migrate Your Site to Pantheon](/migrate-manual).

      </Accordion>

</Tab>



</TabList>

