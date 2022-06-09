# Ghost workaround theme

This is a slightly modified version of the default Casper theme for [Ghost](http://github.com/tryghost/ghost/). The changes here should serve as a temporary fix for draft previews.

We can go back to using a default Ghost theme once we have a permanent fix in place.

# Development

Casper styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# install dependencies
yarn install

# run development server
yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
# create .zip file
yarn zip
```

# License

Released under the [MIT license](LICENSE).
