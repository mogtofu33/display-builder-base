# Display Builder Base

Drupal recipe documentation:

- [https://www.drupal.org/docs/extending-drupal/drupal-recipes](https://www.drupal.org/docs/extending-drupal/drupal-recipes)
- [https://project.pages.drupalcode.org/distributions_recipes/getting_started.html](https://project.pages.drupalcode.org/distributions_recipes/getting_started.html)

This recipe is designed to:

- Install selected components from the Standard install profile
- Provide a Drupal starting point that is ready for development with **Display Builder**
  and **UI Styles** ecosystem modules.
- Add contributed modules for a minimum viable site:
  - easy_breadcrumb
  - link_attributes
  - pathauto
  - redirect
  - simple_sitemap
  - sitemap
  - smart_trim
  - token

This recipe is intended to set up a complete site from scratch and meet core
project expectations.

It is intended to be used as a base for a Display Builder theme recipe, such as
[Display Builder Bootstrap Recipe](https://www.drupal.org/project/display_builder_bootstrap).

For more information, visit [Display Builder](https://www.drupal.org/project/display_builder) and
[UI Suite](https://www.drupal.org/project/ui_suite).

## Installation

- Start with a Drupal **11.3+** site
- Install the `Minimal` profile
- Apply the recipe

You can apply the recipe using PHP in Drupal **11.3+**.

Run this command from the web root:

```shell
php core/scripts/drupal recipe recipes/contrib/display_builder_base
```

Or by using `ddev exec`:

```shell
ddev exec -d /var/www/html/web php core/scripts/drupal recipe recipes/contrib/display_builder_base
```

If the command succeeds, you should see the following output:

```shell
[OK] Display Builder Base applied successfully
```

**Clear the cache** after applying the recipe.

When you return to the site, all recipe configuration and customizations should
be in place.
