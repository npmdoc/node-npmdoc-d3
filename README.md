# npmdoc-d3

#### api documentation for  [d3 (v4.8.0)](https://d3js.org)  [![npm package](https://img.shields.io/npm/v/npmdoc-d3.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-d3) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-d3.svg)](https://travis-ci.org/npmdoc/node-npmdoc-d3)

#### Data-Driven Documents

[![NPM](https://nodei.co/npm/d3.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/d3)

- [https://npmdoc.github.io/node-npmdoc-d3/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-d3/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-d3/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-d3/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-d3/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-d3/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mike Bostock",
        "url": "https://bost.ocks.org/mike"
    },
    "browser": "build/d3.js",
    "bugs": {
        "url": "https://github.com/d3/d3/issues"
    },
    "dependencies": {
        "d3-array": "1.2.0",
        "d3-axis": "1.0.6",
        "d3-brush": "1.0.4",
        "d3-chord": "1.0.4",
        "d3-collection": "1.0.3",
        "d3-color": "1.0.3",
        "d3-dispatch": "1.0.3",
        "d3-drag": "1.0.4",
        "d3-dsv": "1.0.5",
        "d3-ease": "1.0.3",
        "d3-force": "1.0.6",
        "d3-format": "1.2.0",
        "d3-geo": "1.6.3",
        "d3-hierarchy": "1.1.4",
        "d3-interpolate": "1.1.4",
        "d3-path": "1.0.5",
        "d3-polygon": "1.0.3",
        "d3-quadtree": "1.0.3",
        "d3-queue": "3.0.5",
        "d3-random": "1.0.3",
        "d3-request": "1.0.5",
        "d3-scale": "1.0.5",
        "d3-selection": "1.0.5",
        "d3-shape": "1.0.6",
        "d3-time": "1.0.6",
        "d3-time-format": "2.0.5",
        "d3-timer": "1.0.5",
        "d3-transition": "1.0.4",
        "d3-voronoi": "1.1.2",
        "d3-zoom": "1.1.4"
    },
    "description": "Data-Driven Documents",
    "devDependencies": {
        "json2module": "0.0",
        "package-preamble": "0.0",
        "rimraf": "2",
        "rollup": "^0.41.4",
        "rollup-plugin-ascii": "0.0",
        "rollup-plugin-node-resolve": "3",
        "tape": "4",
        "uglify-js": "^2.8.11"
    },
    "directories": {},
    "dist": {
        "shasum": "1ad8d18997869c90b6ad6114e9b92425cee78460",
        "tarball": "https://registry.npmjs.org/d3/-/d3-4.8.0.tgz"
    },
    "gitHead": "02d5392d825930b2bd27e87d1d9bc44a639e10f6",
    "homepage": "https://d3js.org",
    "jsnext:main": "index",
    "keywords": [
        "dom",
        "visualization",
        "svg",
        "animation",
        "canvas"
    ],
    "license": "BSD-3-Clause",
    "main": "build/d3.node.js",
    "maintainers": [
        {
            "name": "mbostock"
        },
        {
            "name": "jasondavies"
        }
    ],
    "module": "index",
    "name": "d3",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/d3/d3.git"
    },
    "scripts": {
        "postpublish": "git push && git push --tags && cd ../d3.github.com && git pull && cp ../d3/build/d3.js d3.v4.js && cp ../d3/build/d3.min.js d3.v4.min.js && git add d3.v4.js d3.v4.min.js && git commit -m \"d3 ${npm_package_version}\" && git push && cd - && cd ../d3-bower && git pull && cp ../d3/LICENSE ../d3/README.md ../d3/build/d3.js ../d3/build/d3.min.js . && git add -- LICENSE README.md d3.js d3.min.js && git commit -m \"${npm_package_version}\" && git tag -am \"${npm_package_version}\" v${npm_package_version} && git push && git push --tags && cd - && zip -j build/d3.zip -- LICENSE README.md API.md CHANGES.md build/d3.js build/d3.min.js",
        "prepublish": "npm run test && rollup -c --banner \"$(preamble)\" -f umd -n d3 -o build/d3.js -- index.js && uglifyjs --preamble \"$(preamble)\" build/d3.js -c negate_iife=false -m -o build/d3.min.js",
        "pretest": "rimraf build && mkdir build && json2module package.json > build/package.js && node rollup.node",
        "test": "tape 'test/**/*-test.js'"
    },
    "version": "4.8.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
