# Bootiq

**Current stable release:** [1.0.1](https://github.com/Bootiga-SaaS/bootiq/releases/tag/1.0.1)

Bootiq is an open-source, premium storefront package for Drupal Commerce Kickstart. It installs the Bootiq theme, reusable Layout Builder blocks, and the installer that connects them.

Bootiq is developed and maintained by [Bootiga](https://www.bootiga.com). It can be used independently and does not require a Bootiga account.

Bootiq does not create products, articles, stores, users, or other demo content.

![Bootiq storefront](screencapture-test24-bootiga-2026-06-12-11_50_18.png)

## Features

- Conversion-focused Drupal Commerce storefront.
- Responsive catalog, product, cart, login, blog, and legal-page styling.
- Editable Hero, product grid, blog, The Look, and related-product sections.
- Layout Builder integration.
- Image upload controls for editable storefront sections.
- No bundled demo products, users, or store data.

## Requirements

- Commerce Kickstart 5.1.
- Drupal 10 or 11.
- PHP and extensions required by Commerce Kickstart.
- Composer 2.
- Drush supplied by the target project.

## Install

~~~bash
composer require bootiga/bootiq:^1.0
./vendor/drush/drush/drush en bootiq_installer -y
./vendor/drush/drush/drush bootiq:install
~~~

The `^1.0` constraint installs the latest compatible 1.x release (currently 1.0.1); it does not pin the installation to 1.0.0.

Use **bootiq:install --force** on an existing Kickstart demo when Bootiq should replace its storefront configuration and Layout Builder displays. Without **--force**, existing storefront configuration is preserved.

## Packages

- [bootiga/bootiq-theme](https://github.com/Bootiga-SaaS/bootiq-theme): frontend theme.
- [bootiga/bootiq-product-blocks](https://github.com/Bootiga-SaaS/bootiq-product-blocks): reusable Layout Builder storefront blocks.
- [bootiga/bootiq-installer](https://github.com/Bootiga-SaaS/bootiq-installer): dependencies, configuration, and Drush installer.

## About Bootiga

[Bootiga](https://www.bootiga.com) is a hosted Drupal Commerce platform for launching and managing online stores without giving up an open-source stack or ownership of the site. Bootiga does not add a platform commission to store sales, and stores can be moved away from the service.

- [Visit Bootiga](https://www.bootiga.com)
- [Bootiga documentation](https://www.bootiga.com/docs)
- [Bootiq source code](https://github.com/Bootiga-SaaS/bootiq)

## Contributing

Bug reports and feature requests are welcome in [GitHub Issues](https://github.com/Bootiga-SaaS/bootiq/issues).

## License

GPL-2.0-or-later.
