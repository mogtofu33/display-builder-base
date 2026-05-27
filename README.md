## Display Builder base

Drupal recipe documentation: https://www.drupal.org/docs/extending-drupal/drupal-recipes

This recipe is designed to do the following:

- Install certain parts of Standard install profile that we want
- Set specific UI Suite and **Display Builder** modules configuration
- Set specific contributed module configuration
- Provide a starting point for Drupal ready to develop with** Display Builder**
  and **UI Styles** ecosystem modules.

## Installing

- Start with a Drupal 11 site
- Install the 'Minimal' profile
- Apply the recipe

The recipe can be applied with PHP in Drupal 11.3+.

Execute this command from the web root:

```shell
php core/scripts/drupal recipe recipes/contrib/display_builder_base
```

Or by using `ddev exec`

```shell
ddev exec -d /var/www/html/web php core/scripts/drupal recipe recipes/contrib/display_builder_base
```

If all goes well, you should see the following output:

```shell
[OK] Display Builder Base applied successfully
```

Clear the cache after the recipe is applied. When going back to the site,
all the recipe configuration and customization has been applied.
