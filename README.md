# MultiVendorX Blocks [![Latest Tag](https://img.shields.io/github/v/tag/multivendorx/mvx-blocks.svg?label=Latest%20Tag&sort=semver&style=flat)](https://github.com/multivendorx/mvx-blocks/releases)

[![Made with PHP](https://img.shields.io/badge/Made%20with-PHP-blue.svg?style=for-the-badge)](https://wc-marketplace.com)

Feature plugin for MultiVendorX + Gutenberg to explore new Blocks for MultiVendorX, and how MultiVendorX might work with the block editor.

MVX Blocks basically a package for MultiVendorX with development version.

## Installing the stable version

We soon release a new version of MultiVendorX Blocks onto WordPress.org every few weeks, which can be used as an easier way to preview the features. But you can use this version by as follows -

1. Make sure you have WordPress 5.0+ and MultiVendorX 3.2+

2. Get a copy of this plugin using the green "Clone or download" button on the right and placed it within WordPress setup "plugins" directory.
3. Activate the plugin.

## Installing the development version

1. Get a copy of this plugin using the green "Clone or download" button on the right.

2. `npm install` to install the dependencies.

3. `npm run start` to compile and run the block in development mode.
4. `npm run build` Use to build production code for your block inside `dist` folder.
5. Activate the plugin.

## Installing as MVX package

1. Get a copy of this plugin using the green "Clone or download" button on the right.

2. Place the plugin folder within "MVX plugin" `packages` folder.
3. Load "MVX Block" plugin module in `$packages` variable of `Package.php`

4. Set `add_filter( "mvx_load_package_{$package_dir}", '__return_true' )`. And for "MVX Blocks" `$package_dir` should be `mvx-blocks/wcmp-blocks.php` unless folder renamed.
5. You can also use it as a wordpress plugin.