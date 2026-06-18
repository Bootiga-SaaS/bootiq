# Bootiq

Modern Drupal Commerce theme developed by Bootiga.

![Bootiq Homepage](https://raw.githubusercontent.com/Bootiga-SaaS/bootiq/main/screencapture-test24-bootiga-2026-06-12-11_50_18.png)

Bootiq is a modern storefront theme for Drupal Commerce, designed to help merchants build elegant, conversion-focused online stores with minimal configuration.

Originally developed as part of the Bootiga ecosystem, Bootiq combines a clean visual design, Layout Builder flexibility and a streamlined shopping experience.

---

## Features

- Drupal 11 compatible
- Drupal Commerce ready
- Responsive design
- Layout Builder integration
- Product category showcases
- Featured product sections
- Blog integration
- Theme customization tools
- Lightweight and performance-oriented
- SEO-friendly structure

---

## Included Packages

The Bootiq installer currently includes:

- `bootiq` (theme)
- `bootiq_product_blocks`
- `bootiq_logo`
- `bootiq_theme_customizer`
- `bootiq_installer`

Additional storefront layouts and configuration are provided separately to keep the theme portable and easy to maintain.

---

## Installation

### Production install

```bash
composer require bootiga/bootiq:^1.0
drush en bootiq_installer -y
drush bootiq:install
```

The installer will:

- Enable required modules
- Install Bootiq as the default theme
- Import storefront configuration
- Rebuild Drupal caches

---

## Local Development

Until the packages are published, add local path repositories to your Drupal Commerce Kickstart project:

```bash
composer config repositories.bootiq-theme path /home/administrador/build/bootiq-installable/package/web/themes/contrib/bootiq
composer config repositories.bootiq-product-blocks path /home/administrador/build/bootiq-installable/package/web/modules/contrib/bootiq_product_blocks
composer config repositories.bootiq-logo path /home/administrador/build/bootiq-installable/package/web/modules/contrib/bootiq_logo
composer config repositories.bootiq-theme-customizer path /home/administrador/build/bootiq-installable/package/web/modules/contrib/bootiq_theme_customizer
composer config repositories.bootiq-installer path /home/administrador/build/bootiq-installable/package/web/modules/contrib/bootiq_installer
composer config repositories.bootiq path /home/administrador/build/bootiq-installable/package

composer require bootiga/bootiq:^1.0

./vendor/drush/drush/drush en bootiq_installer -y
./vendor/drush/drush/drush bootiq:install
```

---

## Project Structure

```text
bootiq/
├── web/themes/contrib/bootiq
├── web/modules/contrib/bootiq_product_blocks
├── web/modules/contrib/bootiq_logo
├── web/modules/contrib/bootiq_theme_customizer
├── web/modules/contrib/bootiq_installer
└── config-candidates/
```

The `config-candidates` directory is intentionally separated from the theme package. Layout Builder layouts, demo content, catalog views and storefront presets should be installed through a dedicated installer module, recipe or distribution profile rather than being forced by the theme itself.

---

## About Bootiga

Bootiq is maintained by Bootiga.

Bootiga is a Drupal Commerce SaaS platform that enables merchants to launch professional online stores in minutes without managing infrastructure, hosting or updates.

**Website:** https://www.bootiga.com

---

## Why Bootiq?

Unlike generic Drupal themes, Bootiq was built specifically for e-commerce.

It focuses on:

- Conversion-oriented storefront layouts
- Fast deployment
- Drupal Commerce best practices
- Modern shopping experiences
- Seamless integration with the Bootiga ecosystem

---

## Contributing

Issues, bug reports and feature requests are welcome.

If you find a bug or have an idea for improvement, please open an issue.

---

## Status

Bootiq is under active development and continuously improved as part of the Bootiga ecosystem.

Current version: **1.x-dev**

---

## License

GPL-2.0-or-later
