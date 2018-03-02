# Website source and hosting for symposium2017.tsa-stl.org
Source code are in the `master` branch while the rendered contents are hosted in the `gh-pages` branch using Github Pages.

## Development
Requires any relevantly new [Node.js][Node.js] installation and [yarn].

```
yarn install  # One-time setup for all dependencies

npm run build:all  # Build both CSS and JS
npm run watch:all  # Browsersync live-update
npm run dist       # Export hosting-ready files under ./dist
```

## Deployment
Push `dist/` to the git branch `gh-pages`, which can be done by [ghp-import]:

```
ghp-import -p dist
```

[Node.js]: https://nodejs.org/en/
[yarn]: https://yarnpkg.com/
[ghp-import]: https://github.com/davisp/ghp-import
