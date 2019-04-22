# creative-pages

[![Build Status][travis-image]][travis-url]
[![License][license-image]][license-url]
[![Dependency Status][dependency-image]][dependency-url]
[![devDependency Status][devdependency-image]][devdependency-url]
[![Code Style][style-image]][style-url]

> A boilerplate for static pages

## Getting Started

```shell
$ yarn <task> [options]

# e.g.
$ yarn serve --port 5210 --open
$ yarn build --production
```

## All Tasks

### lint

Lint styles & scripts files.

### clean

Clean dist & temp files.

### compile

Compile styles & scripts & pages file.

### serve

Running an automated development server.

#### options

- `port`: Server port, Default: `2080`
- `open`: Automatically open browser, Default: `true`

### build

Build the entire project to get releasable files.

- `production`: Production mode, Default: `false`
- `prod`: Alias to `production`

### start

Running projects in production mode.

#### options

- `port`: Server port, Default: `2080`
- `open`: Automatically open browser, Default: `false`

### deploy

Deploy build results to [GitHub Pages](https://pages.github.com).

#### options

- `branch`: The name of the branch you'll be pushing to, Default: `'gh-pages'`

## Folder Structure

```
└── my-pages ········································· proj root
   ├─ public ········································· static
   │  └─ .gitkeep ···································· static file (unprocessed)
   ├─ src ············································ source
   │  ├─ assets ······································ assets
   │  │  ├─ fonts ···································· fonts
   │  │  │  └─ .gitkeep ······························ font file
   │  │  ├─ images ··································· images
   │  │  │  └─ .gitkeep ······························ image file
   │  │  ├─ scripts ·································· scripts (babel / uglify)
   │  │  │  └─ .gitkeep ······························ script file
   │  │  └─ styles ··································· styles (scss / postcss)
   │  │     ├─ _variables.scss ······················· partial file (dont output)
   │  │     └─ main.scss ····························· entry scss file
   │  ├─ data ········································ data
   │  │  └─ menu.yml ································· data file
   │  ├─ layouts ····································· layouts (dont output)
   │  │  └─ basic.html ······························· layout file
   │  ├─ partials ···································· partials (dont output)
   │  │  ├─ footer.html ······························ partial file
   │  │  └─ header.html ······························ partial file
   │  ├─ about.html ·································· page file (use layout & partials)
   │  └─ index.html ·································· page file (use layout & partials)
   ├─ .csscomb.json ·································· csscomb config file
   ├─ .editorconfig ·································· editor config file
   ├─ .gitignore ····································· git ignore file
   ├─ .travis.yml ···································· travis ci config file
   ├─ CHANGELOG.md ··································· repo changelog
   ├─ LICENSE ········································ repo license
   ├─ README.md ······································ repo readme
   ├─ gulpfile.js ···································· gulp tasks file
   ├─ package.json ··································· package file
   └─ yarn.lock ······································ yarn lock file
```

## Related

- [zce/pages-tasks](https://github.com/zce/pages-tasks) - A preset static pages project gulp tasks.
- [zce/pages-boilerplate](https://github.com/zce/pages-boilerplate) - Always a pleasure scaffolding your awesome static sites.

## Contributing

1. **Fork** it on GitHub!
2. **Clone** the fork to your own machine.
3. **Checkout** your feature branch: `git checkout -b my-awesome-feature`
4. **Commit** your changes to your own branch: `git commit -am 'Add some feature'`
5. **Push** your work back up to your fork: `git push -u origin my-awesome-feature`
6. Submit a **Pull Request** so that we can review your changes.

> **NOTE**: Be sure to merge the latest from "upstream" before making a pull request!

## License

[MIT](LICENSE) &copy; [汪磊](https://zce.me)



[travis-image]: https://travis-ci.org/zce/creative-pages.svg?branch=master
[travis-url]: https://travis-ci.org/zce/creative-pages
[license-image]: https://img.shields.io/github/license/zce/creative-pages.svg
[license-url]: https://github.com/zce/creative-pages/blob/master/LICENSE
[dependency-image]: https://img.shields.io/david/zce/creative-pages.svg
[dependency-url]: https://david-dm.org/zce/creative-pages
[devdependency-image]: https://img.shields.io/david/dev/zce/creative-pages.svg
[devdependency-url]: https://david-dm.org/zce/creative-pages?type=dev
[style-image]: https://img.shields.io/badge/code_style-standard-brightgreen.svg
[style-url]: http://standardjs.com
