# api documentation for  [d3 (v4.7.4)](https://d3js.org)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-d3.svg)](https://travis-ci.org/npmdoc/node-npmdoc-d3)
#### Data-Driven Documents

[![NPM](https://nodei.co/npm/d3.png?downloads=true)](https://www.npmjs.com/package/d3)

[![apidoc](https://npmdoc.github.io/node-npmdoc-d3/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-d3_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-d3/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-d3/build/screen-capture.npmPackageListing.svg)



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
        "d3-array": "1.1.1",
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
        "d3-format": "1.1.1",
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
        "rollup-plugin-node-resolve": "2",
        "tape": "4",
        "uglify-js": "^2.8.11"
    },
    "directories": {},
    "dist": {
        "shasum": "a2f40eb57decc51bc469010d48ae74a20e025772",
        "tarball": "https://registry.npmjs.org/d3/-/d3-4.7.4.tgz"
    },
    "gitHead": "514a18676a6a85d968d20ce0929246220917437a",
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
            "name": "mbostock",
            "email": "mbostock@gmail.com"
        },
        {
            "name": "jasondavies",
            "email": "jason@jasondavies.com"
        }
    ],
    "module": "index",
    "name": "d3",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "4.7.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module d3](#apidoc.module.d3)
1.  [function <span class="apidocSignatureSpan">d3.</span>active (node, name)](#apidoc.element.d3.active)
1.  [function <span class="apidocSignatureSpan">d3.</span>arc ()](#apidoc.element.d3.arc)
1.  [function <span class="apidocSignatureSpan">d3.</span>area ()](#apidoc.element.d3.area)
1.  [function <span class="apidocSignatureSpan">d3.</span>ascending (a, b)](#apidoc.element.d3.ascending)
1.  [function <span class="apidocSignatureSpan">d3.</span>axisBottom (scale)](#apidoc.element.d3.axisBottom)
1.  [function <span class="apidocSignatureSpan">d3.</span>axisLeft (scale)](#apidoc.element.d3.axisLeft)
1.  [function <span class="apidocSignatureSpan">d3.</span>axisRight (scale)](#apidoc.element.d3.axisRight)
1.  [function <span class="apidocSignatureSpan">d3.</span>axisTop (scale)](#apidoc.element.d3.axisTop)
1.  [function <span class="apidocSignatureSpan">d3.</span>bisect (a, x, lo, hi)](#apidoc.element.d3.bisect)
1.  [function <span class="apidocSignatureSpan">d3.</span>bisectLeft (a, x, lo, hi)](#apidoc.element.d3.bisectLeft)
1.  [function <span class="apidocSignatureSpan">d3.</span>bisectRight (a, x, lo, hi)](#apidoc.element.d3.bisectRight)
1.  [function <span class="apidocSignatureSpan">d3.</span>bisector (compare)](#apidoc.element.d3.bisector)
1.  [function <span class="apidocSignatureSpan">d3.</span>brush ()](#apidoc.element.d3.brush)
1.  [function <span class="apidocSignatureSpan">d3.</span>brushSelection (node)](#apidoc.element.d3.brushSelection)
1.  [function <span class="apidocSignatureSpan">d3.</span>brushX ()](#apidoc.element.d3.brushX)
1.  [function <span class="apidocSignatureSpan">d3.</span>brushY ()](#apidoc.element.d3.brushY)
1.  [function <span class="apidocSignatureSpan">d3.</span>chord ()](#apidoc.element.d3.chord)
1.  [function <span class="apidocSignatureSpan">d3.</span>cluster ()](#apidoc.element.d3.cluster)
1.  [function <span class="apidocSignatureSpan">d3.</span>color (format)](#apidoc.element.d3.color)
1.  [function <span class="apidocSignatureSpan">d3.</span>color.prototype.constructor ()](#apidoc.element.d3.color.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>creator (name)](#apidoc.element.d3.creator)
1.  [function <span class="apidocSignatureSpan">d3.</span>cross (a, b, f)](#apidoc.element.d3.cross)
1.  [function <span class="apidocSignatureSpan">d3.</span>csv (url, row, callback)](#apidoc.element.d3.csv)
1.  [function <span class="apidocSignatureSpan">d3.</span>csvFormat (rows, columns)](#apidoc.element.d3.csvFormat)
1.  [function <span class="apidocSignatureSpan">d3.</span>csvFormatRows (rows)](#apidoc.element.d3.csvFormatRows)
1.  [function <span class="apidocSignatureSpan">d3.</span>csvParse (text, f)](#apidoc.element.d3.csvParse)
1.  [function <span class="apidocSignatureSpan">d3.</span>csvParseRows (text, f)](#apidoc.element.d3.csvParseRows)
1.  [function <span class="apidocSignatureSpan">d3.</span>cubehelix (h, s, l, opacity)](#apidoc.element.d3.cubehelix)
1.  [function <span class="apidocSignatureSpan">d3.</span>cubehelix.prototype.constructor (h, s, l, opacity)](#apidoc.element.d3.cubehelix.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveBasis (context)](#apidoc.element.d3.curveBasis)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveBasisClosed (context)](#apidoc.element.d3.curveBasisClosed)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveBasisOpen (context)](#apidoc.element.d3.curveBasisOpen)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveBundle (context)](#apidoc.element.d3.curveBundle)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCardinal (context)](#apidoc.element.d3.curveCardinal)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCardinalClosed (context)](#apidoc.element.d3.curveCardinalClosed)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCardinalOpen (context)](#apidoc.element.d3.curveCardinalOpen)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCatmullRom (context)](#apidoc.element.d3.curveCatmullRom)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCatmullRomClosed (context)](#apidoc.element.d3.curveCatmullRomClosed)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCatmullRomOpen (context)](#apidoc.element.d3.curveCatmullRomOpen)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveLinear (context)](#apidoc.element.d3.curveLinear)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveLinearClosed (context)](#apidoc.element.d3.curveLinearClosed)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveMonotoneX (context)](#apidoc.element.d3.curveMonotoneX)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveMonotoneY (context)](#apidoc.element.d3.curveMonotoneY)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveNatural (context)](#apidoc.element.d3.curveNatural)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveStep (context)](#apidoc.element.d3.curveStep)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveStepAfter (context)](#apidoc.element.d3.curveStepAfter)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveStepBefore (context)](#apidoc.element.d3.curveStepBefore)
1.  [function <span class="apidocSignatureSpan">d3.</span>customEvent (event1, listener, that, args)](#apidoc.element.d3.customEvent)
1.  [function <span class="apidocSignatureSpan">d3.</span>descending (a, b)](#apidoc.element.d3.descending)
1.  [function <span class="apidocSignatureSpan">d3.</span>deviation (array, f)](#apidoc.element.d3.deviation)
1.  [function <span class="apidocSignatureSpan">d3.</span>dispatch ()](#apidoc.element.d3.dispatch)
1.  [function <span class="apidocSignatureSpan">d3.</span>dispatch.prototype.constructor (_)](#apidoc.element.d3.dispatch.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>drag ()](#apidoc.element.d3.drag)
1.  [function <span class="apidocSignatureSpan">d3.</span>dragDisable (view)](#apidoc.element.d3.dragDisable)
1.  [function <span class="apidocSignatureSpan">d3.</span>dragEnable (view, noclick)](#apidoc.element.d3.dragEnable)
1.  [function <span class="apidocSignatureSpan">d3.</span>dsvFormat (delimiter)](#apidoc.element.d3.dsvFormat)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBack (t)](#apidoc.element.d3.easeBack)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBackIn (t)](#apidoc.element.d3.easeBackIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBackInOut (t)](#apidoc.element.d3.easeBackInOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBackOut (t)](#apidoc.element.d3.easeBackOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBounce (t)](#apidoc.element.d3.easeBounce)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBounceIn (t)](#apidoc.element.d3.easeBounceIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBounceInOut (t)](#apidoc.element.d3.easeBounceInOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBounceOut (t)](#apidoc.element.d3.easeBounceOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeCircle (t)](#apidoc.element.d3.easeCircle)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeCircleIn (t)](#apidoc.element.d3.easeCircleIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeCircleInOut (t)](#apidoc.element.d3.easeCircleInOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeCircleOut (t)](#apidoc.element.d3.easeCircleOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeCubic (t)](#apidoc.element.d3.easeCubic)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeCubicIn (t)](#apidoc.element.d3.easeCubicIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeCubicInOut (t)](#apidoc.element.d3.easeCubicInOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeCubicOut (t)](#apidoc.element.d3.easeCubicOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeElastic (t)](#apidoc.element.d3.easeElastic)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeElasticIn (t)](#apidoc.element.d3.easeElasticIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeElasticInOut (t)](#apidoc.element.d3.easeElasticInOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeElasticOut (t)](#apidoc.element.d3.easeElasticOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeExp (t)](#apidoc.element.d3.easeExp)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeExpIn (t)](#apidoc.element.d3.easeExpIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeExpInOut (t)](#apidoc.element.d3.easeExpInOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeExpOut (t)](#apidoc.element.d3.easeExpOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeLinear (t)](#apidoc.element.d3.easeLinear)
1.  [function <span class="apidocSignatureSpan">d3.</span>easePoly (t)](#apidoc.element.d3.easePoly)
1.  [function <span class="apidocSignatureSpan">d3.</span>easePolyIn (t)](#apidoc.element.d3.easePolyIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easePolyInOut (t)](#apidoc.element.d3.easePolyInOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easePolyOut (t)](#apidoc.element.d3.easePolyOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeQuad (t)](#apidoc.element.d3.easeQuad)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeQuadIn (t)](#apidoc.element.d3.easeQuadIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeQuadInOut (t)](#apidoc.element.d3.easeQuadInOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeQuadOut (t)](#apidoc.element.d3.easeQuadOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeSin (t)](#apidoc.element.d3.easeSin)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeSinIn (t)](#apidoc.element.d3.easeSinIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeSinInOut (t)](#apidoc.element.d3.easeSinInOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeSinOut (t)](#apidoc.element.d3.easeSinOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>entries (map)](#apidoc.element.d3.entries)
1.  [function <span class="apidocSignatureSpan">d3.</span>extent (array, f)](#apidoc.element.d3.extent)
1.  [function <span class="apidocSignatureSpan">d3.</span>forceCenter (x, y)](#apidoc.element.d3.forceCenter)
1.  [function <span class="apidocSignatureSpan">d3.</span>forceCollide (radius)](#apidoc.element.d3.forceCollide)
1.  [function <span class="apidocSignatureSpan">d3.</span>forceLink (links)](#apidoc.element.d3.forceLink)
1.  [function <span class="apidocSignatureSpan">d3.</span>forceManyBody ()](#apidoc.element.d3.forceManyBody)
1.  [function <span class="apidocSignatureSpan">d3.</span>forceSimulation (nodes)](#apidoc.element.d3.forceSimulation)
1.  [function <span class="apidocSignatureSpan">d3.</span>forceX (x)](#apidoc.element.d3.forceX)
1.  [function <span class="apidocSignatureSpan">d3.</span>forceY (y)](#apidoc.element.d3.forceY)
1.  [function <span class="apidocSignatureSpan">d3.</span>format (specifier)](#apidoc.element.d3.format)
1.  [function <span class="apidocSignatureSpan">d3.</span>formatDefaultLocale (definition)](#apidoc.element.d3.formatDefaultLocale)
1.  [function <span class="apidocSignatureSpan">d3.</span>formatLocale (locale)](#apidoc.element.d3.formatLocale)
1.  [function <span class="apidocSignatureSpan">d3.</span>formatPrefix (specifier, value)](#apidoc.element.d3.formatPrefix)
1.  [function <span class="apidocSignatureSpan">d3.</span>formatSpecifier (specifier)](#apidoc.element.d3.formatSpecifier)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoAlbers ()](#apidoc.element.d3.geoAlbers)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoAlbersUsa ()](#apidoc.element.d3.geoAlbersUsa)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoArea (object)](#apidoc.element.d3.geoArea)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEqualArea ()](#apidoc.element.d3.geoAzimuthalEqualArea)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEqualAreaRaw (x, y)](#apidoc.element.d3.geoAzimuthalEqualAreaRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEquidistant ()](#apidoc.element.d3.geoAzimuthalEquidistant)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEquidistantRaw (x, y)](#apidoc.element.d3.geoAzimuthalEquidistantRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoBounds (feature)](#apidoc.element.d3.geoBounds)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoCentroid (object)](#apidoc.element.d3.geoCentroid)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoCircle ()](#apidoc.element.d3.geoCircle)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoClipExtent ()](#apidoc.element.d3.geoClipExtent)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoConicConformal ()](#apidoc.element.d3.geoConicConformal)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoConicConformalRaw (y0, y1)](#apidoc.element.d3.geoConicConformalRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoConicEqualArea ()](#apidoc.element.d3.geoConicEqualArea)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoConicEqualAreaRaw (y0, y1)](#apidoc.element.d3.geoConicEqualAreaRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoConicEquidistant ()](#apidoc.element.d3.geoConicEquidistant)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoConicEquidistantRaw (y0, y1)](#apidoc.element.d3.geoConicEquidistantRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoContains (object, point)](#apidoc.element.d3.geoContains)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoDistance (a, b)](#apidoc.element.d3.geoDistance)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoEquirectangular ()](#apidoc.element.d3.geoEquirectangular)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoEquirectangularRaw (lambda, phi)](#apidoc.element.d3.geoEquirectangularRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoGnomonic ()](#apidoc.element.d3.geoGnomonic)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoGnomonicRaw (x, y)](#apidoc.element.d3.geoGnomonicRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoGraticule ()](#apidoc.element.d3.geoGraticule)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoGraticule10 ()](#apidoc.element.d3.geoGraticule10)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoIdentity ()](#apidoc.element.d3.geoIdentity)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoInterpolate (a, b)](#apidoc.element.d3.geoInterpolate)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoLength (object)](#apidoc.element.d3.geoLength)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoMercator ()](#apidoc.element.d3.geoMercator)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoMercatorRaw (lambda, phi)](#apidoc.element.d3.geoMercatorRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoOrthographic ()](#apidoc.element.d3.geoOrthographic)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoOrthographicRaw (x, y)](#apidoc.element.d3.geoOrthographicRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoPath (projection, context)](#apidoc.element.d3.geoPath)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoProjection (project)](#apidoc.element.d3.geoProjection)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoProjectionMutator (projectAt)](#apidoc.element.d3.geoProjectionMutator)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoRotation (rotate)](#apidoc.element.d3.geoRotation)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoStereographic ()](#apidoc.element.d3.geoStereographic)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoStereographicRaw (x, y)](#apidoc.element.d3.geoStereographicRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoStream (object, stream)](#apidoc.element.d3.geoStream)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoTransform (methods)](#apidoc.element.d3.geoTransform)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoTransverseMercator ()](#apidoc.element.d3.geoTransverseMercator)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoTransverseMercatorRaw (lambda, phi)](#apidoc.element.d3.geoTransverseMercatorRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>hcl (h, c, l, opacity)](#apidoc.element.d3.hcl)
1.  [function <span class="apidocSignatureSpan">d3.</span>hcl.prototype.constructor (h, c, l, opacity)](#apidoc.element.d3.hcl.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>hierarchy (data, children)](#apidoc.element.d3.hierarchy)
1.  [function <span class="apidocSignatureSpan">d3.</span>hierarchy.prototype.constructor (data)](#apidoc.element.d3.hierarchy.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>histogram ()](#apidoc.element.d3.histogram)
1.  [function <span class="apidocSignatureSpan">d3.</span>hsl (h, s, l, opacity)](#apidoc.element.d3.hsl)
1.  [function <span class="apidocSignatureSpan">d3.</span>hsl.prototype.constructor (h, s, l, opacity)](#apidoc.element.d3.hsl.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>html (url, callback)](#apidoc.element.d3.html)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolate (a, b)](#apidoc.element.d3.interpolate)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateArray (a, b)](#apidoc.element.d3.interpolateArray)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateBasis (values)](#apidoc.element.d3.interpolateBasis)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateBasisClosed (values)](#apidoc.element.d3.interpolateBasisClosed)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateCool (t)](#apidoc.element.d3.interpolateCool)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateCubehelix (start, end)](#apidoc.element.d3.interpolateCubehelix)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateCubehelixDefault (t)](#apidoc.element.d3.interpolateCubehelixDefault)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateCubehelixLong (start, end)](#apidoc.element.d3.interpolateCubehelixLong)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateDate (a, b)](#apidoc.element.d3.interpolateDate)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateHcl (start, end)](#apidoc.element.d3.interpolateHcl)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateHclLong (start, end)](#apidoc.element.d3.interpolateHclLong)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateHsl (start, end)](#apidoc.element.d3.interpolateHsl)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateHslLong (start, end)](#apidoc.element.d3.interpolateHslLong)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateInferno (t)](#apidoc.element.d3.interpolateInferno)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateLab (start, end)](#apidoc.element.d3.interpolateLab)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateMagma (t)](#apidoc.element.d3.interpolateMagma)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateNumber (a, b)](#apidoc.element.d3.interpolateNumber)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateObject (a, b)](#apidoc.element.d3.interpolateObject)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolatePlasma (t)](#apidoc.element.d3.interpolatePlasma)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateRainbow (t)](#apidoc.element.d3.interpolateRainbow)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateRgb (start, end)](#apidoc.element.d3.interpolateRgb)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateRgbBasis (colors)](#apidoc.element.d3.interpolateRgbBasis)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateRgbBasisClosed (colors)](#apidoc.element.d3.interpolateRgbBasisClosed)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateRound (a, b)](#apidoc.element.d3.interpolateRound)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateString (a, b)](#apidoc.element.d3.interpolateString)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateTransformCss (a, b)](#apidoc.element.d3.interpolateTransformCss)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateTransformSvg (a, b)](#apidoc.element.d3.interpolateTransformSvg)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateViridis (t)](#apidoc.element.d3.interpolateViridis)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateWarm (t)](#apidoc.element.d3.interpolateWarm)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateZoom (p0, p1)](#apidoc.element.d3.interpolateZoom)
1.  [function <span class="apidocSignatureSpan">d3.</span>interrupt (node, name)](#apidoc.element.d3.interrupt)
1.  [function <span class="apidocSignatureSpan">d3.</span>interval (callback, delay, time)](#apidoc.element.d3.interval)
1.  [function <span class="apidocSignatureSpan">d3.</span>isoFormat (date)](#apidoc.element.d3.isoFormat)
1.  [function <span class="apidocSignatureSpan">d3.</span>isoParse (string)](#apidoc.element.d3.isoParse)
1.  [function <span class="apidocSignatureSpan">d3.</span>json (url, callback)](#apidoc.element.d3.json)
1.  [function <span class="apidocSignatureSpan">d3.</span>keys (map)](#apidoc.element.d3.keys)
1.  [function <span class="apidocSignatureSpan">d3.</span>lab (l, a, b, opacity)](#apidoc.element.d3.lab)
1.  [function <span class="apidocSignatureSpan">d3.</span>lab.prototype.constructor (l, a, b, opacity)](#apidoc.element.d3.lab.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>line ()](#apidoc.element.d3.line)
1.  [function <span class="apidocSignatureSpan">d3.</span>local ()](#apidoc.element.d3.local)
1.  [function <span class="apidocSignatureSpan">d3.</span>local.prototype.constructor ()](#apidoc.element.d3.local.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>map (object, f)](#apidoc.element.d3.map)
1.  [function <span class="apidocSignatureSpan">d3.</span>map.prototype.constructor ()](#apidoc.element.d3.map.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>matcher (selector)](#apidoc.element.d3.matcher)
1.  [function <span class="apidocSignatureSpan">d3.</span>max (array, f)](#apidoc.element.d3.max)
1.  [function <span class="apidocSignatureSpan">d3.</span>mean (array, f)](#apidoc.element.d3.mean)
1.  [function <span class="apidocSignatureSpan">d3.</span>median (array, f)](#apidoc.element.d3.median)
1.  [function <span class="apidocSignatureSpan">d3.</span>merge (arrays)](#apidoc.element.d3.merge)
1.  [function <span class="apidocSignatureSpan">d3.</span>min (array, f)](#apidoc.element.d3.min)
1.  [function <span class="apidocSignatureSpan">d3.</span>mouse (node)](#apidoc.element.d3.mouse)
1.  [function <span class="apidocSignatureSpan">d3.</span>namespace (name)](#apidoc.element.d3.namespace)
1.  [function <span class="apidocSignatureSpan">d3.</span>nest ()](#apidoc.element.d3.nest)
1.  [function <span class="apidocSignatureSpan">d3.</span>now ()](#apidoc.element.d3.now)
1.  [function <span class="apidocSignatureSpan">d3.</span>pack ()](#apidoc.element.d3.pack)
1.  [function <span class="apidocSignatureSpan">d3.</span>packEnclose (circles)](#apidoc.element.d3.packEnclose)
1.  [function <span class="apidocSignatureSpan">d3.</span>packSiblings (circles)](#apidoc.element.d3.packSiblings)
1.  [function <span class="apidocSignatureSpan">d3.</span>pairs (array, f)](#apidoc.element.d3.pairs)
1.  [function <span class="apidocSignatureSpan">d3.</span>partition ()](#apidoc.element.d3.partition)
1.  [function <span class="apidocSignatureSpan">d3.</span>path ()](#apidoc.element.d3.path)
1.  [function <span class="apidocSignatureSpan">d3.</span>path.prototype.constructor ()](#apidoc.element.d3.path.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>permute (array, indexes)](#apidoc.element.d3.permute)
1.  [function <span class="apidocSignatureSpan">d3.</span>pie ()](#apidoc.element.d3.pie)
1.  [function <span class="apidocSignatureSpan">d3.</span>polygonArea (polygon)](#apidoc.element.d3.polygonArea)
1.  [function <span class="apidocSignatureSpan">d3.</span>polygonCentroid (polygon)](#apidoc.element.d3.polygonCentroid)
1.  [function <span class="apidocSignatureSpan">d3.</span>polygonContains (polygon, point)](#apidoc.element.d3.polygonContains)
1.  [function <span class="apidocSignatureSpan">d3.</span>polygonHull (points)](#apidoc.element.d3.polygonHull)
1.  [function <span class="apidocSignatureSpan">d3.</span>polygonLength (polygon)](#apidoc.element.d3.polygonLength)
1.  [function <span class="apidocSignatureSpan">d3.</span>precisionFixed (step)](#apidoc.element.d3.precisionFixed)
1.  [function <span class="apidocSignatureSpan">d3.</span>precisionPrefix (step, value)](#apidoc.element.d3.precisionPrefix)
1.  [function <span class="apidocSignatureSpan">d3.</span>precisionRound (step, max)](#apidoc.element.d3.precisionRound)
1.  [function <span class="apidocSignatureSpan">d3.</span>quadtree (nodes, x, y)](#apidoc.element.d3.quadtree)
1.  [function <span class="apidocSignatureSpan">d3.</span>quantile (array, p, f)](#apidoc.element.d3.quantile)
1.  [function <span class="apidocSignatureSpan">d3.</span>quantize (interpolator, n)](#apidoc.element.d3.quantize)
1.  [function <span class="apidocSignatureSpan">d3.</span>queue (concurrency)](#apidoc.element.d3.queue)
1.  [function <span class="apidocSignatureSpan">d3.</span>queue.prototype.constructor (size)](#apidoc.element.d3.queue.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>radialArea ()](#apidoc.element.d3.radialArea)
1.  [function <span class="apidocSignatureSpan">d3.</span>radialLine ()](#apidoc.element.d3.radialLine)
1.  [function <span class="apidocSignatureSpan">d3.</span>randomBates (n)](#apidoc.element.d3.randomBates)
1.  [function <span class="apidocSignatureSpan">d3.</span>randomExponential (lambda)](#apidoc.element.d3.randomExponential)
1.  [function <span class="apidocSignatureSpan">d3.</span>randomIrwinHall (n)](#apidoc.element.d3.randomIrwinHall)
1.  [function <span class="apidocSignatureSpan">d3.</span>randomLogNormal ()](#apidoc.element.d3.randomLogNormal)
1.  [function <span class="apidocSignatureSpan">d3.</span>randomNormal (mu, sigma)](#apidoc.element.d3.randomNormal)
1.  [function <span class="apidocSignatureSpan">d3.</span>randomUniform (min, max)](#apidoc.element.d3.randomUniform)
1.  [function <span class="apidocSignatureSpan">d3.</span>range (start, stop, step)](#apidoc.element.d3.range)
1.  [function <span class="apidocSignatureSpan">d3.</span>request (url, callback)](#apidoc.element.d3.request)
1.  [function <span class="apidocSignatureSpan">d3.</span>rgb (r, g, b, opacity)](#apidoc.element.d3.rgb)
1.  [function <span class="apidocSignatureSpan">d3.</span>rgb.prototype.constructor (r, g, b, opacity)](#apidoc.element.d3.rgb.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>ribbon ()](#apidoc.element.d3.ribbon)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleBand ()](#apidoc.element.d3.scaleBand)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleIdentity ()](#apidoc.element.d3.scaleIdentity)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleLinear ()](#apidoc.element.d3.scaleLinear)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleLog ()](#apidoc.element.d3.scaleLog)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleOrdinal (range$$1)](#apidoc.element.d3.scaleOrdinal)
1.  [function <span class="apidocSignatureSpan">d3.</span>scalePoint ()](#apidoc.element.d3.scalePoint)
1.  [function <span class="apidocSignatureSpan">d3.</span>scalePow ()](#apidoc.element.d3.scalePow)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleQuantile ()](#apidoc.element.d3.scaleQuantile)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleQuantize ()](#apidoc.element.d3.scaleQuantize)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleSequential (interpolator)](#apidoc.element.d3.scaleSequential)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleSqrt ()](#apidoc.element.d3.scaleSqrt)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleThreshold ()](#apidoc.element.d3.scaleThreshold)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleTime ()](#apidoc.element.d3.scaleTime)
1.  [function <span class="apidocSignatureSpan">d3.</span>scaleUtc ()](#apidoc.element.d3.scaleUtc)
1.  [function <span class="apidocSignatureSpan">d3.</span>scan (array, compare)](#apidoc.element.d3.scan)
1.  [function <span class="apidocSignatureSpan">d3.</span>select (selector)](#apidoc.element.d3.select)
1.  [function <span class="apidocSignatureSpan">d3.</span>selectAll (selector)](#apidoc.element.d3.selectAll)
1.  [function <span class="apidocSignatureSpan">d3.</span>selection ()](#apidoc.element.d3.selection)
1.  [function <span class="apidocSignatureSpan">d3.</span>selection.prototype.constructor (groups, parents)](#apidoc.element.d3.selection.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>selector (selector)](#apidoc.element.d3.selector)
1.  [function <span class="apidocSignatureSpan">d3.</span>selectorAll (selector)](#apidoc.element.d3.selectorAll)
1.  [function <span class="apidocSignatureSpan">d3.</span>set (object, f)](#apidoc.element.d3.set)
1.  [function <span class="apidocSignatureSpan">d3.</span>set.prototype.constructor ()](#apidoc.element.d3.set.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>shuffle (array, i0, i1)](#apidoc.element.d3.shuffle)
1.  [function <span class="apidocSignatureSpan">d3.</span>stack ()](#apidoc.element.d3.stack)
1.  [function <span class="apidocSignatureSpan">d3.</span>stackOffsetExpand (series, order)](#apidoc.element.d3.stackOffsetExpand)
1.  [function <span class="apidocSignatureSpan">d3.</span>stackOffsetNone (series, order)](#apidoc.element.d3.stackOffsetNone)
1.  [function <span class="apidocSignatureSpan">d3.</span>stackOffsetSilhouette (series, order)](#apidoc.element.d3.stackOffsetSilhouette)
1.  [function <span class="apidocSignatureSpan">d3.</span>stackOffsetWiggle (series, order)](#apidoc.element.d3.stackOffsetWiggle)
1.  [function <span class="apidocSignatureSpan">d3.</span>stackOrderAscending (series)](#apidoc.element.d3.stackOrderAscending)
1.  [function <span class="apidocSignatureSpan">d3.</span>stackOrderDescending (series)](#apidoc.element.d3.stackOrderDescending)
1.  [function <span class="apidocSignatureSpan">d3.</span>stackOrderInsideOut (series)](#apidoc.element.d3.stackOrderInsideOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>stackOrderNone (series)](#apidoc.element.d3.stackOrderNone)
1.  [function <span class="apidocSignatureSpan">d3.</span>stackOrderReverse (series)](#apidoc.element.d3.stackOrderReverse)
1.  [function <span class="apidocSignatureSpan">d3.</span>stratify ()](#apidoc.element.d3.stratify)
1.  [function <span class="apidocSignatureSpan">d3.</span>sum (array, f)](#apidoc.element.d3.sum)
1.  [function <span class="apidocSignatureSpan">d3.</span>symbol ()](#apidoc.element.d3.symbol)
1.  [function <span class="apidocSignatureSpan">d3.</span>text (url, callback)](#apidoc.element.d3.text)
1.  [function <span class="apidocSignatureSpan">d3.</span>thresholdFreedmanDiaconis (values, min, max)](#apidoc.element.d3.thresholdFreedmanDiaconis)
1.  [function <span class="apidocSignatureSpan">d3.</span>thresholdScott (values, min, max)](#apidoc.element.d3.thresholdScott)
1.  [function <span class="apidocSignatureSpan">d3.</span>thresholdSturges (values)](#apidoc.element.d3.thresholdSturges)
1.  [function <span class="apidocSignatureSpan">d3.</span>tickStep (start, stop, count)](#apidoc.element.d3.tickStep)
1.  [function <span class="apidocSignatureSpan">d3.</span>ticks (start, stop, count)](#apidoc.element.d3.ticks)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeDay (date)](#apidoc.element.d3.timeDay)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeDays (start, stop, step)](#apidoc.element.d3.timeDays)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeFormat (specifier)](#apidoc.element.d3.timeFormat)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeFormatDefaultLocale (definition)](#apidoc.element.d3.timeFormatDefaultLocale)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeFormatLocale (locale)](#apidoc.element.d3.timeFormatLocale)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeFriday (date)](#apidoc.element.d3.timeFriday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeFridays (start, stop, step)](#apidoc.element.d3.timeFridays)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeHour (date)](#apidoc.element.d3.timeHour)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeHours (start, stop, step)](#apidoc.element.d3.timeHours)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeInterval (floori, offseti, count, field)](#apidoc.element.d3.timeInterval)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMillisecond (date)](#apidoc.element.d3.timeMillisecond)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMilliseconds (start, stop, step)](#apidoc.element.d3.timeMilliseconds)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMinute (date)](#apidoc.element.d3.timeMinute)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMinutes (start, stop, step)](#apidoc.element.d3.timeMinutes)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMonday (date)](#apidoc.element.d3.timeMonday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMondays (start, stop, step)](#apidoc.element.d3.timeMondays)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMonth (date)](#apidoc.element.d3.timeMonth)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMonths (start, stop, step)](#apidoc.element.d3.timeMonths)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeParse (specifier)](#apidoc.element.d3.timeParse)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeSaturday (date)](#apidoc.element.d3.timeSaturday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeSaturdays (start, stop, step)](#apidoc.element.d3.timeSaturdays)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeSecond (date)](#apidoc.element.d3.timeSecond)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeSeconds (start, stop, step)](#apidoc.element.d3.timeSeconds)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeSunday (date)](#apidoc.element.d3.timeSunday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeSundays (start, stop, step)](#apidoc.element.d3.timeSundays)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeThursday (date)](#apidoc.element.d3.timeThursday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeThursdays (start, stop, step)](#apidoc.element.d3.timeThursdays)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeTuesday (date)](#apidoc.element.d3.timeTuesday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeTuesdays (start, stop, step)](#apidoc.element.d3.timeTuesdays)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeWednesday (date)](#apidoc.element.d3.timeWednesday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeWednesdays (start, stop, step)](#apidoc.element.d3.timeWednesdays)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeWeek (date)](#apidoc.element.d3.timeWeek)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeWeeks (start, stop, step)](#apidoc.element.d3.timeWeeks)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeYear (date)](#apidoc.element.d3.timeYear)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeYears (start, stop, step)](#apidoc.element.d3.timeYears)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeout (callback, delay, time)](#apidoc.element.d3.timeout)
1.  [function <span class="apidocSignatureSpan">d3.</span>timer (callback, delay, time)](#apidoc.element.d3.timer)
1.  [function <span class="apidocSignatureSpan">d3.</span>timer.prototype.constructor ()](#apidoc.element.d3.timer.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>timerFlush ()](#apidoc.element.d3.timerFlush)
1.  [function <span class="apidocSignatureSpan">d3.</span>touch (node, touches, identifier)](#apidoc.element.d3.touch)
1.  [function <span class="apidocSignatureSpan">d3.</span>touches (node, touches)](#apidoc.element.d3.touches)
1.  [function <span class="apidocSignatureSpan">d3.</span>transition (name)](#apidoc.element.d3.transition)
1.  [function <span class="apidocSignatureSpan">d3.</span>transition.prototype.constructor (groups, parents, name, id)](#apidoc.element.d3.transition.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.</span>transpose (matrix)](#apidoc.element.d3.transpose)
1.  [function <span class="apidocSignatureSpan">d3.</span>tree ()](#apidoc.element.d3.tree)
1.  [function <span class="apidocSignatureSpan">d3.</span>treemap ()](#apidoc.element.d3.treemap)
1.  [function <span class="apidocSignatureSpan">d3.</span>treemapBinary (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapBinary)
1.  [function <span class="apidocSignatureSpan">d3.</span>treemapDice (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapDice)
1.  [function <span class="apidocSignatureSpan">d3.</span>treemapResquarify (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapResquarify)
1.  [function <span class="apidocSignatureSpan">d3.</span>treemapSlice (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapSlice)
1.  [function <span class="apidocSignatureSpan">d3.</span>treemapSliceDice (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapSliceDice)
1.  [function <span class="apidocSignatureSpan">d3.</span>treemapSquarify (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapSquarify)
1.  [function <span class="apidocSignatureSpan">d3.</span>tsv (url, row, callback)](#apidoc.element.d3.tsv)
1.  [function <span class="apidocSignatureSpan">d3.</span>tsvFormat (rows, columns)](#apidoc.element.d3.tsvFormat)
1.  [function <span class="apidocSignatureSpan">d3.</span>tsvFormatRows (rows)](#apidoc.element.d3.tsvFormatRows)
1.  [function <span class="apidocSignatureSpan">d3.</span>tsvParse (text, f)](#apidoc.element.d3.tsvParse)
1.  [function <span class="apidocSignatureSpan">d3.</span>tsvParseRows (text, f)](#apidoc.element.d3.tsvParseRows)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcDay (date)](#apidoc.element.d3.utcDay)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcDays (start, stop, step)](#apidoc.element.d3.utcDays)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcFormat (specifier)](#apidoc.element.d3.utcFormat)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcFriday (date)](#apidoc.element.d3.utcFriday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcFridays (start, stop, step)](#apidoc.element.d3.utcFridays)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcHour (date)](#apidoc.element.d3.utcHour)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcHours (start, stop, step)](#apidoc.element.d3.utcHours)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMillisecond (date)](#apidoc.element.d3.utcMillisecond)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMilliseconds (start, stop, step)](#apidoc.element.d3.utcMilliseconds)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMinute (date)](#apidoc.element.d3.utcMinute)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMinutes (start, stop, step)](#apidoc.element.d3.utcMinutes)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMonday (date)](#apidoc.element.d3.utcMonday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMondays (start, stop, step)](#apidoc.element.d3.utcMondays)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMonth (date)](#apidoc.element.d3.utcMonth)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMonths (start, stop, step)](#apidoc.element.d3.utcMonths)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcParse (specifier)](#apidoc.element.d3.utcParse)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcSaturday (date)](#apidoc.element.d3.utcSaturday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcSaturdays (start, stop, step)](#apidoc.element.d3.utcSaturdays)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcSecond (date)](#apidoc.element.d3.utcSecond)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcSeconds (start, stop, step)](#apidoc.element.d3.utcSeconds)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcSunday (date)](#apidoc.element.d3.utcSunday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcSundays (start, stop, step)](#apidoc.element.d3.utcSundays)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcThursday (date)](#apidoc.element.d3.utcThursday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcThursdays (start, stop, step)](#apidoc.element.d3.utcThursdays)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcTuesday (date)](#apidoc.element.d3.utcTuesday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcTuesdays (start, stop, step)](#apidoc.element.d3.utcTuesdays)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcWednesday (date)](#apidoc.element.d3.utcWednesday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcWednesdays (start, stop, step)](#apidoc.element.d3.utcWednesdays)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcWeek (date)](#apidoc.element.d3.utcWeek)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcWeeks (start, stop, step)](#apidoc.element.d3.utcWeeks)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcYear (date)](#apidoc.element.d3.utcYear)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcYears (start, stop, step)](#apidoc.element.d3.utcYears)
1.  [function <span class="apidocSignatureSpan">d3.</span>values (map)](#apidoc.element.d3.values)
1.  [function <span class="apidocSignatureSpan">d3.</span>variance (array, f)](#apidoc.element.d3.variance)
1.  [function <span class="apidocSignatureSpan">d3.</span>voronoi ()](#apidoc.element.d3.voronoi)
1.  [function <span class="apidocSignatureSpan">d3.</span>window (node)](#apidoc.element.d3.window)
1.  [function <span class="apidocSignatureSpan">d3.</span>xml (url, callback)](#apidoc.element.d3.xml)
1.  [function <span class="apidocSignatureSpan">d3.</span>zip ()](#apidoc.element.d3.zip)
1.  [function <span class="apidocSignatureSpan">d3.</span>zoom ()](#apidoc.element.d3.zoom)
1.  [function <span class="apidocSignatureSpan">d3.</span>zoomTransform (node)](#apidoc.element.d3.zoomTransform)
1.  [function <span class="apidocSignatureSpan">d3.</span>zoomTransform.prototype.constructor (k, x, y)](#apidoc.element.d3.zoomTransform.prototype.constructor)
1.  object <span class="apidocSignatureSpan">d3.</span>color.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>cubehelix.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>dispatch.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>event
1.  object <span class="apidocSignatureSpan">d3.</span>formatSpecifier.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>hcl.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>hierarchy.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>hsl.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>lab.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>local.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>map.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>namespaces
1.  object <span class="apidocSignatureSpan">d3.</span>path.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>quadtree.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>queue.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>rgb.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>scaleImplicit
1.  object <span class="apidocSignatureSpan">d3.</span>schemeCategory10
1.  object <span class="apidocSignatureSpan">d3.</span>schemeCategory20
1.  object <span class="apidocSignatureSpan">d3.</span>schemeCategory20b
1.  object <span class="apidocSignatureSpan">d3.</span>schemeCategory20c
1.  object <span class="apidocSignatureSpan">d3.</span>selection.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>set.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>symbolCircle
1.  object <span class="apidocSignatureSpan">d3.</span>symbolCross
1.  object <span class="apidocSignatureSpan">d3.</span>symbolDiamond
1.  object <span class="apidocSignatureSpan">d3.</span>symbolSquare
1.  object <span class="apidocSignatureSpan">d3.</span>symbolStar
1.  object <span class="apidocSignatureSpan">d3.</span>symbolTriangle
1.  object <span class="apidocSignatureSpan">d3.</span>symbolWye
1.  object <span class="apidocSignatureSpan">d3.</span>symbols
1.  object <span class="apidocSignatureSpan">d3.</span>timer.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>transition.prototype
1.  object <span class="apidocSignatureSpan">d3.</span>zoomIdentity
1.  object <span class="apidocSignatureSpan">d3.</span>zoomTransform.prototype
1.  string <span class="apidocSignatureSpan">d3.</span>version

#### [module d3.color](#apidoc.module.d3.color)
1.  [function <span class="apidocSignatureSpan">d3.</span>color (format)](#apidoc.element.d3.color.color)

#### [module d3.color.prototype](#apidoc.module.d3.color.prototype)
1.  [function <span class="apidocSignatureSpan">d3.color.prototype.</span>constructor ()](#apidoc.element.d3.color.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.color.prototype.</span>displayable ()](#apidoc.element.d3.color.prototype.displayable)
1.  [function <span class="apidocSignatureSpan">d3.color.prototype.</span>toString ()](#apidoc.element.d3.color.prototype.toString)

#### [module d3.color.prototype.constructor](#apidoc.module.d3.color.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.color.prototype.</span>constructor ()](#apidoc.element.d3.color.prototype.constructor.constructor)

#### [module d3.cubehelix](#apidoc.module.d3.cubehelix)
1.  [function <span class="apidocSignatureSpan">d3.</span>cubehelix (h, s, l, opacity)](#apidoc.element.d3.cubehelix.cubehelix)

#### [module d3.cubehelix.prototype](#apidoc.module.d3.cubehelix.prototype)
1.  [function <span class="apidocSignatureSpan">d3.cubehelix.prototype.</span>brighter (k)](#apidoc.element.d3.cubehelix.prototype.brighter)
1.  [function <span class="apidocSignatureSpan">d3.cubehelix.prototype.</span>constructor (h, s, l, opacity)](#apidoc.element.d3.cubehelix.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.cubehelix.prototype.</span>darker (k)](#apidoc.element.d3.cubehelix.prototype.darker)
1.  [function <span class="apidocSignatureSpan">d3.cubehelix.prototype.</span>rgb ()](#apidoc.element.d3.cubehelix.prototype.rgb)

#### [module d3.cubehelix.prototype.constructor](#apidoc.module.d3.cubehelix.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.cubehelix.prototype.</span>constructor ()](#apidoc.element.d3.cubehelix.prototype.constructor.constructor)

#### [module d3.curveBundle](#apidoc.module.d3.curveBundle)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveBundle (context)](#apidoc.element.d3.curveBundle.curveBundle)
1.  [function <span class="apidocSignatureSpan">d3.curveBundle.</span>beta (beta)](#apidoc.element.d3.curveBundle.beta)

#### [module d3.curveCardinal](#apidoc.module.d3.curveCardinal)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCardinal (context)](#apidoc.element.d3.curveCardinal.curveCardinal)
1.  [function <span class="apidocSignatureSpan">d3.curveCardinal.</span>tension (tension)](#apidoc.element.d3.curveCardinal.tension)

#### [module d3.curveCardinalClosed](#apidoc.module.d3.curveCardinalClosed)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCardinalClosed (context)](#apidoc.element.d3.curveCardinalClosed.curveCardinalClosed)
1.  [function <span class="apidocSignatureSpan">d3.curveCardinalClosed.</span>tension (tension)](#apidoc.element.d3.curveCardinalClosed.tension)

#### [module d3.curveCardinalOpen](#apidoc.module.d3.curveCardinalOpen)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCardinalOpen (context)](#apidoc.element.d3.curveCardinalOpen.curveCardinalOpen)
1.  [function <span class="apidocSignatureSpan">d3.curveCardinalOpen.</span>tension (tension)](#apidoc.element.d3.curveCardinalOpen.tension)

#### [module d3.curveCatmullRom](#apidoc.module.d3.curveCatmullRom)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCatmullRom (context)](#apidoc.element.d3.curveCatmullRom.curveCatmullRom)
1.  [function <span class="apidocSignatureSpan">d3.curveCatmullRom.</span>alpha (alpha)](#apidoc.element.d3.curveCatmullRom.alpha)

#### [module d3.curveCatmullRomClosed](#apidoc.module.d3.curveCatmullRomClosed)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCatmullRomClosed (context)](#apidoc.element.d3.curveCatmullRomClosed.curveCatmullRomClosed)
1.  [function <span class="apidocSignatureSpan">d3.curveCatmullRomClosed.</span>alpha (alpha)](#apidoc.element.d3.curveCatmullRomClosed.alpha)

#### [module d3.curveCatmullRomOpen](#apidoc.module.d3.curveCatmullRomOpen)
1.  [function <span class="apidocSignatureSpan">d3.</span>curveCatmullRomOpen (context)](#apidoc.element.d3.curveCatmullRomOpen.curveCatmullRomOpen)
1.  [function <span class="apidocSignatureSpan">d3.curveCatmullRomOpen.</span>alpha (alpha)](#apidoc.element.d3.curveCatmullRomOpen.alpha)

#### [module d3.dispatch](#apidoc.module.d3.dispatch)
1.  [function <span class="apidocSignatureSpan">d3.</span>dispatch ()](#apidoc.element.d3.dispatch.dispatch)

#### [module d3.dispatch.prototype](#apidoc.module.d3.dispatch.prototype)
1.  [function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>apply (type, that, args)](#apidoc.element.d3.dispatch.prototype.apply)
1.  [function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>call (type, that)](#apidoc.element.d3.dispatch.prototype.call)
1.  [function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>constructor (_)](#apidoc.element.d3.dispatch.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>copy ()](#apidoc.element.d3.dispatch.prototype.copy)
1.  [function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>on (typename, callback)](#apidoc.element.d3.dispatch.prototype.on)

#### [module d3.dispatch.prototype.constructor](#apidoc.module.d3.dispatch.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>constructor ()](#apidoc.element.d3.dispatch.prototype.constructor.constructor)

#### [module d3.easeBack](#apidoc.module.d3.easeBack)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBack (t)](#apidoc.element.d3.easeBack.easeBack)
1.  [function <span class="apidocSignatureSpan">d3.easeBack.</span>overshoot (s)](#apidoc.element.d3.easeBack.overshoot)

#### [module d3.easeBackIn](#apidoc.module.d3.easeBackIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBackIn (t)](#apidoc.element.d3.easeBackIn.easeBackIn)
1.  [function <span class="apidocSignatureSpan">d3.easeBackIn.</span>overshoot (s)](#apidoc.element.d3.easeBackIn.overshoot)

#### [module d3.easeBackOut](#apidoc.module.d3.easeBackOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeBackOut (t)](#apidoc.element.d3.easeBackOut.easeBackOut)
1.  [function <span class="apidocSignatureSpan">d3.easeBackOut.</span>overshoot (s)](#apidoc.element.d3.easeBackOut.overshoot)

#### [module d3.easeElastic](#apidoc.module.d3.easeElastic)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeElastic (t)](#apidoc.element.d3.easeElastic.easeElastic)
1.  [function <span class="apidocSignatureSpan">d3.easeElastic.</span>amplitude (a)](#apidoc.element.d3.easeElastic.amplitude)
1.  [function <span class="apidocSignatureSpan">d3.easeElastic.</span>period (p)](#apidoc.element.d3.easeElastic.period)

#### [module d3.easeElasticIn](#apidoc.module.d3.easeElasticIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeElasticIn (t)](#apidoc.element.d3.easeElasticIn.easeElasticIn)
1.  [function <span class="apidocSignatureSpan">d3.easeElasticIn.</span>amplitude (a)](#apidoc.element.d3.easeElasticIn.amplitude)
1.  [function <span class="apidocSignatureSpan">d3.easeElasticIn.</span>period (p)](#apidoc.element.d3.easeElasticIn.period)

#### [module d3.easeElasticInOut](#apidoc.module.d3.easeElasticInOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easeElasticInOut (t)](#apidoc.element.d3.easeElasticInOut.easeElasticInOut)
1.  [function <span class="apidocSignatureSpan">d3.easeElasticInOut.</span>amplitude (a)](#apidoc.element.d3.easeElasticInOut.amplitude)
1.  [function <span class="apidocSignatureSpan">d3.easeElasticInOut.</span>period (p)](#apidoc.element.d3.easeElasticInOut.period)

#### [module d3.easePoly](#apidoc.module.d3.easePoly)
1.  [function <span class="apidocSignatureSpan">d3.</span>easePoly (t)](#apidoc.element.d3.easePoly.easePoly)
1.  [function <span class="apidocSignatureSpan">d3.easePoly.</span>exponent (e)](#apidoc.element.d3.easePoly.exponent)

#### [module d3.easePolyIn](#apidoc.module.d3.easePolyIn)
1.  [function <span class="apidocSignatureSpan">d3.</span>easePolyIn (t)](#apidoc.element.d3.easePolyIn.easePolyIn)
1.  [function <span class="apidocSignatureSpan">d3.easePolyIn.</span>exponent (e)](#apidoc.element.d3.easePolyIn.exponent)

#### [module d3.easePolyOut](#apidoc.module.d3.easePolyOut)
1.  [function <span class="apidocSignatureSpan">d3.</span>easePolyOut (t)](#apidoc.element.d3.easePolyOut.easePolyOut)
1.  [function <span class="apidocSignatureSpan">d3.easePolyOut.</span>exponent (e)](#apidoc.element.d3.easePolyOut.exponent)

#### [module d3.formatSpecifier](#apidoc.module.d3.formatSpecifier)
1.  [function <span class="apidocSignatureSpan">d3.</span>formatSpecifier (specifier)](#apidoc.element.d3.formatSpecifier.formatSpecifier)

#### [module d3.formatSpecifier.prototype](#apidoc.module.d3.formatSpecifier.prototype)
1.  [function <span class="apidocSignatureSpan">d3.formatSpecifier.prototype.</span>toString ()](#apidoc.element.d3.formatSpecifier.prototype.toString)

#### [module d3.geoAzimuthalEqualAreaRaw](#apidoc.module.d3.geoAzimuthalEqualAreaRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEqualAreaRaw (x, y)](#apidoc.element.d3.geoAzimuthalEqualAreaRaw.geoAzimuthalEqualAreaRaw)
1.  [function <span class="apidocSignatureSpan">d3.geoAzimuthalEqualAreaRaw.</span>invert (x, y)](#apidoc.element.d3.geoAzimuthalEqualAreaRaw.invert)

#### [module d3.geoAzimuthalEquidistantRaw](#apidoc.module.d3.geoAzimuthalEquidistantRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEquidistantRaw (x, y)](#apidoc.element.d3.geoAzimuthalEquidistantRaw.geoAzimuthalEquidistantRaw)
1.  [function <span class="apidocSignatureSpan">d3.geoAzimuthalEquidistantRaw.</span>invert (x, y)](#apidoc.element.d3.geoAzimuthalEquidistantRaw.invert)

#### [module d3.geoEquirectangularRaw](#apidoc.module.d3.geoEquirectangularRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoEquirectangularRaw (lambda, phi)](#apidoc.element.d3.geoEquirectangularRaw.geoEquirectangularRaw)
1.  [function <span class="apidocSignatureSpan">d3.geoEquirectangularRaw.</span>invert (lambda, phi)](#apidoc.element.d3.geoEquirectangularRaw.invert)

#### [module d3.geoGnomonicRaw](#apidoc.module.d3.geoGnomonicRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoGnomonicRaw (x, y)](#apidoc.element.d3.geoGnomonicRaw.geoGnomonicRaw)
1.  [function <span class="apidocSignatureSpan">d3.geoGnomonicRaw.</span>invert (x, y)](#apidoc.element.d3.geoGnomonicRaw.invert)

#### [module d3.geoMercatorRaw](#apidoc.module.d3.geoMercatorRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoMercatorRaw (lambda, phi)](#apidoc.element.d3.geoMercatorRaw.geoMercatorRaw)
1.  [function <span class="apidocSignatureSpan">d3.geoMercatorRaw.</span>invert (x, y)](#apidoc.element.d3.geoMercatorRaw.invert)

#### [module d3.geoOrthographicRaw](#apidoc.module.d3.geoOrthographicRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoOrthographicRaw (x, y)](#apidoc.element.d3.geoOrthographicRaw.geoOrthographicRaw)
1.  [function <span class="apidocSignatureSpan">d3.geoOrthographicRaw.</span>invert (x, y)](#apidoc.element.d3.geoOrthographicRaw.invert)

#### [module d3.geoStereographicRaw](#apidoc.module.d3.geoStereographicRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoStereographicRaw (x, y)](#apidoc.element.d3.geoStereographicRaw.geoStereographicRaw)
1.  [function <span class="apidocSignatureSpan">d3.geoStereographicRaw.</span>invert (x, y)](#apidoc.element.d3.geoStereographicRaw.invert)

#### [module d3.geoTransverseMercatorRaw](#apidoc.module.d3.geoTransverseMercatorRaw)
1.  [function <span class="apidocSignatureSpan">d3.</span>geoTransverseMercatorRaw (lambda, phi)](#apidoc.element.d3.geoTransverseMercatorRaw.geoTransverseMercatorRaw)
1.  [function <span class="apidocSignatureSpan">d3.geoTransverseMercatorRaw.</span>invert (x, y)](#apidoc.element.d3.geoTransverseMercatorRaw.invert)

#### [module d3.hcl](#apidoc.module.d3.hcl)
1.  [function <span class="apidocSignatureSpan">d3.</span>hcl (h, c, l, opacity)](#apidoc.element.d3.hcl.hcl)

#### [module d3.hcl.prototype](#apidoc.module.d3.hcl.prototype)
1.  [function <span class="apidocSignatureSpan">d3.hcl.prototype.</span>brighter (k)](#apidoc.element.d3.hcl.prototype.brighter)
1.  [function <span class="apidocSignatureSpan">d3.hcl.prototype.</span>constructor (h, c, l, opacity)](#apidoc.element.d3.hcl.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.hcl.prototype.</span>darker (k)](#apidoc.element.d3.hcl.prototype.darker)
1.  [function <span class="apidocSignatureSpan">d3.hcl.prototype.</span>rgb ()](#apidoc.element.d3.hcl.prototype.rgb)

#### [module d3.hcl.prototype.constructor](#apidoc.module.d3.hcl.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.hcl.prototype.</span>constructor ()](#apidoc.element.d3.hcl.prototype.constructor.constructor)

#### [module d3.hierarchy](#apidoc.module.d3.hierarchy)
1.  [function <span class="apidocSignatureSpan">d3.</span>hierarchy (data, children)](#apidoc.element.d3.hierarchy.hierarchy)

#### [module d3.hierarchy.prototype](#apidoc.module.d3.hierarchy.prototype)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>ancestors ()](#apidoc.element.d3.hierarchy.prototype.ancestors)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>constructor (data)](#apidoc.element.d3.hierarchy.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>copy ()](#apidoc.element.d3.hierarchy.prototype.copy)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>count ()](#apidoc.element.d3.hierarchy.prototype.count)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>descendants ()](#apidoc.element.d3.hierarchy.prototype.descendants)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>each (callback)](#apidoc.element.d3.hierarchy.prototype.each)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>eachAfter (callback)](#apidoc.element.d3.hierarchy.prototype.eachAfter)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>eachBefore (callback)](#apidoc.element.d3.hierarchy.prototype.eachBefore)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>leaves ()](#apidoc.element.d3.hierarchy.prototype.leaves)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>links ()](#apidoc.element.d3.hierarchy.prototype.links)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>path (end)](#apidoc.element.d3.hierarchy.prototype.path)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>sort (compare)](#apidoc.element.d3.hierarchy.prototype.sort)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>sum (value)](#apidoc.element.d3.hierarchy.prototype.sum)

#### [module d3.hierarchy.prototype.constructor](#apidoc.module.d3.hierarchy.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>constructor ()](#apidoc.element.d3.hierarchy.prototype.constructor.constructor)

#### [module d3.hsl](#apidoc.module.d3.hsl)
1.  [function <span class="apidocSignatureSpan">d3.</span>hsl (h, s, l, opacity)](#apidoc.element.d3.hsl.hsl)

#### [module d3.hsl.prototype](#apidoc.module.d3.hsl.prototype)
1.  [function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>brighter (k)](#apidoc.element.d3.hsl.prototype.brighter)
1.  [function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>constructor (h, s, l, opacity)](#apidoc.element.d3.hsl.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>darker (k)](#apidoc.element.d3.hsl.prototype.darker)
1.  [function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>displayable ()](#apidoc.element.d3.hsl.prototype.displayable)
1.  [function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>rgb ()](#apidoc.element.d3.hsl.prototype.rgb)

#### [module d3.hsl.prototype.constructor](#apidoc.module.d3.hsl.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>constructor ()](#apidoc.element.d3.hsl.prototype.constructor.constructor)

#### [module d3.interpolateCubehelix](#apidoc.module.d3.interpolateCubehelix)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateCubehelix (start, end)](#apidoc.element.d3.interpolateCubehelix.interpolateCubehelix)
1.  [function <span class="apidocSignatureSpan">d3.interpolateCubehelix.</span>gamma (y)](#apidoc.element.d3.interpolateCubehelix.gamma)

#### [module d3.interpolateCubehelixLong](#apidoc.module.d3.interpolateCubehelixLong)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateCubehelixLong (start, end)](#apidoc.element.d3.interpolateCubehelixLong.interpolateCubehelixLong)
1.  [function <span class="apidocSignatureSpan">d3.interpolateCubehelixLong.</span>gamma (y)](#apidoc.element.d3.interpolateCubehelixLong.gamma)

#### [module d3.interpolateRgb](#apidoc.module.d3.interpolateRgb)
1.  [function <span class="apidocSignatureSpan">d3.</span>interpolateRgb (start, end)](#apidoc.element.d3.interpolateRgb.interpolateRgb)
1.  [function <span class="apidocSignatureSpan">d3.interpolateRgb.</span>gamma (y)](#apidoc.element.d3.interpolateRgb.gamma)

#### [module d3.lab](#apidoc.module.d3.lab)
1.  [function <span class="apidocSignatureSpan">d3.</span>lab (l, a, b, opacity)](#apidoc.element.d3.lab.lab)

#### [module d3.lab.prototype](#apidoc.module.d3.lab.prototype)
1.  [function <span class="apidocSignatureSpan">d3.lab.prototype.</span>brighter (k)](#apidoc.element.d3.lab.prototype.brighter)
1.  [function <span class="apidocSignatureSpan">d3.lab.prototype.</span>constructor (l, a, b, opacity)](#apidoc.element.d3.lab.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.lab.prototype.</span>darker (k)](#apidoc.element.d3.lab.prototype.darker)
1.  [function <span class="apidocSignatureSpan">d3.lab.prototype.</span>rgb ()](#apidoc.element.d3.lab.prototype.rgb)

#### [module d3.lab.prototype.constructor](#apidoc.module.d3.lab.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.lab.prototype.</span>constructor ()](#apidoc.element.d3.lab.prototype.constructor.constructor)

#### [module d3.local](#apidoc.module.d3.local)
1.  [function <span class="apidocSignatureSpan">d3.</span>local ()](#apidoc.element.d3.local.local)

#### [module d3.local.prototype](#apidoc.module.d3.local.prototype)
1.  [function <span class="apidocSignatureSpan">d3.local.prototype.</span>constructor ()](#apidoc.element.d3.local.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.local.prototype.</span>get (node)](#apidoc.element.d3.local.prototype.get)
1.  [function <span class="apidocSignatureSpan">d3.local.prototype.</span>remove (node)](#apidoc.element.d3.local.prototype.remove)
1.  [function <span class="apidocSignatureSpan">d3.local.prototype.</span>set (node, value)](#apidoc.element.d3.local.prototype.set)
1.  [function <span class="apidocSignatureSpan">d3.local.prototype.</span>toString ()](#apidoc.element.d3.local.prototype.toString)

#### [module d3.local.prototype.constructor](#apidoc.module.d3.local.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.local.prototype.</span>constructor ()](#apidoc.element.d3.local.prototype.constructor.constructor)

#### [module d3.map](#apidoc.module.d3.map)
1.  [function <span class="apidocSignatureSpan">d3.</span>map (object, f)](#apidoc.element.d3.map.map)

#### [module d3.map.prototype](#apidoc.module.d3.map.prototype)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>clear ()](#apidoc.element.d3.map.prototype.clear)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>constructor ()](#apidoc.element.d3.map.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>each (f)](#apidoc.element.d3.map.prototype.each)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>empty ()](#apidoc.element.d3.map.prototype.empty)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>entries ()](#apidoc.element.d3.map.prototype.entries)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>get (key)](#apidoc.element.d3.map.prototype.get)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>has (key)](#apidoc.element.d3.map.prototype.has)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>keys ()](#apidoc.element.d3.map.prototype.keys)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>remove (key)](#apidoc.element.d3.map.prototype.remove)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>set (key, value)](#apidoc.element.d3.map.prototype.set)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>size ()](#apidoc.element.d3.map.prototype.size)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>values ()](#apidoc.element.d3.map.prototype.values)

#### [module d3.map.prototype.constructor](#apidoc.module.d3.map.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.map.prototype.</span>constructor ()](#apidoc.element.d3.map.prototype.constructor.constructor)

#### [module d3.path](#apidoc.module.d3.path)
1.  [function <span class="apidocSignatureSpan">d3.</span>path ()](#apidoc.element.d3.path.path)

#### [module d3.path.prototype](#apidoc.module.d3.path.prototype)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>arc (x, y, r, a0, a1, ccw)](#apidoc.element.d3.path.prototype.arc)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>arcTo (x1, y1, x2, y2, r)](#apidoc.element.d3.path.prototype.arcTo)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>bezierCurveTo (x1, y1, x2, y2, x, y)](#apidoc.element.d3.path.prototype.bezierCurveTo)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>closePath ()](#apidoc.element.d3.path.prototype.closePath)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>constructor ()](#apidoc.element.d3.path.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>lineTo (x, y)](#apidoc.element.d3.path.prototype.lineTo)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>moveTo (x, y)](#apidoc.element.d3.path.prototype.moveTo)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>quadraticCurveTo (x1, y1, x, y)](#apidoc.element.d3.path.prototype.quadraticCurveTo)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>rect (x, y, w, h)](#apidoc.element.d3.path.prototype.rect)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>toString ()](#apidoc.element.d3.path.prototype.toString)

#### [module d3.path.prototype.constructor](#apidoc.module.d3.path.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.path.prototype.</span>constructor ()](#apidoc.element.d3.path.prototype.constructor.constructor)

#### [module d3.quadtree](#apidoc.module.d3.quadtree)
1.  [function <span class="apidocSignatureSpan">d3.</span>quadtree (nodes, x, y)](#apidoc.element.d3.quadtree.quadtree)

#### [module d3.quadtree.prototype](#apidoc.module.d3.quadtree.prototype)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>add (d)](#apidoc.element.d3.quadtree.prototype.add)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>addAll (data)](#apidoc.element.d3.quadtree.prototype.addAll)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>copy ()](#apidoc.element.d3.quadtree.prototype.copy)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>cover (x, y)](#apidoc.element.d3.quadtree.prototype.cover)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>data ()](#apidoc.element.d3.quadtree.prototype.data)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>extent (_)](#apidoc.element.d3.quadtree.prototype.extent)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>find (x, y, radius)](#apidoc.element.d3.quadtree.prototype.find)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>remove (d)](#apidoc.element.d3.quadtree.prototype.remove)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>removeAll (data)](#apidoc.element.d3.quadtree.prototype.removeAll)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>root ()](#apidoc.element.d3.quadtree.prototype.root)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>size ()](#apidoc.element.d3.quadtree.prototype.size)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>visit (callback)](#apidoc.element.d3.quadtree.prototype.visit)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>visitAfter (callback)](#apidoc.element.d3.quadtree.prototype.visitAfter)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>x (_)](#apidoc.element.d3.quadtree.prototype.x)
1.  [function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>y (_)](#apidoc.element.d3.quadtree.prototype.y)

#### [module d3.queue](#apidoc.module.d3.queue)
1.  [function <span class="apidocSignatureSpan">d3.</span>queue (concurrency)](#apidoc.element.d3.queue.queue)

#### [module d3.queue.prototype](#apidoc.module.d3.queue.prototype)
1.  [function <span class="apidocSignatureSpan">d3.queue.prototype.</span>abort ()](#apidoc.element.d3.queue.prototype.abort)
1.  [function <span class="apidocSignatureSpan">d3.queue.prototype.</span>await (callback)](#apidoc.element.d3.queue.prototype.await)
1.  [function <span class="apidocSignatureSpan">d3.queue.prototype.</span>awaitAll (callback)](#apidoc.element.d3.queue.prototype.awaitAll)
1.  [function <span class="apidocSignatureSpan">d3.queue.prototype.</span>constructor (size)](#apidoc.element.d3.queue.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.queue.prototype.</span>defer (callback)](#apidoc.element.d3.queue.prototype.defer)

#### [module d3.queue.prototype.constructor](#apidoc.module.d3.queue.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.queue.prototype.</span>constructor ()](#apidoc.element.d3.queue.prototype.constructor.constructor)

#### [module d3.rgb](#apidoc.module.d3.rgb)
1.  [function <span class="apidocSignatureSpan">d3.</span>rgb (r, g, b, opacity)](#apidoc.element.d3.rgb.rgb)

#### [module d3.rgb.prototype](#apidoc.module.d3.rgb.prototype)
1.  [function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>brighter (k)](#apidoc.element.d3.rgb.prototype.brighter)
1.  [function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>constructor (r, g, b, opacity)](#apidoc.element.d3.rgb.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>darker (k)](#apidoc.element.d3.rgb.prototype.darker)
1.  [function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>displayable ()](#apidoc.element.d3.rgb.prototype.displayable)
1.  [function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>rgb ()](#apidoc.element.d3.rgb.prototype.rgb)
1.  [function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>toString ()](#apidoc.element.d3.rgb.prototype.toString)

#### [module d3.rgb.prototype.constructor](#apidoc.module.d3.rgb.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>constructor ()](#apidoc.element.d3.rgb.prototype.constructor.constructor)

#### [module d3.selection](#apidoc.module.d3.selection)
1.  [function <span class="apidocSignatureSpan">d3.</span>selection ()](#apidoc.element.d3.selection.selection)

#### [module d3.selection.prototype](#apidoc.module.d3.selection.prototype)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>append (name)](#apidoc.element.d3.selection.prototype.append)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>attr (name, value)](#apidoc.element.d3.selection.prototype.attr)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>call ()](#apidoc.element.d3.selection.prototype.call)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>classed (name, value)](#apidoc.element.d3.selection.prototype.classed)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>constructor (groups, parents)](#apidoc.element.d3.selection.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>data (value, key)](#apidoc.element.d3.selection.prototype.data)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>datum (value)](#apidoc.element.d3.selection.prototype.datum)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>dispatch (type, params)](#apidoc.element.d3.selection.prototype.dispatch)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>each (callback)](#apidoc.element.d3.selection.prototype.each)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>empty ()](#apidoc.element.d3.selection.prototype.empty)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>enter ()](#apidoc.element.d3.selection.prototype.enter)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>exit ()](#apidoc.element.d3.selection.prototype.exit)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>filter (match)](#apidoc.element.d3.selection.prototype.filter)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>html (value)](#apidoc.element.d3.selection.prototype.html)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>insert (name, before)](#apidoc.element.d3.selection.prototype.insert)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>interrupt (name)](#apidoc.element.d3.selection.prototype.interrupt)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>lower ()](#apidoc.element.d3.selection.prototype.lower)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>merge (selection)](#apidoc.element.d3.selection.prototype.merge)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>node ()](#apidoc.element.d3.selection.prototype.node)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>nodes ()](#apidoc.element.d3.selection.prototype.nodes)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>on (typename, value, capture)](#apidoc.element.d3.selection.prototype.on)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>order ()](#apidoc.element.d3.selection.prototype.order)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>property (name, value)](#apidoc.element.d3.selection.prototype.property)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>raise ()](#apidoc.element.d3.selection.prototype.raise)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>remove ()](#apidoc.element.d3.selection.prototype.remove)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>select (select)](#apidoc.element.d3.selection.prototype.select)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>selectAll (select)](#apidoc.element.d3.selection.prototype.selectAll)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>size ()](#apidoc.element.d3.selection.prototype.size)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>sort (compare)](#apidoc.element.d3.selection.prototype.sort)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>style (name, value, priority)](#apidoc.element.d3.selection.prototype.style)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>text (value)](#apidoc.element.d3.selection.prototype.text)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>transition (name)](#apidoc.element.d3.selection.prototype.transition)

#### [module d3.selection.prototype.constructor](#apidoc.module.d3.selection.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.selection.prototype.</span>constructor ()](#apidoc.element.d3.selection.prototype.constructor.constructor)

#### [module d3.set](#apidoc.module.d3.set)
1.  [function <span class="apidocSignatureSpan">d3.</span>set (object, f)](#apidoc.element.d3.set.set)

#### [module d3.set.prototype](#apidoc.module.d3.set.prototype)
1.  [function <span class="apidocSignatureSpan">d3.set.prototype.</span>add (value)](#apidoc.element.d3.set.prototype.add)
1.  [function <span class="apidocSignatureSpan">d3.set.prototype.</span>clear ()](#apidoc.element.d3.set.prototype.clear)
1.  [function <span class="apidocSignatureSpan">d3.set.prototype.</span>constructor ()](#apidoc.element.d3.set.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.set.prototype.</span>each (f)](#apidoc.element.d3.set.prototype.each)
1.  [function <span class="apidocSignatureSpan">d3.set.prototype.</span>empty ()](#apidoc.element.d3.set.prototype.empty)
1.  [function <span class="apidocSignatureSpan">d3.set.prototype.</span>has (key)](#apidoc.element.d3.set.prototype.has)
1.  [function <span class="apidocSignatureSpan">d3.set.prototype.</span>remove (key)](#apidoc.element.d3.set.prototype.remove)
1.  [function <span class="apidocSignatureSpan">d3.set.prototype.</span>size ()](#apidoc.element.d3.set.prototype.size)
1.  [function <span class="apidocSignatureSpan">d3.set.prototype.</span>values ()](#apidoc.element.d3.set.prototype.values)

#### [module d3.set.prototype.constructor](#apidoc.module.d3.set.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.set.prototype.</span>constructor ()](#apidoc.element.d3.set.prototype.constructor.constructor)

#### [module d3.symbolCircle](#apidoc.module.d3.symbolCircle)
1.  [function <span class="apidocSignatureSpan">d3.symbolCircle.</span>draw (context, size)](#apidoc.element.d3.symbolCircle.draw)

#### [module d3.symbolCross](#apidoc.module.d3.symbolCross)
1.  [function <span class="apidocSignatureSpan">d3.symbolCross.</span>draw (context, size)](#apidoc.element.d3.symbolCross.draw)

#### [module d3.symbolDiamond](#apidoc.module.d3.symbolDiamond)
1.  [function <span class="apidocSignatureSpan">d3.symbolDiamond.</span>draw (context, size)](#apidoc.element.d3.symbolDiamond.draw)

#### [module d3.symbolSquare](#apidoc.module.d3.symbolSquare)
1.  [function <span class="apidocSignatureSpan">d3.symbolSquare.</span>draw (context, size)](#apidoc.element.d3.symbolSquare.draw)

#### [module d3.symbolStar](#apidoc.module.d3.symbolStar)
1.  [function <span class="apidocSignatureSpan">d3.symbolStar.</span>draw (context, size)](#apidoc.element.d3.symbolStar.draw)

#### [module d3.symbolTriangle](#apidoc.module.d3.symbolTriangle)
1.  [function <span class="apidocSignatureSpan">d3.symbolTriangle.</span>draw (context, size)](#apidoc.element.d3.symbolTriangle.draw)

#### [module d3.symbolWye](#apidoc.module.d3.symbolWye)
1.  [function <span class="apidocSignatureSpan">d3.symbolWye.</span>draw (context, size)](#apidoc.element.d3.symbolWye.draw)

#### [module d3.timeDay](#apidoc.module.d3.timeDay)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeDay (date)](#apidoc.element.d3.timeDay.timeDay)
1.  [function <span class="apidocSignatureSpan">d3.timeDay.</span>ceil (date)](#apidoc.element.d3.timeDay.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeDay.</span>count (start, end)](#apidoc.element.d3.timeDay.count)
1.  [function <span class="apidocSignatureSpan">d3.timeDay.</span>every (step)](#apidoc.element.d3.timeDay.every)
1.  [function <span class="apidocSignatureSpan">d3.timeDay.</span>filter (test)](#apidoc.element.d3.timeDay.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeDay.</span>floor (date)](#apidoc.element.d3.timeDay.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeDay.</span>offset (date, step)](#apidoc.element.d3.timeDay.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeDay.</span>range (start, stop, step)](#apidoc.element.d3.timeDay.range)
1.  [function <span class="apidocSignatureSpan">d3.timeDay.</span>round (date)](#apidoc.element.d3.timeDay.round)

#### [module d3.timeFriday](#apidoc.module.d3.timeFriday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeFriday (date)](#apidoc.element.d3.timeFriday.timeFriday)
1.  [function <span class="apidocSignatureSpan">d3.timeFriday.</span>ceil (date)](#apidoc.element.d3.timeFriday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeFriday.</span>count (start, end)](#apidoc.element.d3.timeFriday.count)
1.  [function <span class="apidocSignatureSpan">d3.timeFriday.</span>every (step)](#apidoc.element.d3.timeFriday.every)
1.  [function <span class="apidocSignatureSpan">d3.timeFriday.</span>filter (test)](#apidoc.element.d3.timeFriday.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeFriday.</span>floor (date)](#apidoc.element.d3.timeFriday.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeFriday.</span>offset (date, step)](#apidoc.element.d3.timeFriday.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeFriday.</span>range (start, stop, step)](#apidoc.element.d3.timeFriday.range)
1.  [function <span class="apidocSignatureSpan">d3.timeFriday.</span>round (date)](#apidoc.element.d3.timeFriday.round)

#### [module d3.timeHour](#apidoc.module.d3.timeHour)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeHour (date)](#apidoc.element.d3.timeHour.timeHour)
1.  [function <span class="apidocSignatureSpan">d3.timeHour.</span>ceil (date)](#apidoc.element.d3.timeHour.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeHour.</span>count (start, end)](#apidoc.element.d3.timeHour.count)
1.  [function <span class="apidocSignatureSpan">d3.timeHour.</span>every (step)](#apidoc.element.d3.timeHour.every)
1.  [function <span class="apidocSignatureSpan">d3.timeHour.</span>filter (test)](#apidoc.element.d3.timeHour.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeHour.</span>floor (date)](#apidoc.element.d3.timeHour.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeHour.</span>offset (date, step)](#apidoc.element.d3.timeHour.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeHour.</span>range (start, stop, step)](#apidoc.element.d3.timeHour.range)
1.  [function <span class="apidocSignatureSpan">d3.timeHour.</span>round (date)](#apidoc.element.d3.timeHour.round)

#### [module d3.timeMillisecond](#apidoc.module.d3.timeMillisecond)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMillisecond (date)](#apidoc.element.d3.timeMillisecond.timeMillisecond)
1.  [function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>ceil (date)](#apidoc.element.d3.timeMillisecond.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>count (start, end)](#apidoc.element.d3.timeMillisecond.count)
1.  [function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>every (k)](#apidoc.element.d3.timeMillisecond.every)
1.  [function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>filter (test)](#apidoc.element.d3.timeMillisecond.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>floor (date)](#apidoc.element.d3.timeMillisecond.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>offset (date, step)](#apidoc.element.d3.timeMillisecond.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>range (start, stop, step)](#apidoc.element.d3.timeMillisecond.range)
1.  [function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>round (date)](#apidoc.element.d3.timeMillisecond.round)

#### [module d3.timeMinute](#apidoc.module.d3.timeMinute)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMinute (date)](#apidoc.element.d3.timeMinute.timeMinute)
1.  [function <span class="apidocSignatureSpan">d3.timeMinute.</span>ceil (date)](#apidoc.element.d3.timeMinute.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeMinute.</span>count (start, end)](#apidoc.element.d3.timeMinute.count)
1.  [function <span class="apidocSignatureSpan">d3.timeMinute.</span>every (step)](#apidoc.element.d3.timeMinute.every)
1.  [function <span class="apidocSignatureSpan">d3.timeMinute.</span>filter (test)](#apidoc.element.d3.timeMinute.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeMinute.</span>floor (date)](#apidoc.element.d3.timeMinute.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeMinute.</span>offset (date, step)](#apidoc.element.d3.timeMinute.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeMinute.</span>range (start, stop, step)](#apidoc.element.d3.timeMinute.range)
1.  [function <span class="apidocSignatureSpan">d3.timeMinute.</span>round (date)](#apidoc.element.d3.timeMinute.round)

#### [module d3.timeMonday](#apidoc.module.d3.timeMonday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMonday (date)](#apidoc.element.d3.timeMonday.timeMonday)
1.  [function <span class="apidocSignatureSpan">d3.timeMonday.</span>ceil (date)](#apidoc.element.d3.timeMonday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeMonday.</span>count (start, end)](#apidoc.element.d3.timeMonday.count)
1.  [function <span class="apidocSignatureSpan">d3.timeMonday.</span>every (step)](#apidoc.element.d3.timeMonday.every)
1.  [function <span class="apidocSignatureSpan">d3.timeMonday.</span>filter (test)](#apidoc.element.d3.timeMonday.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeMonday.</span>floor (date)](#apidoc.element.d3.timeMonday.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeMonday.</span>offset (date, step)](#apidoc.element.d3.timeMonday.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeMonday.</span>range (start, stop, step)](#apidoc.element.d3.timeMonday.range)
1.  [function <span class="apidocSignatureSpan">d3.timeMonday.</span>round (date)](#apidoc.element.d3.timeMonday.round)

#### [module d3.timeMonth](#apidoc.module.d3.timeMonth)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeMonth (date)](#apidoc.element.d3.timeMonth.timeMonth)
1.  [function <span class="apidocSignatureSpan">d3.timeMonth.</span>ceil (date)](#apidoc.element.d3.timeMonth.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeMonth.</span>count (start, end)](#apidoc.element.d3.timeMonth.count)
1.  [function <span class="apidocSignatureSpan">d3.timeMonth.</span>every (step)](#apidoc.element.d3.timeMonth.every)
1.  [function <span class="apidocSignatureSpan">d3.timeMonth.</span>filter (test)](#apidoc.element.d3.timeMonth.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeMonth.</span>floor (date)](#apidoc.element.d3.timeMonth.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeMonth.</span>offset (date, step)](#apidoc.element.d3.timeMonth.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeMonth.</span>range (start, stop, step)](#apidoc.element.d3.timeMonth.range)
1.  [function <span class="apidocSignatureSpan">d3.timeMonth.</span>round (date)](#apidoc.element.d3.timeMonth.round)

#### [module d3.timeSaturday](#apidoc.module.d3.timeSaturday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeSaturday (date)](#apidoc.element.d3.timeSaturday.timeSaturday)
1.  [function <span class="apidocSignatureSpan">d3.timeSaturday.</span>ceil (date)](#apidoc.element.d3.timeSaturday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeSaturday.</span>count (start, end)](#apidoc.element.d3.timeSaturday.count)
1.  [function <span class="apidocSignatureSpan">d3.timeSaturday.</span>every (step)](#apidoc.element.d3.timeSaturday.every)
1.  [function <span class="apidocSignatureSpan">d3.timeSaturday.</span>filter (test)](#apidoc.element.d3.timeSaturday.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeSaturday.</span>floor (date)](#apidoc.element.d3.timeSaturday.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeSaturday.</span>offset (date, step)](#apidoc.element.d3.timeSaturday.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeSaturday.</span>range (start, stop, step)](#apidoc.element.d3.timeSaturday.range)
1.  [function <span class="apidocSignatureSpan">d3.timeSaturday.</span>round (date)](#apidoc.element.d3.timeSaturday.round)

#### [module d3.timeSecond](#apidoc.module.d3.timeSecond)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeSecond (date)](#apidoc.element.d3.timeSecond.timeSecond)
1.  [function <span class="apidocSignatureSpan">d3.timeSecond.</span>ceil (date)](#apidoc.element.d3.timeSecond.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeSecond.</span>count (start, end)](#apidoc.element.d3.timeSecond.count)
1.  [function <span class="apidocSignatureSpan">d3.timeSecond.</span>every (step)](#apidoc.element.d3.timeSecond.every)
1.  [function <span class="apidocSignatureSpan">d3.timeSecond.</span>filter (test)](#apidoc.element.d3.timeSecond.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeSecond.</span>floor (date)](#apidoc.element.d3.timeSecond.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeSecond.</span>offset (date, step)](#apidoc.element.d3.timeSecond.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeSecond.</span>range (start, stop, step)](#apidoc.element.d3.timeSecond.range)
1.  [function <span class="apidocSignatureSpan">d3.timeSecond.</span>round (date)](#apidoc.element.d3.timeSecond.round)

#### [module d3.timeThursday](#apidoc.module.d3.timeThursday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeThursday (date)](#apidoc.element.d3.timeThursday.timeThursday)
1.  [function <span class="apidocSignatureSpan">d3.timeThursday.</span>ceil (date)](#apidoc.element.d3.timeThursday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeThursday.</span>count (start, end)](#apidoc.element.d3.timeThursday.count)
1.  [function <span class="apidocSignatureSpan">d3.timeThursday.</span>every (step)](#apidoc.element.d3.timeThursday.every)
1.  [function <span class="apidocSignatureSpan">d3.timeThursday.</span>filter (test)](#apidoc.element.d3.timeThursday.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeThursday.</span>floor (date)](#apidoc.element.d3.timeThursday.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeThursday.</span>offset (date, step)](#apidoc.element.d3.timeThursday.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeThursday.</span>range (start, stop, step)](#apidoc.element.d3.timeThursday.range)
1.  [function <span class="apidocSignatureSpan">d3.timeThursday.</span>round (date)](#apidoc.element.d3.timeThursday.round)

#### [module d3.timeTuesday](#apidoc.module.d3.timeTuesday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeTuesday (date)](#apidoc.element.d3.timeTuesday.timeTuesday)
1.  [function <span class="apidocSignatureSpan">d3.timeTuesday.</span>ceil (date)](#apidoc.element.d3.timeTuesday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeTuesday.</span>count (start, end)](#apidoc.element.d3.timeTuesday.count)
1.  [function <span class="apidocSignatureSpan">d3.timeTuesday.</span>every (step)](#apidoc.element.d3.timeTuesday.every)
1.  [function <span class="apidocSignatureSpan">d3.timeTuesday.</span>filter (test)](#apidoc.element.d3.timeTuesday.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeTuesday.</span>floor (date)](#apidoc.element.d3.timeTuesday.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeTuesday.</span>offset (date, step)](#apidoc.element.d3.timeTuesday.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeTuesday.</span>range (start, stop, step)](#apidoc.element.d3.timeTuesday.range)
1.  [function <span class="apidocSignatureSpan">d3.timeTuesday.</span>round (date)](#apidoc.element.d3.timeTuesday.round)

#### [module d3.timeWednesday](#apidoc.module.d3.timeWednesday)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeWednesday (date)](#apidoc.element.d3.timeWednesday.timeWednesday)
1.  [function <span class="apidocSignatureSpan">d3.timeWednesday.</span>ceil (date)](#apidoc.element.d3.timeWednesday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeWednesday.</span>count (start, end)](#apidoc.element.d3.timeWednesday.count)
1.  [function <span class="apidocSignatureSpan">d3.timeWednesday.</span>every (step)](#apidoc.element.d3.timeWednesday.every)
1.  [function <span class="apidocSignatureSpan">d3.timeWednesday.</span>filter (test)](#apidoc.element.d3.timeWednesday.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeWednesday.</span>floor (date)](#apidoc.element.d3.timeWednesday.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeWednesday.</span>offset (date, step)](#apidoc.element.d3.timeWednesday.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeWednesday.</span>range (start, stop, step)](#apidoc.element.d3.timeWednesday.range)
1.  [function <span class="apidocSignatureSpan">d3.timeWednesday.</span>round (date)](#apidoc.element.d3.timeWednesday.round)

#### [module d3.timeWeek](#apidoc.module.d3.timeWeek)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeWeek (date)](#apidoc.element.d3.timeWeek.timeWeek)
1.  [function <span class="apidocSignatureSpan">d3.timeWeek.</span>ceil (date)](#apidoc.element.d3.timeWeek.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeWeek.</span>count (start, end)](#apidoc.element.d3.timeWeek.count)
1.  [function <span class="apidocSignatureSpan">d3.timeWeek.</span>every (step)](#apidoc.element.d3.timeWeek.every)
1.  [function <span class="apidocSignatureSpan">d3.timeWeek.</span>filter (test)](#apidoc.element.d3.timeWeek.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeWeek.</span>floor (date)](#apidoc.element.d3.timeWeek.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeWeek.</span>offset (date, step)](#apidoc.element.d3.timeWeek.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeWeek.</span>range (start, stop, step)](#apidoc.element.d3.timeWeek.range)
1.  [function <span class="apidocSignatureSpan">d3.timeWeek.</span>round (date)](#apidoc.element.d3.timeWeek.round)

#### [module d3.timeYear](#apidoc.module.d3.timeYear)
1.  [function <span class="apidocSignatureSpan">d3.</span>timeYear (date)](#apidoc.element.d3.timeYear.timeYear)
1.  [function <span class="apidocSignatureSpan">d3.timeYear.</span>ceil (date)](#apidoc.element.d3.timeYear.ceil)
1.  [function <span class="apidocSignatureSpan">d3.timeYear.</span>count (start, end)](#apidoc.element.d3.timeYear.count)
1.  [function <span class="apidocSignatureSpan">d3.timeYear.</span>every (k)](#apidoc.element.d3.timeYear.every)
1.  [function <span class="apidocSignatureSpan">d3.timeYear.</span>filter (test)](#apidoc.element.d3.timeYear.filter)
1.  [function <span class="apidocSignatureSpan">d3.timeYear.</span>floor (date)](#apidoc.element.d3.timeYear.floor)
1.  [function <span class="apidocSignatureSpan">d3.timeYear.</span>offset (date, step)](#apidoc.element.d3.timeYear.offset)
1.  [function <span class="apidocSignatureSpan">d3.timeYear.</span>range (start, stop, step)](#apidoc.element.d3.timeYear.range)
1.  [function <span class="apidocSignatureSpan">d3.timeYear.</span>round (date)](#apidoc.element.d3.timeYear.round)

#### [module d3.timer](#apidoc.module.d3.timer)
1.  [function <span class="apidocSignatureSpan">d3.</span>timer (callback, delay, time)](#apidoc.element.d3.timer.timer)

#### [module d3.timer.prototype](#apidoc.module.d3.timer.prototype)
1.  [function <span class="apidocSignatureSpan">d3.timer.prototype.</span>constructor ()](#apidoc.element.d3.timer.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.timer.prototype.</span>restart (callback, delay, time)](#apidoc.element.d3.timer.prototype.restart)
1.  [function <span class="apidocSignatureSpan">d3.timer.prototype.</span>stop ()](#apidoc.element.d3.timer.prototype.stop)

#### [module d3.timer.prototype.constructor](#apidoc.module.d3.timer.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.timer.prototype.</span>constructor ()](#apidoc.element.d3.timer.prototype.constructor.constructor)

#### [module d3.transition](#apidoc.module.d3.transition)
1.  [function <span class="apidocSignatureSpan">d3.</span>transition (name)](#apidoc.element.d3.transition.transition)

#### [module d3.transition.prototype](#apidoc.module.d3.transition.prototype)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>attr (name, value)](#apidoc.element.d3.transition.prototype.attr)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>attrTween (name, value)](#apidoc.element.d3.transition.prototype.attrTween)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>call ()](#apidoc.element.d3.transition.prototype.call)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>constructor (groups, parents, name, id)](#apidoc.element.d3.transition.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>delay (value)](#apidoc.element.d3.transition.prototype.delay)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>duration (value)](#apidoc.element.d3.transition.prototype.duration)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>each (callback)](#apidoc.element.d3.transition.prototype.each)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>ease (value)](#apidoc.element.d3.transition.prototype.ease)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>empty ()](#apidoc.element.d3.transition.prototype.empty)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>filter (match)](#apidoc.element.d3.transition.prototype.filter)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>merge (transition)](#apidoc.element.d3.transition.prototype.merge)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>node ()](#apidoc.element.d3.transition.prototype.node)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>nodes ()](#apidoc.element.d3.transition.prototype.nodes)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>on (name, listener)](#apidoc.element.d3.transition.prototype.on)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>remove ()](#apidoc.element.d3.transition.prototype.remove)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>select (select)](#apidoc.element.d3.transition.prototype.select)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>selectAll (select)](#apidoc.element.d3.transition.prototype.selectAll)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>selection ()](#apidoc.element.d3.transition.prototype.selection)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>size ()](#apidoc.element.d3.transition.prototype.size)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>style (name, value, priority)](#apidoc.element.d3.transition.prototype.style)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>styleTween (name, value, priority)](#apidoc.element.d3.transition.prototype.styleTween)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>text (value)](#apidoc.element.d3.transition.prototype.text)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>transition ()](#apidoc.element.d3.transition.prototype.transition)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>tween (name, value)](#apidoc.element.d3.transition.prototype.tween)

#### [module d3.transition.prototype.constructor](#apidoc.module.d3.transition.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.transition.prototype.</span>constructor ()](#apidoc.element.d3.transition.prototype.constructor.constructor)

#### [module d3.treemapResquarify](#apidoc.module.d3.treemapResquarify)
1.  [function <span class="apidocSignatureSpan">d3.</span>treemapResquarify (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapResquarify.treemapResquarify)
1.  [function <span class="apidocSignatureSpan">d3.treemapResquarify.</span>ratio (x)](#apidoc.element.d3.treemapResquarify.ratio)

#### [module d3.treemapSquarify](#apidoc.module.d3.treemapSquarify)
1.  [function <span class="apidocSignatureSpan">d3.</span>treemapSquarify (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapSquarify.treemapSquarify)
1.  [function <span class="apidocSignatureSpan">d3.treemapSquarify.</span>ratio (x)](#apidoc.element.d3.treemapSquarify.ratio)

#### [module d3.utcDay](#apidoc.module.d3.utcDay)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcDay (date)](#apidoc.element.d3.utcDay.utcDay)
1.  [function <span class="apidocSignatureSpan">d3.utcDay.</span>ceil (date)](#apidoc.element.d3.utcDay.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcDay.</span>count (start, end)](#apidoc.element.d3.utcDay.count)
1.  [function <span class="apidocSignatureSpan">d3.utcDay.</span>every (step)](#apidoc.element.d3.utcDay.every)
1.  [function <span class="apidocSignatureSpan">d3.utcDay.</span>filter (test)](#apidoc.element.d3.utcDay.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcDay.</span>floor (date)](#apidoc.element.d3.utcDay.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcDay.</span>offset (date, step)](#apidoc.element.d3.utcDay.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcDay.</span>range (start, stop, step)](#apidoc.element.d3.utcDay.range)
1.  [function <span class="apidocSignatureSpan">d3.utcDay.</span>round (date)](#apidoc.element.d3.utcDay.round)

#### [module d3.utcFriday](#apidoc.module.d3.utcFriday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcFriday (date)](#apidoc.element.d3.utcFriday.utcFriday)
1.  [function <span class="apidocSignatureSpan">d3.utcFriday.</span>ceil (date)](#apidoc.element.d3.utcFriday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcFriday.</span>count (start, end)](#apidoc.element.d3.utcFriday.count)
1.  [function <span class="apidocSignatureSpan">d3.utcFriday.</span>every (step)](#apidoc.element.d3.utcFriday.every)
1.  [function <span class="apidocSignatureSpan">d3.utcFriday.</span>filter (test)](#apidoc.element.d3.utcFriday.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcFriday.</span>floor (date)](#apidoc.element.d3.utcFriday.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcFriday.</span>offset (date, step)](#apidoc.element.d3.utcFriday.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcFriday.</span>range (start, stop, step)](#apidoc.element.d3.utcFriday.range)
1.  [function <span class="apidocSignatureSpan">d3.utcFriday.</span>round (date)](#apidoc.element.d3.utcFriday.round)

#### [module d3.utcHour](#apidoc.module.d3.utcHour)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcHour (date)](#apidoc.element.d3.utcHour.utcHour)
1.  [function <span class="apidocSignatureSpan">d3.utcHour.</span>ceil (date)](#apidoc.element.d3.utcHour.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcHour.</span>count (start, end)](#apidoc.element.d3.utcHour.count)
1.  [function <span class="apidocSignatureSpan">d3.utcHour.</span>every (step)](#apidoc.element.d3.utcHour.every)
1.  [function <span class="apidocSignatureSpan">d3.utcHour.</span>filter (test)](#apidoc.element.d3.utcHour.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcHour.</span>floor (date)](#apidoc.element.d3.utcHour.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcHour.</span>offset (date, step)](#apidoc.element.d3.utcHour.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcHour.</span>range (start, stop, step)](#apidoc.element.d3.utcHour.range)
1.  [function <span class="apidocSignatureSpan">d3.utcHour.</span>round (date)](#apidoc.element.d3.utcHour.round)

#### [module d3.utcMinute](#apidoc.module.d3.utcMinute)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMinute (date)](#apidoc.element.d3.utcMinute.utcMinute)
1.  [function <span class="apidocSignatureSpan">d3.utcMinute.</span>ceil (date)](#apidoc.element.d3.utcMinute.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcMinute.</span>count (start, end)](#apidoc.element.d3.utcMinute.count)
1.  [function <span class="apidocSignatureSpan">d3.utcMinute.</span>every (step)](#apidoc.element.d3.utcMinute.every)
1.  [function <span class="apidocSignatureSpan">d3.utcMinute.</span>filter (test)](#apidoc.element.d3.utcMinute.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcMinute.</span>floor (date)](#apidoc.element.d3.utcMinute.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcMinute.</span>offset (date, step)](#apidoc.element.d3.utcMinute.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcMinute.</span>range (start, stop, step)](#apidoc.element.d3.utcMinute.range)
1.  [function <span class="apidocSignatureSpan">d3.utcMinute.</span>round (date)](#apidoc.element.d3.utcMinute.round)

#### [module d3.utcMonday](#apidoc.module.d3.utcMonday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMonday (date)](#apidoc.element.d3.utcMonday.utcMonday)
1.  [function <span class="apidocSignatureSpan">d3.utcMonday.</span>ceil (date)](#apidoc.element.d3.utcMonday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcMonday.</span>count (start, end)](#apidoc.element.d3.utcMonday.count)
1.  [function <span class="apidocSignatureSpan">d3.utcMonday.</span>every (step)](#apidoc.element.d3.utcMonday.every)
1.  [function <span class="apidocSignatureSpan">d3.utcMonday.</span>filter (test)](#apidoc.element.d3.utcMonday.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcMonday.</span>floor (date)](#apidoc.element.d3.utcMonday.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcMonday.</span>offset (date, step)](#apidoc.element.d3.utcMonday.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcMonday.</span>range (start, stop, step)](#apidoc.element.d3.utcMonday.range)
1.  [function <span class="apidocSignatureSpan">d3.utcMonday.</span>round (date)](#apidoc.element.d3.utcMonday.round)

#### [module d3.utcMonth](#apidoc.module.d3.utcMonth)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcMonth (date)](#apidoc.element.d3.utcMonth.utcMonth)
1.  [function <span class="apidocSignatureSpan">d3.utcMonth.</span>ceil (date)](#apidoc.element.d3.utcMonth.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcMonth.</span>count (start, end)](#apidoc.element.d3.utcMonth.count)
1.  [function <span class="apidocSignatureSpan">d3.utcMonth.</span>every (step)](#apidoc.element.d3.utcMonth.every)
1.  [function <span class="apidocSignatureSpan">d3.utcMonth.</span>filter (test)](#apidoc.element.d3.utcMonth.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcMonth.</span>floor (date)](#apidoc.element.d3.utcMonth.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcMonth.</span>offset (date, step)](#apidoc.element.d3.utcMonth.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcMonth.</span>range (start, stop, step)](#apidoc.element.d3.utcMonth.range)
1.  [function <span class="apidocSignatureSpan">d3.utcMonth.</span>round (date)](#apidoc.element.d3.utcMonth.round)

#### [module d3.utcSaturday](#apidoc.module.d3.utcSaturday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcSaturday (date)](#apidoc.element.d3.utcSaturday.utcSaturday)
1.  [function <span class="apidocSignatureSpan">d3.utcSaturday.</span>ceil (date)](#apidoc.element.d3.utcSaturday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcSaturday.</span>count (start, end)](#apidoc.element.d3.utcSaturday.count)
1.  [function <span class="apidocSignatureSpan">d3.utcSaturday.</span>every (step)](#apidoc.element.d3.utcSaturday.every)
1.  [function <span class="apidocSignatureSpan">d3.utcSaturday.</span>filter (test)](#apidoc.element.d3.utcSaturday.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcSaturday.</span>floor (date)](#apidoc.element.d3.utcSaturday.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcSaturday.</span>offset (date, step)](#apidoc.element.d3.utcSaturday.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcSaturday.</span>range (start, stop, step)](#apidoc.element.d3.utcSaturday.range)
1.  [function <span class="apidocSignatureSpan">d3.utcSaturday.</span>round (date)](#apidoc.element.d3.utcSaturday.round)

#### [module d3.utcThursday](#apidoc.module.d3.utcThursday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcThursday (date)](#apidoc.element.d3.utcThursday.utcThursday)
1.  [function <span class="apidocSignatureSpan">d3.utcThursday.</span>ceil (date)](#apidoc.element.d3.utcThursday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcThursday.</span>count (start, end)](#apidoc.element.d3.utcThursday.count)
1.  [function <span class="apidocSignatureSpan">d3.utcThursday.</span>every (step)](#apidoc.element.d3.utcThursday.every)
1.  [function <span class="apidocSignatureSpan">d3.utcThursday.</span>filter (test)](#apidoc.element.d3.utcThursday.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcThursday.</span>floor (date)](#apidoc.element.d3.utcThursday.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcThursday.</span>offset (date, step)](#apidoc.element.d3.utcThursday.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcThursday.</span>range (start, stop, step)](#apidoc.element.d3.utcThursday.range)
1.  [function <span class="apidocSignatureSpan">d3.utcThursday.</span>round (date)](#apidoc.element.d3.utcThursday.round)

#### [module d3.utcTuesday](#apidoc.module.d3.utcTuesday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcTuesday (date)](#apidoc.element.d3.utcTuesday.utcTuesday)
1.  [function <span class="apidocSignatureSpan">d3.utcTuesday.</span>ceil (date)](#apidoc.element.d3.utcTuesday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcTuesday.</span>count (start, end)](#apidoc.element.d3.utcTuesday.count)
1.  [function <span class="apidocSignatureSpan">d3.utcTuesday.</span>every (step)](#apidoc.element.d3.utcTuesday.every)
1.  [function <span class="apidocSignatureSpan">d3.utcTuesday.</span>filter (test)](#apidoc.element.d3.utcTuesday.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcTuesday.</span>floor (date)](#apidoc.element.d3.utcTuesday.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcTuesday.</span>offset (date, step)](#apidoc.element.d3.utcTuesday.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcTuesday.</span>range (start, stop, step)](#apidoc.element.d3.utcTuesday.range)
1.  [function <span class="apidocSignatureSpan">d3.utcTuesday.</span>round (date)](#apidoc.element.d3.utcTuesday.round)

#### [module d3.utcWednesday](#apidoc.module.d3.utcWednesday)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcWednesday (date)](#apidoc.element.d3.utcWednesday.utcWednesday)
1.  [function <span class="apidocSignatureSpan">d3.utcWednesday.</span>ceil (date)](#apidoc.element.d3.utcWednesday.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcWednesday.</span>count (start, end)](#apidoc.element.d3.utcWednesday.count)
1.  [function <span class="apidocSignatureSpan">d3.utcWednesday.</span>every (step)](#apidoc.element.d3.utcWednesday.every)
1.  [function <span class="apidocSignatureSpan">d3.utcWednesday.</span>filter (test)](#apidoc.element.d3.utcWednesday.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcWednesday.</span>floor (date)](#apidoc.element.d3.utcWednesday.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcWednesday.</span>offset (date, step)](#apidoc.element.d3.utcWednesday.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcWednesday.</span>range (start, stop, step)](#apidoc.element.d3.utcWednesday.range)
1.  [function <span class="apidocSignatureSpan">d3.utcWednesday.</span>round (date)](#apidoc.element.d3.utcWednesday.round)

#### [module d3.utcWeek](#apidoc.module.d3.utcWeek)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcWeek (date)](#apidoc.element.d3.utcWeek.utcWeek)
1.  [function <span class="apidocSignatureSpan">d3.utcWeek.</span>ceil (date)](#apidoc.element.d3.utcWeek.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcWeek.</span>count (start, end)](#apidoc.element.d3.utcWeek.count)
1.  [function <span class="apidocSignatureSpan">d3.utcWeek.</span>every (step)](#apidoc.element.d3.utcWeek.every)
1.  [function <span class="apidocSignatureSpan">d3.utcWeek.</span>filter (test)](#apidoc.element.d3.utcWeek.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcWeek.</span>floor (date)](#apidoc.element.d3.utcWeek.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcWeek.</span>offset (date, step)](#apidoc.element.d3.utcWeek.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcWeek.</span>range (start, stop, step)](#apidoc.element.d3.utcWeek.range)
1.  [function <span class="apidocSignatureSpan">d3.utcWeek.</span>round (date)](#apidoc.element.d3.utcWeek.round)

#### [module d3.utcYear](#apidoc.module.d3.utcYear)
1.  [function <span class="apidocSignatureSpan">d3.</span>utcYear (date)](#apidoc.element.d3.utcYear.utcYear)
1.  [function <span class="apidocSignatureSpan">d3.utcYear.</span>ceil (date)](#apidoc.element.d3.utcYear.ceil)
1.  [function <span class="apidocSignatureSpan">d3.utcYear.</span>count (start, end)](#apidoc.element.d3.utcYear.count)
1.  [function <span class="apidocSignatureSpan">d3.utcYear.</span>every (k)](#apidoc.element.d3.utcYear.every)
1.  [function <span class="apidocSignatureSpan">d3.utcYear.</span>filter (test)](#apidoc.element.d3.utcYear.filter)
1.  [function <span class="apidocSignatureSpan">d3.utcYear.</span>floor (date)](#apidoc.element.d3.utcYear.floor)
1.  [function <span class="apidocSignatureSpan">d3.utcYear.</span>offset (date, step)](#apidoc.element.d3.utcYear.offset)
1.  [function <span class="apidocSignatureSpan">d3.utcYear.</span>range (start, stop, step)](#apidoc.element.d3.utcYear.range)
1.  [function <span class="apidocSignatureSpan">d3.utcYear.</span>round (date)](#apidoc.element.d3.utcYear.round)

#### [module d3.zoomTransform](#apidoc.module.d3.zoomTransform)
1.  [function <span class="apidocSignatureSpan">d3.</span>zoomTransform (node)](#apidoc.element.d3.zoomTransform.zoomTransform)

#### [module d3.zoomTransform.prototype](#apidoc.module.d3.zoomTransform.prototype)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>apply (point)](#apidoc.element.d3.zoomTransform.prototype.apply)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>applyX (x)](#apidoc.element.d3.zoomTransform.prototype.applyX)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>applyY (y)](#apidoc.element.d3.zoomTransform.prototype.applyY)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>constructor (k, x, y)](#apidoc.element.d3.zoomTransform.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>invert (location)](#apidoc.element.d3.zoomTransform.prototype.invert)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>invertX (x)](#apidoc.element.d3.zoomTransform.prototype.invertX)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>invertY (y)](#apidoc.element.d3.zoomTransform.prototype.invertY)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>rescaleX (x)](#apidoc.element.d3.zoomTransform.prototype.rescaleX)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>rescaleY (y)](#apidoc.element.d3.zoomTransform.prototype.rescaleY)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>scale (k)](#apidoc.element.d3.zoomTransform.prototype.scale)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>toString ()](#apidoc.element.d3.zoomTransform.prototype.toString)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>translate (x, y)](#apidoc.element.d3.zoomTransform.prototype.translate)

#### [module d3.zoomTransform.prototype.constructor](#apidoc.module.d3.zoomTransform.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>constructor ()](#apidoc.element.d3.zoomTransform.prototype.constructor.constructor)



# <a name="apidoc.module.d3"></a>[module d3](#apidoc.module.d3)

#### <a name="apidoc.element.d3.active"></a>[function <span class="apidocSignatureSpan">d3.</span>active (node, name)](#apidoc.element.d3.active)
- description and source-code
```javascript
active = function (node, name) {
  var schedules = node.__transition,
      schedule,
      i;

  if (schedules) {
    name = name == null ? null : name + "";
    for (i in schedules) {
      if ((schedule = schedules[i]).state > SCHEDULED && schedule.name === name) {
        return new Transition([[node]], root, name, +i);
      }
    }
  }

  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.arc"></a>[function <span class="apidocSignatureSpan">d3.</span>arc ()](#apidoc.element.d3.arc)
- description and source-code
```javascript
arc = function () {
  var innerRadius = arcInnerRadius,
      outerRadius = arcOuterRadius,
      cornerRadius = constant(0),
      padRadius = null,
      startAngle = arcStartAngle,
      endAngle = arcEndAngle,
      padAngle = arcPadAngle,
      context = null;

  function arc() {
    var buffer,
        r,
        r0 = +innerRadius.apply(this, arguments),
        r1 = +outerRadius.apply(this, arguments),
        a0 = startAngle.apply(this, arguments) - halfPi,
        a1 = endAngle.apply(this, arguments) - halfPi,
        da = abs(a1 - a0),
        cw = a1 > a0;

    if (!context) context = buffer = d3Path.path();

    // Ensure that the outer radius is always larger than the inner radius.
    if (r1 < r0) r = r1, r1 = r0, r0 = r;

    // Is it a point?
    if (!(r1 > epsilon)) context.moveTo(0, 0);

    // Or is it a circle or annulus?
    else if (da > tau - epsilon) {
      context.moveTo(r1 * cos(a0), r1 * sin(a0));
      context.arc(0, 0, r1, a0, a1, !cw);
      if (r0 > epsilon) {
        context.moveTo(r0 * cos(a1), r0 * sin(a1));
        context.arc(0, 0, r0, a1, a0, cw);
      }
    }

    // Or is it a circular or annular sector?
    else {
      var a01 = a0,
          a11 = a1,
          a00 = a0,
          a10 = a1,
          da0 = da,
          da1 = da,
          ap = padAngle.apply(this, arguments) / 2,
          rp = (ap > epsilon) && (padRadius ? +padRadius.apply(this, arguments) : sqrt(r0 * r0 + r1 * r1)),
          rc = min(abs(r1 - r0) / 2, +cornerRadius.apply(this, arguments)),
          rc0 = rc,
          rc1 = rc,
          t0,
          t1;

      // Apply padding? Note that since r1 ≥ r0, da1 ≥ da0.
      if (rp > epsilon) {
        var p0 = asin(rp / r0 * sin(ap)),
            p1 = asin(rp / r1 * sin(ap));
        if ((da0 -= p0 * 2) > epsilon) p0 *= (cw ? 1 : -1), a00 += p0, a10 -= p0;
        else da0 = 0, a00 = a10 = (a0 + a1) / 2;
        if ((da1 -= p1 * 2) > epsilon) p1 *= (cw ? 1 : -1), a01 += p1, a11 -= p1;
        else da1 = 0, a01 = a11 = (a0 + a1) / 2;
      }

      var x01 = r1 * cos(a01),
          y01 = r1 * sin(a01),
          x10 = r0 * cos(a10),
          y10 = r0 * sin(a10);

      // Apply rounded corners?
      if (rc > epsilon) {
        var x11 = r1 * cos(a11),
            y11 = r1 * sin(a11),
            x00 = r0 * cos(a00),
            y00 = r0 * sin(a00);

        // Restrict the corner radius according to the sector angle.
        if (da < pi) {
          var oc = da0 > epsilon ? intersect(x01, y01, x00, y00, x11, y11, x10, y10) : [x10, y10],
              ax = x01 - oc[0],
              ay = y01 - oc[1],
              bx = x11 - oc[0],
              by = y11 - oc[1],
              kc = 1 / sin(acos((ax * bx + ay * by) / (sqrt(ax * ax + ay * ay) * sqrt(bx * bx + by * by))) / 2),
              lc = sqrt(oc[0] * oc[0] + oc[1] * oc[1]);
          rc0 = min(rc, (r0 - lc) / (kc - 1));
          rc1 = min(rc, (r1 - lc) / (kc + 1));
        }
      }

      // Is the sector collapsed to a line?
      if (!(da1 > epsilon)) context.moveTo(x01, y01);

      // Does the sector’s outer ring have rounded corners?
      else if (rc1 > epsilon) {
        t0 = cornerTangents(x00, y00, x01, y01, r1, rc1, cw);
        t1 = cornerTangents(x11, y11, x10, y10, r1, rc1, cw);

        context.moveTo(t0.cx + t0.x01, t0.cy + t0.y01);

        // Have the corners merged?
        if (rc1 < rc) context.arc(t0.cx, t0.cy, rc1, atan2(t0.y01, t0.x01), atan2(t1.y01, t1.x01), !cw);

        // Otherwise, draw the two corners and the ring.
        else {
          context.arc(t0.cx, t0.cy, rc1, atan2(t0.y01, t0.x01), atan2(t0.y11, t0.x11), !cw);
          context.arc(0, 0, r1, atan2(t0.cy + t0.y11, t0.cx + t0.x11), atan2(t1.cy + t1.y11, t1.cx + t1.x11), !cw);
          context.arc(t1.cx, t1.cy, rc1, atan2(t1.y11, t1.x11), atan2(t1.y01, t1.x01), !cw);
        }
      }

      // Or is the outer ring just a circular arc?
      else context.moveTo(x01, y01), context.arc(0, 0, r1, a01, a11, !cw);

      // Is there no inner ring, and it’s a circular sector?
      // Or perhaps it’s an annular sector collap ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.area"></a>[function <span class="apidocSignatureSpan">d3.</span>area ()](#apidoc.element.d3.area)
- description and source-code
```javascript
area = function () {
  var x0 = x,
      x1 = null,
      y0 = constant(0),
      y1 = y,
      defined = constant(true),
      context = null,
      curve = curveLinear,
      output = null;

  function area(data) {
    var i,
        j,
        k,
        n = data.length,
        d,
        defined0 = false,
        buffer,
        x0z = new Array(n),
        y0z = new Array(n);

    if (context == null) output = curve(buffer = d3Path.path());

    for (i = 0; i <= n; ++i) {
      if (!(i < n && defined(d = data[i], i, data)) === defined0) {
        if (defined0 = !defined0) {
          j = i;
          output.areaStart();
          output.lineStart();
        } else {
          output.lineEnd();
          output.lineStart();
          for (k = i - 1; k >= j; --k) {
            output.point(x0z[k], y0z[k]);
          }
          output.lineEnd();
          output.areaEnd();
        }
      }
      if (defined0) {
        x0z[i] = +x0(d, i, data), y0z[i] = +y0(d, i, data);
        output.point(x1 ? +x1(d, i, data) : x0z[i], y1 ? +y1(d, i, data) : y0z[i]);
      }
    }

    if (buffer) return output = null, buffer + "" || null;
  }

  function arealine() {
    return line().defined(defined).curve(curve).context(context);
  }

  area.x = function(_) {
    return arguments.length ? (x0 = typeof _ === "function" ? _ : constant(+_), x1 = null, area) : x0;
  };

  area.x0 = function(_) {
    return arguments.length ? (x0 = typeof _ === "function" ? _ : constant(+_), area) : x0;
  };

  area.x1 = function(_) {
    return arguments.length ? (x1 = _ == null ? null : typeof _ === "function" ? _ : constant(+_), area) : x1;
  };

  area.y = function(_) {
    return arguments.length ? (y0 = typeof _ === "function" ? _ : constant(+_), y1 = null, area) : y0;
  };

  area.y0 = function(_) {
    return arguments.length ? (y0 = typeof _ === "function" ? _ : constant(+_), area) : y0;
  };

  area.y1 = function(_) {
    return arguments.length ? (y1 = _ == null ? null : typeof _ === "function" ? _ : constant(+_), area) : y1;
  };

  area.lineX0 =
  area.lineY0 = function() {
    return arealine().x(x0).y(y0);
  };

  area.lineY1 = function() {
    return arealine().x(x0).y(y1);
  };

  area.lineX1 = function() {
    return arealine().x(x1).y(y0);
  };

  area.defined = function(_) {
    return arguments.length ? (defined = typeof _ === "function" ? _ : constant(!!_), area) : defined;
  };

  area.curve = function(_) {
    return arguments.length ? (curve = _, context != null && (output = curve(context)), area) : curve;
  };

  area.context = function(_) {
    return arguments.length ? (_ == null ? context = output = null : output = curve(context = _), area) : context;
  };

  return area;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.ascending"></a>[function <span class="apidocSignatureSpan">d3.</span>ascending (a, b)](#apidoc.element.d3.ascending)
- description and source-code
```javascript
ascending = function (a, b) {
  return a < b ? -1 : a > b ? 1 : a >= b ? 0 : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.axisBottom"></a>[function <span class="apidocSignatureSpan">d3.</span>axisBottom (scale)](#apidoc.element.d3.axisBottom)
- description and source-code
```javascript
function axisBottom(scale) {
  return axis(bottom, scale);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.axisLeft"></a>[function <span class="apidocSignatureSpan">d3.</span>axisLeft (scale)](#apidoc.element.d3.axisLeft)
- description and source-code
```javascript
function axisLeft(scale) {
  return axis(left, scale);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.axisRight"></a>[function <span class="apidocSignatureSpan">d3.</span>axisRight (scale)](#apidoc.element.d3.axisRight)
- description and source-code
```javascript
function axisRight(scale) {
  return axis(right, scale);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.axisTop"></a>[function <span class="apidocSignatureSpan">d3.</span>axisTop (scale)](#apidoc.element.d3.axisTop)
- description and source-code
```javascript
function axisTop(scale) {
  return axis(top, scale);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.bisect"></a>[function <span class="apidocSignatureSpan">d3.</span>bisect (a, x, lo, hi)](#apidoc.element.d3.bisect)
- description and source-code
```javascript
bisect = function (a, x, lo, hi) {
  if (lo == null) lo = 0;
  if (hi == null) hi = a.length;
  while (lo < hi) {
    var mid = lo + hi >>> 1;
    if (compare(a[mid], x) > 0) hi = mid;
    else lo = mid + 1;
  }
  return lo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.bisectLeft"></a>[function <span class="apidocSignatureSpan">d3.</span>bisectLeft (a, x, lo, hi)](#apidoc.element.d3.bisectLeft)
- description and source-code
```javascript
bisectLeft = function (a, x, lo, hi) {
  if (lo == null) lo = 0;
  if (hi == null) hi = a.length;
  while (lo < hi) {
    var mid = lo + hi >>> 1;
    if (compare(a[mid], x) < 0) lo = mid + 1;
    else hi = mid;
  }
  return lo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.bisectRight"></a>[function <span class="apidocSignatureSpan">d3.</span>bisectRight (a, x, lo, hi)](#apidoc.element.d3.bisectRight)
- description and source-code
```javascript
bisectRight = function (a, x, lo, hi) {
  if (lo == null) lo = 0;
  if (hi == null) hi = a.length;
  while (lo < hi) {
    var mid = lo + hi >>> 1;
    if (compare(a[mid], x) > 0) hi = mid;
    else lo = mid + 1;
  }
  return lo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.bisector"></a>[function <span class="apidocSignatureSpan">d3.</span>bisector (compare)](#apidoc.element.d3.bisector)
- description and source-code
```javascript
bisector = function (compare) {
  if (compare.length === 1) compare = ascendingComparator(compare);
  return {
    left: function(a, x, lo, hi) {
      if (lo == null) lo = 0;
      if (hi == null) hi = a.length;
      while (lo < hi) {
        var mid = lo + hi >>> 1;
        if (compare(a[mid], x) < 0) lo = mid + 1;
        else hi = mid;
      }
      return lo;
    },
    right: function(a, x, lo, hi) {
      if (lo == null) lo = 0;
      if (hi == null) hi = a.length;
      while (lo < hi) {
        var mid = lo + hi >>> 1;
        if (compare(a[mid], x) > 0) hi = mid;
        else lo = mid + 1;
      }
      return lo;
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.brush"></a>[function <span class="apidocSignatureSpan">d3.</span>brush ()](#apidoc.element.d3.brush)
- description and source-code
```javascript
brush = function () {
  return brush$1(XY);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.brushSelection"></a>[function <span class="apidocSignatureSpan">d3.</span>brushSelection (node)](#apidoc.element.d3.brushSelection)
- description and source-code
```javascript
function brushSelection(node) {
  var state = node.__brush;
  return state ? state.dim.output(state.selection) : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.brushX"></a>[function <span class="apidocSignatureSpan">d3.</span>brushX ()](#apidoc.element.d3.brushX)
- description and source-code
```javascript
function brushX() {
  return brush$1(X);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.brushY"></a>[function <span class="apidocSignatureSpan">d3.</span>brushY ()](#apidoc.element.d3.brushY)
- description and source-code
```javascript
function brushY() {
  return brush$1(Y);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.chord"></a>[function <span class="apidocSignatureSpan">d3.</span>chord ()](#apidoc.element.d3.chord)
- description and source-code
```javascript
chord = function () {
  var padAngle = 0,
      sortGroups = null,
      sortSubgroups = null,
      sortChords = null;

  function chord(matrix) {
    var n = matrix.length,
        groupSums = [],
        groupIndex = d3Array.range(n),
        subgroupIndex = [],
        chords = [],
        groups = chords.groups = new Array(n),
        subgroups = new Array(n * n),
        k,
        x,
        x0,
        dx,
        i,
        j;

    // Compute the sum.
    k = 0, i = -1; while (++i < n) {
      x = 0, j = -1; while (++j < n) {
        x += matrix[i][j];
      }
      groupSums.push(x);
      subgroupIndex.push(d3Array.range(n));
      k += x;
    }

    // Sort groups…
    if (sortGroups) groupIndex.sort(function(a, b) {
      return sortGroups(groupSums[a], groupSums[b]);
    });

    // Sort subgroups…
    if (sortSubgroups) subgroupIndex.forEach(function(d, i) {
      d.sort(function(a, b) {
        return sortSubgroups(matrix[i][a], matrix[i][b]);
      });
    });

    // Convert the sum to scaling factor for [0, 2pi].
    // TODO Allow start and end angle to be specified?
    // TODO Allow padding to be specified as percentage?
    k = max(0, tau - padAngle * n) / k;
    dx = k ? padAngle : tau / n;

    // Compute the start and end angle for each group and subgroup.
    // Note: Opera has a bug reordering object literal properties!
    x = 0, i = -1; while (++i < n) {
      x0 = x, j = -1; while (++j < n) {
        var di = groupIndex[i],
            dj = subgroupIndex[di][j],
            v = matrix[di][dj],
            a0 = x,
            a1 = x += v * k;
        subgroups[dj * n + di] = {
          index: di,
          subindex: dj,
          startAngle: a0,
          endAngle: a1,
          value: v
        };
      }
      groups[di] = {
        index: di,
        startAngle: x0,
        endAngle: x,
        value: groupSums[di]
      };
      x += dx;
    }

    // Generate chords for each (non-empty) subgroup-subgroup link.
    i = -1; while (++i < n) {
      j = i - 1; while (++j < n) {
        var source = subgroups[j * n + i],
            target = subgroups[i * n + j];
        if (source.value || target.value) {
          chords.push(source.value < target.value
              ? {source: target, target: source}
              : {source: source, target: target});
        }
      }
    }

    return sortChords ? chords.sort(sortChords) : chords;
  }

  chord.padAngle = function(_) {
    return arguments.length ? (padAngle = max(0, _), chord) : padAngle;
  };

  chord.sortGroups = function(_) {
    return arguments.length ? (sortGroups = _, chord) : sortGroups;
  };

  chord.sortSubgroups = function(_) {
    return arguments.length ? (sortSubgroups = _, chord) : sortSubgroups;
  };

  chord.sortChords = function(_) {
    return arguments.length ? (_ == null ? sortChords = null : (sortChords = compareValue(_))._ = _, chord) : sortChords && sortChords
._;
  };

  return chord;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.cluster"></a>[function <span class="apidocSignatureSpan">d3.</span>cluster ()](#apidoc.element.d3.cluster)
- description and source-code
```javascript
cluster = function () {
  var separation = defaultSeparation,
      dx = 1,
      dy = 1,
      nodeSize = false;

  function cluster(root) {
    var previousNode,
        x = 0;

    // First walk, computing the initial x & y values.
    root.eachAfter(function(node) {
      var children = node.children;
      if (children) {
        node.x = meanX(children);
        node.y = maxY(children);
      } else {
        node.x = previousNode ? x += separation(node, previousNode) : 0;
        node.y = 0;
        previousNode = node;
      }
    });

    var left = leafLeft(root),
        right = leafRight(root),
        x0 = left.x - separation(left, right) / 2,
        x1 = right.x + separation(right, left) / 2;

    // Second walk, normalizing x & y to the desired size.
    return root.eachAfter(nodeSize ? function(node) {
      node.x = (node.x - root.x) * dx;
      node.y = (root.y - node.y) * dy;
    } : function(node) {
      node.x = (node.x - x0) / (x1 - x0) * dx;
      node.y = (1 - (root.y ? node.y / root.y : 1)) * dy;
    });
  }

  cluster.separation = function(x) {
    return arguments.length ? (separation = x, cluster) : separation;
  };

  cluster.size = function(x) {
    return arguments.length ? (nodeSize = false, dx = +x[0], dy = +x[1], cluster) : (nodeSize ? null : [dx, dy]);
  };

  cluster.nodeSize = function(x) {
    return arguments.length ? (nodeSize = true, dx = +x[0], dy = +x[1], cluster) : (nodeSize ? [dx, dy] : null);
  };

  return cluster;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.color"></a>[function <span class="apidocSignatureSpan">d3.</span>color (format)](#apidoc.element.d3.color)
- description and source-code
```javascript
function color(format) {
  var m;
  format = (format + "").trim().toLowerCase();
  return (m = reHex3.exec(format)) ? (m = parseInt(m[1], 16), new Rgb((m >> 8 & 0xf) | (m >> 4 & 0x0f0), (m >> 4 & 0xf) | (m & 0xf0
), ((m & 0xf) << 4) | (m & 0xf), 1)) // #f00
      : (m = reHex6.exec(format)) ? rgbn(parseInt(m[1], 16)) // #ff0000
      : (m = reRgbInteger.exec(format)) ? new Rgb(m[1], m[2], m[3], 1) // rgb(255, 0, 0)
      : (m = reRgbPercent.exec(format)) ? new Rgb(m[1] * 255 / 100, m[2] * 255 / 100, m[3] * 255 / 100, 1) // rgb(100%, 0%, 0%)
      : (m = reRgbaInteger.exec(format)) ? rgba(m[1], m[2], m[3], m[4]) // rgba(255, 0, 0, 1)
      : (m = reRgbaPercent.exec(format)) ? rgba(m[1] * 255 / 100, m[2] * 255 / 100, m[3] * 255 / 100, m[4]) // rgb(100%, 0%, 0%,
1)
      : (m = reHslPercent.exec(format)) ? hsla(m[1], m[2] / 100, m[3] / 100, 1) // hsl(120, 50%, 50%)
      : (m = reHslaPercent.exec(format)) ? hsla(m[1], m[2] / 100, m[3] / 100, m[4]) // hsla(120, 50%, 50%, 1)
      : named.hasOwnProperty(format) ? rgbn(named[format])
      : format === "transparent" ? new Rgb(NaN, NaN, NaN, 0)
      : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.color.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>color.prototype.constructor ()](#apidoc.element.d3.color.prototype.constructor)
- description and source-code
```javascript
function Color() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.creator"></a>[function <span class="apidocSignatureSpan">d3.</span>creator (name)](#apidoc.element.d3.creator)
- description and source-code
```javascript
creator = function (name) {
  var fullname = namespace(name);
  return (fullname.local
      ? creatorFixed
      : creatorInherit)(fullname);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.cross"></a>[function <span class="apidocSignatureSpan">d3.</span>cross (a, b, f)](#apidoc.element.d3.cross)
- description and source-code
```javascript
cross = function (a, b, f) {
  var na = a.length, nb = b.length, c = new Array(na * nb), ia, ib, ic, va;
  if (f == null) f = pair;
  for (ia = ic = 0; ia < na; ++ia) for (va = a[ia], ib = 0; ib < nb; ++ib, ++ic) c[ic] = f(va, b[ib]);
  return c;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.csv"></a>[function <span class="apidocSignatureSpan">d3.</span>csv (url, row, callback)](#apidoc.element.d3.csv)
- description and source-code
```javascript
csv = function (url, row, callback) {
  if (arguments.length < 3) callback = row, row = null;
  var r = request(url).mimeType(defaultMimeType);
  r.row = function(_) { return arguments.length ? r.response(responseOf(parse, row = _)) : row; };
  r.row(row);
  return callback ? r.get(callback) : r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.csvFormat"></a>[function <span class="apidocSignatureSpan">d3.</span>csvFormat (rows, columns)](#apidoc.element.d3.csvFormat)
- description and source-code
```javascript
function format(rows, columns) {
  if (columns == null) columns = inferColumns(rows);
  return [columns.map(formatValue).join(delimiter)].concat(rows.map(function(row) {
    return columns.map(function(column) {
      return formatValue(row[column]);
    }).join(delimiter);
  })).join("\n");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.csvFormatRows"></a>[function <span class="apidocSignatureSpan">d3.</span>csvFormatRows (rows)](#apidoc.element.d3.csvFormatRows)
- description and source-code
```javascript
function formatRows(rows) {
  return rows.map(formatRow).join("\n");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.csvParse"></a>[function <span class="apidocSignatureSpan">d3.</span>csvParse (text, f)](#apidoc.element.d3.csvParse)
- description and source-code
```javascript
function parse(text, f) {
  var convert, columns, rows = parseRows(text, function(row, i) {
    if (convert) return convert(row, i - 1);
    columns = row, convert = f ? customConverter(row, f) : objectConverter(row);
  });
  rows.columns = columns;
  return rows;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.csvParseRows"></a>[function <span class="apidocSignatureSpan">d3.</span>csvParseRows (text, f)](#apidoc.element.d3.csvParseRows)
- description and source-code
```javascript
function parseRows(text, f) {
  var EOL = {}, // sentinel value for end-of-line
      EOF = {}, // sentinel value for end-of-file
      rows = [], // output rows
      N = text.length,
      I = 0, // current character index
      n = 0, // the current line number
      t, // the current token
      eol; // is the current token followed by EOL?

  function token() {
    if (I >= N) return EOF; // special case: end of file
    if (eol) return eol = false, EOL; // special case: end of line

    // special case: quotes
    var j = I, c;
    if (text.charCodeAt(j) === 34) {
      var i = j;
      while (i++ < N) {
        if (text.charCodeAt(i) === 34) {
          if (text.charCodeAt(i + 1) !== 34) break;
          ++i;
        }
      }
      I = i + 2;
      c = text.charCodeAt(i + 1);
      if (c === 13) {
        eol = true;
        if (text.charCodeAt(i + 2) === 10) ++I;
      } else if (c === 10) {
        eol = true;
      }
      return text.slice(j + 1, i).replace(/""/g, "\"");
    }

    // common case: find next delimiter or newline
    while (I < N) {
      var k = 1;
      c = text.charCodeAt(I++);
      if (c === 10) eol = true; // \n
      else if (c === 13) { eol = true; if (text.charCodeAt(I) === 10) ++I, ++k; } // \r|\r\n
      else if (c !== delimiterCode) continue;
      return text.slice(j, I - k);
    }

    // special case: last token before EOF
    return text.slice(j);
  }

  while ((t = token()) !== EOF) {
    var a = [];
    while (t !== EOL && t !== EOF) {
      a.push(t);
      t = token();
    }
    if (f && (a = f(a, n++)) == null) continue;
    rows.push(a);
  }

  return rows;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.cubehelix"></a>[function <span class="apidocSignatureSpan">d3.</span>cubehelix (h, s, l, opacity)](#apidoc.element.d3.cubehelix)
- description and source-code
```javascript
function cubehelix(h, s, l, opacity) {
  return arguments.length === 1 ? cubehelixConvert(h) : new Cubehelix(h, s, l, opacity == null ? 1 : opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.cubehelix.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>cubehelix.prototype.constructor (h, s, l, opacity)](#apidoc.element.d3.cubehelix.prototype.constructor)
- description and source-code
```javascript
function Cubehelix(h, s, l, opacity) {
  this.h = +h;
  this.s = +s;
  this.l = +l;
  this.opacity = +opacity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveBasis"></a>[function <span class="apidocSignatureSpan">d3.</span>curveBasis (context)](#apidoc.element.d3.curveBasis)
- description and source-code
```javascript
curveBasis = function (context) {
  return new Basis(context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveBasisClosed"></a>[function <span class="apidocSignatureSpan">d3.</span>curveBasisClosed (context)](#apidoc.element.d3.curveBasisClosed)
- description and source-code
```javascript
curveBasisClosed = function (context) {
  return new BasisClosed(context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveBasisOpen"></a>[function <span class="apidocSignatureSpan">d3.</span>curveBasisOpen (context)](#apidoc.element.d3.curveBasisOpen)
- description and source-code
```javascript
curveBasisOpen = function (context) {
  return new BasisOpen(context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveBundle"></a>[function <span class="apidocSignatureSpan">d3.</span>curveBundle (context)](#apidoc.element.d3.curveBundle)
- description and source-code
```javascript
function bundle(context) {
  return beta === 1 ? new Basis(context) : new Bundle(context, beta);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCardinal"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCardinal (context)](#apidoc.element.d3.curveCardinal)
- description and source-code
```javascript
function cardinal(context) {
  return new Cardinal(context, tension);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCardinalClosed"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCardinalClosed (context)](#apidoc.element.d3.curveCardinalClosed)
- description and source-code
```javascript
function cardinal(context) {
  return new CardinalClosed(context, tension);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCardinalOpen"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCardinalOpen (context)](#apidoc.element.d3.curveCardinalOpen)
- description and source-code
```javascript
function cardinal(context) {
  return new CardinalOpen(context, tension);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCatmullRom"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCatmullRom (context)](#apidoc.element.d3.curveCatmullRom)
- description and source-code
```javascript
function catmullRom(context) {
  return alpha ? new CatmullRom(context, alpha) : new Cardinal(context, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCatmullRomClosed"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCatmullRomClosed (context)](#apidoc.element.d3.curveCatmullRomClosed)
- description and source-code
```javascript
function catmullRom(context) {
  return alpha ? new CatmullRomClosed(context, alpha) : new CardinalClosed(context, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCatmullRomOpen"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCatmullRomOpen (context)](#apidoc.element.d3.curveCatmullRomOpen)
- description and source-code
```javascript
function catmullRom(context) {
  return alpha ? new CatmullRomOpen(context, alpha) : new CardinalOpen(context, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveLinear"></a>[function <span class="apidocSignatureSpan">d3.</span>curveLinear (context)](#apidoc.element.d3.curveLinear)
- description and source-code
```javascript
curveLinear = function (context) {
  return new Linear(context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveLinearClosed"></a>[function <span class="apidocSignatureSpan">d3.</span>curveLinearClosed (context)](#apidoc.element.d3.curveLinearClosed)
- description and source-code
```javascript
curveLinearClosed = function (context) {
  return new LinearClosed(context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveMonotoneX"></a>[function <span class="apidocSignatureSpan">d3.</span>curveMonotoneX (context)](#apidoc.element.d3.curveMonotoneX)
- description and source-code
```javascript
function monotoneX(context) {
  return new MonotoneX(context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveMonotoneY"></a>[function <span class="apidocSignatureSpan">d3.</span>curveMonotoneY (context)](#apidoc.element.d3.curveMonotoneY)
- description and source-code
```javascript
function monotoneY(context) {
  return new MonotoneY(context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveNatural"></a>[function <span class="apidocSignatureSpan">d3.</span>curveNatural (context)](#apidoc.element.d3.curveNatural)
- description and source-code
```javascript
curveNatural = function (context) {
  return new Natural(context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveStep"></a>[function <span class="apidocSignatureSpan">d3.</span>curveStep (context)](#apidoc.element.d3.curveStep)
- description and source-code
```javascript
curveStep = function (context) {
  return new Step(context, 0.5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveStepAfter"></a>[function <span class="apidocSignatureSpan">d3.</span>curveStepAfter (context)](#apidoc.element.d3.curveStepAfter)
- description and source-code
```javascript
function stepAfter(context) {
  return new Step(context, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveStepBefore"></a>[function <span class="apidocSignatureSpan">d3.</span>curveStepBefore (context)](#apidoc.element.d3.curveStepBefore)
- description and source-code
```javascript
function stepBefore(context) {
  return new Step(context, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.customEvent"></a>[function <span class="apidocSignatureSpan">d3.</span>customEvent (event1, listener, that, args)](#apidoc.element.d3.customEvent)
- description and source-code
```javascript
function customEvent(event1, listener, that, args) {
  var event0 = exports.event;
  event1.sourceEvent = exports.event;
  exports.event = event1;
  try {
    return listener.apply(that, args);
  } finally {
    exports.event = event0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.descending"></a>[function <span class="apidocSignatureSpan">d3.</span>descending (a, b)](#apidoc.element.d3.descending)
- description and source-code
```javascript
descending = function (a, b) {
  return b < a ? -1 : b > a ? 1 : b >= a ? 0 : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.deviation"></a>[function <span class="apidocSignatureSpan">d3.</span>deviation (array, f)](#apidoc.element.d3.deviation)
- description and source-code
```javascript
deviation = function (array, f) {
  var v = variance(array, f);
  return v ? Math.sqrt(v) : v;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.dispatch"></a>[function <span class="apidocSignatureSpan">d3.</span>dispatch ()](#apidoc.element.d3.dispatch)
- description and source-code
```javascript
function dispatch() {
  for (var i = 0, n = arguments.length, _ = {}, t; i < n; ++i) {
    if (!(t = arguments[i] + "") || (t in _)) throw new Error("illegal type: " + t);
    _[t] = [];
  }
  return new Dispatch(_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.dispatch.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>dispatch.prototype.constructor (_)](#apidoc.element.d3.dispatch.prototype.constructor)
- description and source-code
```javascript
function Dispatch(_) {
  this._ = _;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.drag"></a>[function <span class="apidocSignatureSpan">d3.</span>drag ()](#apidoc.element.d3.drag)
- description and source-code
```javascript
drag = function () {
  var filter = defaultFilter,
      container = defaultContainer,
      subject = defaultSubject,
      gestures = {},
      listeners = d3Dispatch.dispatch("start", "drag", "end"),
      active = 0,
      mousemoving,
      touchending;

  function drag(selection) {
    selection
        .on("mousedown.drag", mousedowned)
        .on("touchstart.drag", touchstarted)
        .on("touchmove.drag", touchmoved)
        .on("touchend.drag touchcancel.drag", touchended)
        .style("-webkit-tap-highlight-color", "rgba(0,0,0,0)");
  }

  function mousedowned() {
    if (touchending || !filter.apply(this, arguments)) return;
    var gesture = beforestart("mouse", container.apply(this, arguments), d3Selection.mouse, this, arguments);
    if (!gesture) return;
    d3Selection.select(d3Selection.event.view).on("mousemove.drag", mousemoved, true).on("mouseup.drag", mouseupped, true);
    nodrag(d3Selection.event.view);
    nopropagation();
    mousemoving = false;
    gesture("start");
  }

  function mousemoved() {
    noevent();
    mousemoving = true;
    gestures.mouse("drag");
  }

  function mouseupped() {
    d3Selection.select(d3Selection.event.view).on("mousemove.drag mouseup.drag", null);
    yesdrag(d3Selection.event.view, mousemoving);
    noevent();
    gestures.mouse("end");
  }

  function touchstarted() {
    if (!filter.apply(this, arguments)) return;
    var touches = d3Selection.event.changedTouches,
        c = container.apply(this, arguments),
        n = touches.length, i, gesture;

    for (i = 0; i < n; ++i) {
      if (gesture = beforestart(touches[i].identifier, c, d3Selection.touch, this, arguments)) {
        nopropagation();
        gesture("start");
      }
    }
  }

  function touchmoved() {
    var touches = d3Selection.event.changedTouches,
        n = touches.length, i, gesture;

    for (i = 0; i < n; ++i) {
      if (gesture = gestures[touches[i].identifier]) {
        noevent();
        gesture("drag");
      }
    }
  }

  function touchended() {
    var touches = d3Selection.event.changedTouches,
        n = touches.length, i, gesture;

    if (touchending) clearTimeout(touchending);
    touchending = setTimeout(function() { touchending = null; }, 500); // Ghost clicks are delayed!
    for (i = 0; i < n; ++i) {
      if (gesture = gestures[touches[i].identifier]) {
        nopropagation();
        gesture("end");
      }
    }
  }

  function beforestart(id, container, point, that, args) {
    var p = point(container, id), s, dx, dy,
        sublisteners = listeners.copy();

    if (!d3Selection.customEvent(new DragEvent(drag, "beforestart", s, id, active, p[0], p[1], 0, 0, sublisteners), function() {
      if ((d3Selection.event.subject = s = subject.apply(that, args)) == null) return false;
      dx = s.x - p[0] || 0;
      dy = s.y - p[1] || 0;
      return true;
    })) return;

    return function gesture(type) {
      var p0 = p, n;
      switch (type) {
        case "start": gestures[id] = gesture, n = active++; break;
        case "end": delete gestures[id], --active; // nobreak
        case "drag": p = point(container, id), n = active; break;
      }
      d3Selection.customEvent(new DragEvent(drag, type, s, id, n, p[0] + dx, p[1] + dy, p[0] - p0[0], p[1] - p0[1], sublisteners
), sublisteners.apply, sublisteners, [type, that, args]);
    };
  }

  drag.filter = function(_) {
    return arguments.length ? (filter = typeof _ === "function" ? _ : constant(!!_), drag) : filter;
  };

  drag.container = function(_) {
    return arguments.length ? (container = typeof _ === "function" ? _ : constant(_), drag) : container;
  };

  drag.subject = function(_) {
    return arguments.length ? (subject = typeof _ === "function" ? _ : constant(_), drag) : subject;
  };

  drag.on = function() {
    var value = listeners.on.apply(listeners, arguments);
    return value === listeners ? drag : value;
  };

  return drag;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.dragDisable"></a>[function <span class="apidocSignatureSpan">d3.</span>dragDisable (view)](#apidoc.element.d3.dragDisable)
- description and source-code
```javascript
dragDisable = function (view) {
  var root = view.document.documentElement,
      selection = d3Selection.select(view).on("dragstart.drag", noevent, true);
  if ("onselectstart" in root) {
    selection.on("selectstart.drag", noevent, true);
  } else {
    root.__noselect = root.style.MozUserSelect;
    root.style.MozUserSelect = "none";
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.dragEnable"></a>[function <span class="apidocSignatureSpan">d3.</span>dragEnable (view, noclick)](#apidoc.element.d3.dragEnable)
- description and source-code
```javascript
function yesdrag(view, noclick) {
  var root = view.document.documentElement,
      selection = d3Selection.select(view).on("dragstart.drag", null);
  if (noclick) {
    selection.on("click.drag", noevent, true);
    setTimeout(function() { selection.on("click.drag", null); }, 0);
  }
  if ("onselectstart" in root) {
    selection.on("selectstart.drag", null);
  } else {
    root.style.MozUserSelect = root.__noselect;
    delete root.__noselect;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.dsvFormat"></a>[function <span class="apidocSignatureSpan">d3.</span>dsvFormat (delimiter)](#apidoc.element.d3.dsvFormat)
- description and source-code
```javascript
dsvFormat = function (delimiter) {
  var reFormat = new RegExp("[\"" + delimiter + "\n\r]"),
      delimiterCode = delimiter.charCodeAt(0);

  function parse(text, f) {
    var convert, columns, rows = parseRows(text, function(row, i) {
      if (convert) return convert(row, i - 1);
      columns = row, convert = f ? customConverter(row, f) : objectConverter(row);
    });
    rows.columns = columns;
    return rows;
  }

  function parseRows(text, f) {
    var EOL = {}, // sentinel value for end-of-line
        EOF = {}, // sentinel value for end-of-file
        rows = [], // output rows
        N = text.length,
        I = 0, // current character index
        n = 0, // the current line number
        t, // the current token
        eol; // is the current token followed by EOL?

    function token() {
      if (I >= N) return EOF; // special case: end of file
      if (eol) return eol = false, EOL; // special case: end of line

      // special case: quotes
      var j = I, c;
      if (text.charCodeAt(j) === 34) {
        var i = j;
        while (i++ < N) {
          if (text.charCodeAt(i) === 34) {
            if (text.charCodeAt(i + 1) !== 34) break;
            ++i;
          }
        }
        I = i + 2;
        c = text.charCodeAt(i + 1);
        if (c === 13) {
          eol = true;
          if (text.charCodeAt(i + 2) === 10) ++I;
        } else if (c === 10) {
          eol = true;
        }
        return text.slice(j + 1, i).replace(/""/g, "\"");
      }

      // common case: find next delimiter or newline
      while (I < N) {
        var k = 1;
        c = text.charCodeAt(I++);
        if (c === 10) eol = true; // \n
        else if (c === 13) { eol = true; if (text.charCodeAt(I) === 10) ++I, ++k; } // \r|\r\n
        else if (c !== delimiterCode) continue;
        return text.slice(j, I - k);
      }

      // special case: last token before EOF
      return text.slice(j);
    }

    while ((t = token()) !== EOF) {
      var a = [];
      while (t !== EOL && t !== EOF) {
        a.push(t);
        t = token();
      }
      if (f && (a = f(a, n++)) == null) continue;
      rows.push(a);
    }

    return rows;
  }

  function format(rows, columns) {
    if (columns == null) columns = inferColumns(rows);
    return [columns.map(formatValue).join(delimiter)].concat(rows.map(function(row) {
      return columns.map(function(column) {
        return formatValue(row[column]);
      }).join(delimiter);
    })).join("\n");
  }

  function formatRows(rows) {
    return rows.map(formatRow).join("\n");
  }

  function formatRow(row) {
    return row.map(formatValue).join(delimiter);
  }

  function formatValue(text) {
    return text == null ? ""
        : reFormat.test(text += "") ? "\"" + text.replace(/\"/g, "\"\"") + "\""
        : text;
  }

  return {
    parse: parse,
    parseRows: parseRows,
    format: format,
    formatRows: formatRows
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBack"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBack (t)](#apidoc.element.d3.easeBack)
- description and source-code
```javascript
function backInOut(t) {
  return ((t *= 2) < 1 ? t * t * ((s + 1) * t - s) : (t -= 2) * t * ((s + 1) * t + s) + 2) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBackIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBackIn (t)](#apidoc.element.d3.easeBackIn)
- description and source-code
```javascript
function backIn(t) {
  return t * t * ((s + 1) * t - s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBackInOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBackInOut (t)](#apidoc.element.d3.easeBackInOut)
- description and source-code
```javascript
function backInOut(t) {
  return ((t *= 2) < 1 ? t * t * ((s + 1) * t - s) : (t -= 2) * t * ((s + 1) * t + s) + 2) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBackOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBackOut (t)](#apidoc.element.d3.easeBackOut)
- description and source-code
```javascript
function backOut(t) {
  return --t * t * ((s + 1) * t + s) + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBounce"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBounce (t)](#apidoc.element.d3.easeBounce)
- description and source-code
```javascript
function bounceOut(t) {
  return (t = +t) < b1 ? b0 * t * t : t < b3 ? b0 * (t -= b2) * t + b4 : t < b6 ? b0 * (t -= b5) * t + b7 : b0 * (t -= b8) * t +
b9;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBounceIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBounceIn (t)](#apidoc.element.d3.easeBounceIn)
- description and source-code
```javascript
function bounceIn(t) {
  return 1 - bounceOut(1 - t);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBounceInOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBounceInOut (t)](#apidoc.element.d3.easeBounceInOut)
- description and source-code
```javascript
function bounceInOut(t) {
  return ((t *= 2) <= 1 ? 1 - bounceOut(1 - t) : bounceOut(t - 1) + 1) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBounceOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBounceOut (t)](#apidoc.element.d3.easeBounceOut)
- description and source-code
```javascript
function bounceOut(t) {
  return (t = +t) < b1 ? b0 * t * t : t < b3 ? b0 * (t -= b2) * t + b4 : t < b6 ? b0 * (t -= b5) * t + b7 : b0 * (t -= b8) * t +
b9;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeCircle"></a>[function <span class="apidocSignatureSpan">d3.</span>easeCircle (t)](#apidoc.element.d3.easeCircle)
- description and source-code
```javascript
function circleInOut(t) {
  return ((t *= 2) <= 1 ? 1 - Math.sqrt(1 - t * t) : Math.sqrt(1 - (t -= 2) * t) + 1) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeCircleIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easeCircleIn (t)](#apidoc.element.d3.easeCircleIn)
- description and source-code
```javascript
function circleIn(t) {
  return 1 - Math.sqrt(1 - t * t);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeCircleInOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeCircleInOut (t)](#apidoc.element.d3.easeCircleInOut)
- description and source-code
```javascript
function circleInOut(t) {
  return ((t *= 2) <= 1 ? 1 - Math.sqrt(1 - t * t) : Math.sqrt(1 - (t -= 2) * t) + 1) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeCircleOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeCircleOut (t)](#apidoc.element.d3.easeCircleOut)
- description and source-code
```javascript
function circleOut(t) {
  return Math.sqrt(1 - --t * t);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeCubic"></a>[function <span class="apidocSignatureSpan">d3.</span>easeCubic (t)](#apidoc.element.d3.easeCubic)
- description and source-code
```javascript
function cubicInOut(t) {
  return ((t *= 2) <= 1 ? t * t * t : (t -= 2) * t * t + 2) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeCubicIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easeCubicIn (t)](#apidoc.element.d3.easeCubicIn)
- description and source-code
```javascript
function cubicIn(t) {
  return t * t * t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeCubicInOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeCubicInOut (t)](#apidoc.element.d3.easeCubicInOut)
- description and source-code
```javascript
function cubicInOut(t) {
  return ((t *= 2) <= 1 ? t * t * t : (t -= 2) * t * t + 2) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeCubicOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeCubicOut (t)](#apidoc.element.d3.easeCubicOut)
- description and source-code
```javascript
function cubicOut(t) {
  return --t * t * t + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeElastic"></a>[function <span class="apidocSignatureSpan">d3.</span>easeElastic (t)](#apidoc.element.d3.easeElastic)
- description and source-code
```javascript
function elasticOut(t) {
  return 1 - a * Math.pow(2, -10 * (t = +t)) * Math.sin((t + s) / p);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeElasticIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easeElasticIn (t)](#apidoc.element.d3.easeElasticIn)
- description and source-code
```javascript
function elasticIn(t) {
  return a * Math.pow(2, 10 * --t) * Math.sin((s - t) / p);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeElasticInOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeElasticInOut (t)](#apidoc.element.d3.easeElasticInOut)
- description and source-code
```javascript
function elasticInOut(t) {
  return ((t = t * 2 - 1) < 0
      ? a * Math.pow(2, 10 * t) * Math.sin((s - t) / p)
      : 2 - a * Math.pow(2, -10 * t) * Math.sin((s + t) / p)) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeElasticOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeElasticOut (t)](#apidoc.element.d3.easeElasticOut)
- description and source-code
```javascript
function elasticOut(t) {
  return 1 - a * Math.pow(2, -10 * (t = +t)) * Math.sin((t + s) / p);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeExp"></a>[function <span class="apidocSignatureSpan">d3.</span>easeExp (t)](#apidoc.element.d3.easeExp)
- description and source-code
```javascript
function expInOut(t) {
  return ((t *= 2) <= 1 ? Math.pow(2, 10 * t - 10) : 2 - Math.pow(2, 10 - 10 * t)) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeExpIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easeExpIn (t)](#apidoc.element.d3.easeExpIn)
- description and source-code
```javascript
function expIn(t) {
  return Math.pow(2, 10 * t - 10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeExpInOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeExpInOut (t)](#apidoc.element.d3.easeExpInOut)
- description and source-code
```javascript
function expInOut(t) {
  return ((t *= 2) <= 1 ? Math.pow(2, 10 * t - 10) : 2 - Math.pow(2, 10 - 10 * t)) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeExpOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeExpOut (t)](#apidoc.element.d3.easeExpOut)
- description and source-code
```javascript
function expOut(t) {
  return 1 - Math.pow(2, -10 * t);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeLinear"></a>[function <span class="apidocSignatureSpan">d3.</span>easeLinear (t)](#apidoc.element.d3.easeLinear)
- description and source-code
```javascript
function linear(t) {
  return +t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easePoly"></a>[function <span class="apidocSignatureSpan">d3.</span>easePoly (t)](#apidoc.element.d3.easePoly)
- description and source-code
```javascript
function polyInOut(t) {
  return ((t *= 2) <= 1 ? Math.pow(t, e) : 2 - Math.pow(2 - t, e)) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easePolyIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easePolyIn (t)](#apidoc.element.d3.easePolyIn)
- description and source-code
```javascript
function polyIn(t) {
  return Math.pow(t, e);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easePolyInOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easePolyInOut (t)](#apidoc.element.d3.easePolyInOut)
- description and source-code
```javascript
function polyInOut(t) {
  return ((t *= 2) <= 1 ? Math.pow(t, e) : 2 - Math.pow(2 - t, e)) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easePolyOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easePolyOut (t)](#apidoc.element.d3.easePolyOut)
- description and source-code
```javascript
function polyOut(t) {
  return 1 - Math.pow(1 - t, e);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeQuad"></a>[function <span class="apidocSignatureSpan">d3.</span>easeQuad (t)](#apidoc.element.d3.easeQuad)
- description and source-code
```javascript
function quadInOut(t) {
  return ((t *= 2) <= 1 ? t * t : --t * (2 - t) + 1) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeQuadIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easeQuadIn (t)](#apidoc.element.d3.easeQuadIn)
- description and source-code
```javascript
function quadIn(t) {
  return t * t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeQuadInOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeQuadInOut (t)](#apidoc.element.d3.easeQuadInOut)
- description and source-code
```javascript
function quadInOut(t) {
  return ((t *= 2) <= 1 ? t * t : --t * (2 - t) + 1) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeQuadOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeQuadOut (t)](#apidoc.element.d3.easeQuadOut)
- description and source-code
```javascript
function quadOut(t) {
  return t * (2 - t);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeSin"></a>[function <span class="apidocSignatureSpan">d3.</span>easeSin (t)](#apidoc.element.d3.easeSin)
- description and source-code
```javascript
function sinInOut(t) {
  return (1 - Math.cos(pi * t)) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeSinIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easeSinIn (t)](#apidoc.element.d3.easeSinIn)
- description and source-code
```javascript
function sinIn(t) {
  return 1 - Math.cos(t * halfPi);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeSinInOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeSinInOut (t)](#apidoc.element.d3.easeSinInOut)
- description and source-code
```javascript
function sinInOut(t) {
  return (1 - Math.cos(pi * t)) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeSinOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeSinOut (t)](#apidoc.element.d3.easeSinOut)
- description and source-code
```javascript
function sinOut(t) {
  return Math.sin(t * halfPi);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.entries"></a>[function <span class="apidocSignatureSpan">d3.</span>entries (map)](#apidoc.element.d3.entries)
- description and source-code
```javascript
entries = function (map) {
  var entries = [];
  for (var key in map) entries.push({key: key, value: map[key]});
  return entries;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.extent"></a>[function <span class="apidocSignatureSpan">d3.</span>extent (array, f)](#apidoc.element.d3.extent)
- description and source-code
```javascript
extent = function (array, f) {
  var i = -1,
      n = array.length,
      a,
      b,
      c;

  if (f == null) {
    while (++i < n) if ((b = array[i]) != null && b >= b) { a = c = b; break; }
    while (++i < n) if ((b = array[i]) != null) {
      if (a > b) a = b;
      if (c < b) c = b;
    }
  }

  else {
    while (++i < n) if ((b = f(array[i], i, array)) != null && b >= b) { a = c = b; break; }
    while (++i < n) if ((b = f(array[i], i, array)) != null) {
      if (a > b) a = b;
      if (c < b) c = b;
    }
  }

  return [a, c];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.forceCenter"></a>[function <span class="apidocSignatureSpan">d3.</span>forceCenter (x, y)](#apidoc.element.d3.forceCenter)
- description and source-code
```javascript
forceCenter = function (x, y) {
  var nodes;

  if (x == null) x = 0;
  if (y == null) y = 0;

  function force() {
    var i,
        n = nodes.length,
        node,
        sx = 0,
        sy = 0;

    for (i = 0; i < n; ++i) {
      node = nodes[i], sx += node.x, sy += node.y;
    }

    for (sx = sx / n - x, sy = sy / n - y, i = 0; i < n; ++i) {
      node = nodes[i], node.x -= sx, node.y -= sy;
    }
  }

  force.initialize = function(_) {
    nodes = _;
  };

  force.x = function(_) {
    return arguments.length ? (x = +_, force) : x;
  };

  force.y = function(_) {
    return arguments.length ? (y = +_, force) : y;
  };

  return force;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.forceCollide"></a>[function <span class="apidocSignatureSpan">d3.</span>forceCollide (radius)](#apidoc.element.d3.forceCollide)
- description and source-code
```javascript
forceCollide = function (radius) {
  var nodes,
      radii,
      strength = 1,
      iterations = 1;

  if (typeof radius !== "function") radius = constant(radius == null ? 1 : +radius);

  function force() {
    var i, n = nodes.length,
        tree,
        node,
        xi,
        yi,
        ri,
        ri2;

    for (var k = 0; k < iterations; ++k) {
      tree = d3Quadtree.quadtree(nodes, x, y).visitAfter(prepare);
      for (i = 0; i < n; ++i) {
        node = nodes[i];
        ri = radii[node.index], ri2 = ri * ri;
        xi = node.x + node.vx;
        yi = node.y + node.vy;
        tree.visit(apply);
      }
    }

    function apply(quad, x0, y0, x1, y1) {
      var data = quad.data, rj = quad.r, r = ri + rj;
      if (data) {
        if (data.index > node.index) {
          var x = xi - data.x - data.vx,
              y = yi - data.y - data.vy,
              l = x * x + y * y;
          if (l < r * r) {
            if (x === 0) x = jiggle(), l += x * x;
            if (y === 0) y = jiggle(), l += y * y;
            l = (r - (l = Math.sqrt(l))) / l * strength;
            node.vx += (x *= l) * (r = (rj *= rj) / (ri2 + rj));
            node.vy += (y *= l) * r;
            data.vx -= x * (r = 1 - r);
            data.vy -= y * r;
          }
        }
        return;
      }
      return x0 > xi + r || x1 < xi - r || y0 > yi + r || y1 < yi - r;
    }
  }

  function prepare(quad) {
    if (quad.data) return quad.r = radii[quad.data.index];
    for (var i = quad.r = 0; i < 4; ++i) {
      if (quad[i] && quad[i].r > quad.r) {
        quad.r = quad[i].r;
      }
    }
  }

  function initialize() {
    if (!nodes) return;
    var i, n = nodes.length, node;
    radii = new Array(n);
    for (i = 0; i < n; ++i) node = nodes[i], radii[node.index] = +radius(node, i, nodes);
  }

  force.initialize = function(_) {
    nodes = _;
    initialize();
  };

  force.iterations = function(_) {
    return arguments.length ? (iterations = +_, force) : iterations;
  };

  force.strength = function(_) {
    return arguments.length ? (strength = +_, force) : strength;
  };

  force.radius = function(_) {
    return arguments.length ? (radius = typeof _ === "function" ? _ : constant(+_), initialize(), force) : radius;
  };

  return force;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.forceLink"></a>[function <span class="apidocSignatureSpan">d3.</span>forceLink (links)](#apidoc.element.d3.forceLink)
- description and source-code
```javascript
forceLink = function (links) {
  var id = index,
      strength = defaultStrength,
      strengths,
      distance = constant(30),
      distances,
      nodes,
      count,
      bias,
      iterations = 1;

  if (links == null) links = [];

  function defaultStrength(link) {
    return 1 / Math.min(count[link.source.index], count[link.target.index]);
  }

  function force(alpha) {
    for (var k = 0, n = links.length; k < iterations; ++k) {
      for (var i = 0, link, source, target, x, y, l, b; i < n; ++i) {
        link = links[i], source = link.source, target = link.target;
        x = target.x + target.vx - source.x - source.vx || jiggle();
        y = target.y + target.vy - source.y - source.vy || jiggle();
        l = Math.sqrt(x * x + y * y);
        l = (l - distances[i]) / l * alpha * strengths[i];
        x *= l, y *= l;
        target.vx -= x * (b = bias[i]);
        target.vy -= y * b;
        source.vx += x * (b = 1 - b);
        source.vy += y * b;
      }
    }
  }

  function initialize() {
    if (!nodes) return;

    var i,
        n = nodes.length,
        m = links.length,
        nodeById = d3Collection.map(nodes, id),
        link;

    for (i = 0, count = new Array(n); i < m; ++i) {
      link = links[i], link.index = i;
      if (typeof link.source !== "object") link.source = find(nodeById, link.source);
      if (typeof link.target !== "object") link.target = find(nodeById, link.target);
      count[link.source.index] = (count[link.source.index] || 0) + 1;
      count[link.target.index] = (count[link.target.index] || 0) + 1;
    }

    for (i = 0, bias = new Array(m); i < m; ++i) {
      link = links[i], bias[i] = count[link.source.index] / (count[link.source.index] + count[link.target.index]);
    }

    strengths = new Array(m), initializeStrength();
    distances = new Array(m), initializeDistance();
  }

  function initializeStrength() {
    if (!nodes) return;

    for (var i = 0, n = links.length; i < n; ++i) {
      strengths[i] = +strength(links[i], i, links);
    }
  }

  function initializeDistance() {
    if (!nodes) return;

    for (var i = 0, n = links.length; i < n; ++i) {
      distances[i] = +distance(links[i], i, links);
    }
  }

  force.initialize = function(_) {
    nodes = _;
    initialize();
  };

  force.links = function(_) {
    return arguments.length ? (links = _, initialize(), force) : links;
  };

  force.id = function(_) {
    return arguments.length ? (id = _, force) : id;
  };

  force.iterations = function(_) {
    return arguments.length ? (iterations = +_, force) : iterations;
  };

  force.strength = function(_) {
    return arguments.length ? (strength = typeof _ === "function" ? _ : constant(+_), initializeStrength(), force) : strength;
  };

  force.distance = function(_) {
    return arguments.length ? (distance = typeof _ === "function" ? _ : constant(+_), initializeDistance(), force) : distance;
  };

  return force;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.forceManyBody"></a>[function <span class="apidocSignatureSpan">d3.</span>forceManyBody ()](#apidoc.element.d3.forceManyBody)
- description and source-code
```javascript
forceManyBody = function () {
  var nodes,
      node,
      alpha,
      strength = constant(-30),
      strengths,
      distanceMin2 = 1,
      distanceMax2 = Infinity,
      theta2 = 0.81;

  function force(_) {
    var i, n = nodes.length, tree = d3Quadtree.quadtree(nodes, x$1, y$1).visitAfter(accumulate);
    for (alpha = _, i = 0; i < n; ++i) node = nodes[i], tree.visit(apply);
  }

  function initialize() {
    if (!nodes) return;
    var i, n = nodes.length, node;
    strengths = new Array(n);
    for (i = 0; i < n; ++i) node = nodes[i], strengths[node.index] = +strength(node, i, nodes);
  }

  function accumulate(quad) {
    var strength = 0, q, c, x$$1, y$$1, i;

    // For internal nodes, accumulate forces from child quadrants.
    if (quad.length) {
      for (x$$1 = y$$1 = i = 0; i < 4; ++i) {
        if ((q = quad[i]) && (c = q.value)) {
          strength += c, x$$1 += c * q.x, y$$1 += c * q.y;
        }
      }
      quad.x = x$$1 / strength;
      quad.y = y$$1 / strength;
    }

    // For leaf nodes, accumulate forces from coincident quadrants.
    else {
      q = quad;
      q.x = q.data.x;
      q.y = q.data.y;
      do strength += strengths[q.data.index];
      while (q = q.next);
    }

    quad.value = strength;
  }

  function apply(quad, x1, _, x2) {
    if (!quad.value) return true;

    var x$$1 = quad.x - node.x,
        y$$1 = quad.y - node.y,
        w = x2 - x1,
        l = x$$1 * x$$1 + y$$1 * y$$1;

    // Apply the Barnes-Hut approximation if possible.
    // Limit forces for very close nodes; randomize direction if coincident.
    if (w * w / theta2 < l) {
      if (l < distanceMax2) {
        if (x$$1 === 0) x$$1 = jiggle(), l += x$$1 * x$$1;
        if (y$$1 === 0) y$$1 = jiggle(), l += y$$1 * y$$1;
        if (l < distanceMin2) l = Math.sqrt(distanceMin2 * l);
        node.vx += x$$1 * quad.value * alpha / l;
        node.vy += y$$1 * quad.value * alpha / l;
      }
      return true;
    }

    // Otherwise, process points directly.
    else if (quad.length || l >= distanceMax2) return;

    // Limit forces for very close nodes; randomize direction if coincident.
    if (quad.data !== node || quad.next) {
      if (x$$1 === 0) x$$1 = jiggle(), l += x$$1 * x$$1;
      if (y$$1 === 0) y$$1 = jiggle(), l += y$$1 * y$$1;
      if (l < distanceMin2) l = Math.sqrt(distanceMin2 * l);
    }

    do if (quad.data !== node) {
      w = strengths[quad.data.index] * alpha / l;
      node.vx += x$$1 * w;
      node.vy += y$$1 * w;
    } while (quad = quad.next);
  }

  force.initialize = function(_) {
    nodes = _;
    initialize();
  };

  force.strength = function(_) {
    return arguments.length ? (strength = typeof _ === "function" ? _ : constant(+_), initialize(), force) : strength;
  };

  force.distanceMin = function(_) {
    return arguments.length ? (distanceMin2 = _ * _, force) : Math.sqrt(distanceMin2);
  };

  force.distanceMax = function(_) {
    return arguments.length ? (distanceMax2 = _ * _, force) : Math.sqrt(distanceMax2);
  };

  force.theta = function(_) {
    return arguments.length ? (theta2 = _ * _, force) : Math.sqrt(theta2);
  };

  return force;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.forceSimulation"></a>[function <span class="apidocSignatureSpan">d3.</span>forceSimulation (nodes)](#apidoc.element.d3.forceSimulation)
- description and source-code
```javascript
forceSimulation = function (nodes) {
  var simulation,
      alpha = 1,
      alphaMin = 0.001,
      alphaDecay = 1 - Math.pow(alphaMin, 1 / 300),
      alphaTarget = 0,
      velocityDecay = 0.6,
      forces = d3Collection.map(),
      stepper = d3Timer.timer(step),
      event = d3Dispatch.dispatch("tick", "end");

  if (nodes == null) nodes = [];

  function step() {
    tick();
    event.call("tick", simulation);
    if (alpha < alphaMin) {
      stepper.stop();
      event.call("end", simulation);
    }
  }

  function tick() {
    var i, n = nodes.length, node;

    alpha += (alphaTarget - alpha) * alphaDecay;

    forces.each(function(force) {
      force(alpha);
    });

    for (i = 0; i < n; ++i) {
      node = nodes[i];
      if (node.fx == null) node.x += node.vx *= velocityDecay;
      else node.x = node.fx, node.vx = 0;
      if (node.fy == null) node.y += node.vy *= velocityDecay;
      else node.y = node.fy, node.vy = 0;
    }
  }

  function initializeNodes() {
    for (var i = 0, n = nodes.length, node; i < n; ++i) {
      node = nodes[i], node.index = i;
      if (isNaN(node.x) || isNaN(node.y)) {
        var radius = initialRadius * Math.sqrt(i), angle = i * initialAngle;
        node.x = radius * Math.cos(angle);
        node.y = radius * Math.sin(angle);
      }
      if (isNaN(node.vx) || isNaN(node.vy)) {
        node.vx = node.vy = 0;
      }
    }
  }

  function initializeForce(force) {
    if (force.initialize) force.initialize(nodes);
    return force;
  }

  initializeNodes();

  return simulation = {
    tick: tick,

    restart: function() {
      return stepper.restart(step), simulation;
    },

    stop: function() {
      return stepper.stop(), simulation;
    },

    nodes: function(_) {
      return arguments.length ? (nodes = _, initializeNodes(), forces.each(initializeForce), simulation) : nodes;
    },

    alpha: function(_) {
      return arguments.length ? (alpha = +_, simulation) : alpha;
    },

    alphaMin: function(_) {
      return arguments.length ? (alphaMin = +_, simulation) : alphaMin;
    },

    alphaDecay: function(_) {
      return arguments.length ? (alphaDecay = +_, simulation) : +alphaDecay;
    },

    alphaTarget: function(_) {
      return arguments.length ? (alphaTarget = +_, simulation) : alphaTarget;
    },

    velocityDecay: function(_) {
      return arguments.length ? (velocityDecay = 1 - _, simulation) : 1 - velocityDecay;
    },

    force: function(name, _) {
      return arguments.length > 1 ? ((_ == null ? forces.remove(name) : forces.set(name, initializeForce(_))), simulation) : forces
.get(name);
    },

    find: function(x, y, radius) {
      var i = 0,
          n = nodes.length,
          dx,
          dy,
          d2,
          node,
          closest;

      if (radius == null) radius = Infinity;
      else radius *= radius;

      for (i = 0; i < n; ++i) {
        node = nodes[i];
        dx = x - node.x;
        dy = y - node.y;
        d2 = dx * dx + dy * dy;
        if (d2 < radius) closest = node, radius = d2;
      }

      return closest;
    },

    on: function(name, _) {
      return arguments.length > 1 ? (event.on(name, _), simulation) : event.on(name);
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.forceX"></a>[function <span class="apidocSignatureSpan">d3.</span>forceX (x)](#apidoc.element.d3.forceX)
- description and source-code
```javascript
forceX = function (x) {
  var strength = constant(0.1),
      nodes,
      strengths,
      xz;

  if (typeof x !== "function") x = constant(x == null ? 0 : +x);

  function force(alpha) {
    for (var i = 0, n = nodes.length, node; i < n; ++i) {
      node = nodes[i], node.vx += (xz[i] - node.x) * strengths[i] * alpha;
    }
  }

  function initialize() {
    if (!nodes) return;
    var i, n = nodes.length;
    strengths = new Array(n);
    xz = new Array(n);
    for (i = 0; i < n; ++i) {
      strengths[i] = isNaN(xz[i] = +x(nodes[i], i, nodes)) ? 0 : +strength(nodes[i], i, nodes);
    }
  }

  force.initialize = function(_) {
    nodes = _;
    initialize();
  };

  force.strength = function(_) {
    return arguments.length ? (strength = typeof _ === "function" ? _ : constant(+_), initialize(), force) : strength;
  };

  force.x = function(_) {
    return arguments.length ? (x = typeof _ === "function" ? _ : constant(+_), initialize(), force) : x;
  };

  return force;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.forceY"></a>[function <span class="apidocSignatureSpan">d3.</span>forceY (y)](#apidoc.element.d3.forceY)
- description and source-code
```javascript
forceY = function (y) {
  var strength = constant(0.1),
      nodes,
      strengths,
      yz;

  if (typeof y !== "function") y = constant(y == null ? 0 : +y);

  function force(alpha) {
    for (var i = 0, n = nodes.length, node; i < n; ++i) {
      node = nodes[i], node.vy += (yz[i] - node.y) * strengths[i] * alpha;
    }
  }

  function initialize() {
    if (!nodes) return;
    var i, n = nodes.length;
    strengths = new Array(n);
    yz = new Array(n);
    for (i = 0; i < n; ++i) {
      strengths[i] = isNaN(yz[i] = +y(nodes[i], i, nodes)) ? 0 : +strength(nodes[i], i, nodes);
    }
  }

  force.initialize = function(_) {
    nodes = _;
    initialize();
  };

  force.strength = function(_) {
    return arguments.length ? (strength = typeof _ === "function" ? _ : constant(+_), initialize(), force) : strength;
  };

  force.y = function(_) {
    return arguments.length ? (y = typeof _ === "function" ? _ : constant(+_), initialize(), force) : y;
  };

  return force;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.format"></a>[function <span class="apidocSignatureSpan">d3.</span>format (specifier)](#apidoc.element.d3.format)
- description and source-code
```javascript
function newFormat(specifier) {
  specifier = formatSpecifier(specifier);

  var fill = specifier.fill,
      align = specifier.align,
      sign = specifier.sign,
      symbol = specifier.symbol,
      zero = specifier.zero,
      width = specifier.width,
      comma = specifier.comma,
      precision = specifier.precision,
      type = specifier.type;

  // Compute the prefix and suffix.
  // For SI-prefix, the suffix is lazily computed.
  var prefix = symbol === "$" ? currency[0] : symbol === "#" && /[boxX]/.test(type) ? "0" + type.toLowerCase() : "",
      suffix = symbol === "$" ? currency[1] : /[%p]/.test(type) ? "%" : "";

  // What format function should we use?
  // Is this an integer type?
  // Can this type generate exponential notation?
  var formatType = formatTypes[type],
      maybeSuffix = !type || /[defgprs%]/.test(type);

  // Set the default precision if not specified,
  // or clamp the specified precision to the supported range.
  // For significant precision, it must be in [1, 21].
  // For fixed precision, it must be in [0, 20].
  precision = precision == null ? (type ? 6 : 12)
      : /[gprs]/.test(type) ? Math.max(1, Math.min(21, precision))
      : Math.max(0, Math.min(20, precision));

  function format(value) {
    var valuePrefix = prefix,
        valueSuffix = suffix,
        i, n, c;

    if (type === "c") {
      valueSuffix = formatType(value) + valueSuffix;
      value = "";
    } else {
      value = +value;

      // Perform the initial formatting.
      var valueNegative = value < 0;
      value = formatType(Math.abs(value), precision);

      // If a negative value rounds to zero during formatting, treat as positive.
      if (valueNegative && +value === 0) valueNegative = false;

      // Compute the prefix and suffix.
      valuePrefix = (valueNegative ? (sign === "(" ? sign : "-") : sign === "-" || sign === "(" ? "" : sign) + valuePrefix;
      valueSuffix = valueSuffix + (type === "s" ? prefixes[8 + prefixExponent / 3] : "") + (valueNegative && sign === "(" ? ")" : "");

      // Break the formatted value into the integer “value” part that can be
      // grouped, and fractional or exponential “suffix” part that is not.
      if (maybeSuffix) {
        i = -1, n = value.length;
        while (++i < n) {
          if (c = value.charCodeAt(i), 48 > c || c > 57) {
            valueSuffix = (c === 46 ? decimal + value.slice(i + 1) : value.slice(i)) + valueSuffix;
            value = value.slice(0, i);
            break;
          }
        }
      }
    }

    // If the fill character is not "0", grouping is applied before padding.
    if (comma && !zero) value = group(value, Infinity);

    // Compute the padding.
    var length = valuePrefix.length + value.length + valueSuffix.length,
        padding = length < width ? new Array(width - length + 1).join(fill) : "";

    // If the fill character is "0", grouping is applied after padding.
    if (comma && zero) value = group(padding + value, padding.length ? width - valueSuffix.length : Infinity), padding = "";

    // Reconstruct the final output based on the desired alignment.
    switch (align) {
      case "<": value = valuePrefix + value + valueSuffix + padding; break;
      case "=": value = valuePrefix + padding + value + valueSuffix; break;
      case "^": value = padding.slice(0, length = padding.length >> 1) + valuePrefix + value + valueSuffix + padding.slice(length
); break;
      default: value = padding + valuePrefix + value + valueSuffix; break;
    }

    return numerals(value);
  }

  format.toString = function() {
    return specifier + "";
  };

  return format;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.formatDefaultLocale"></a>[function <span class="apidocSignatureSpan">d3.</span>formatDefaultLocale (definition)](#apidoc.element.d3.formatDefaultLocale)
- description and source-code
```javascript
function defaultLocale(definition) {
  locale = formatLocale(definition);
  exports.format = locale.format;
  exports.formatPrefix = locale.formatPrefix;
  return locale;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.formatLocale"></a>[function <span class="apidocSignatureSpan">d3.</span>formatLocale (locale)](#apidoc.element.d3.formatLocale)
- description and source-code
```javascript
formatLocale = function (locale) {
  var group = locale.grouping && locale.thousands ? formatGroup(locale.grouping, locale.thousands) : identity,
      currency = locale.currency,
      decimal = locale.decimal,
      numerals = locale.numerals ? formatNumerals(locale.numerals) : identity;

  function newFormat(specifier) {
    specifier = formatSpecifier(specifier);

    var fill = specifier.fill,
        align = specifier.align,
        sign = specifier.sign,
        symbol = specifier.symbol,
        zero = specifier.zero,
        width = specifier.width,
        comma = specifier.comma,
        precision = specifier.precision,
        type = specifier.type;

    // Compute the prefix and suffix.
    // For SI-prefix, the suffix is lazily computed.
    var prefix = symbol === "$" ? currency[0] : symbol === "#" && /[boxX]/.test(type) ? "0" + type.toLowerCase() : "",
        suffix = symbol === "$" ? currency[1] : /[%p]/.test(type) ? "%" : "";

    // What format function should we use?
    // Is this an integer type?
    // Can this type generate exponential notation?
    var formatType = formatTypes[type],
        maybeSuffix = !type || /[defgprs%]/.test(type);

    // Set the default precision if not specified,
    // or clamp the specified precision to the supported range.
    // For significant precision, it must be in [1, 21].
    // For fixed precision, it must be in [0, 20].
    precision = precision == null ? (type ? 6 : 12)
        : /[gprs]/.test(type) ? Math.max(1, Math.min(21, precision))
        : Math.max(0, Math.min(20, precision));

    function format(value) {
      var valuePrefix = prefix,
          valueSuffix = suffix,
          i, n, c;

      if (type === "c") {
        valueSuffix = formatType(value) + valueSuffix;
        value = "";
      } else {
        value = +value;

        // Perform the initial formatting.
        var valueNegative = value < 0;
        value = formatType(Math.abs(value), precision);

        // If a negative value rounds to zero during formatting, treat as positive.
        if (valueNegative && +value === 0) valueNegative = false;

        // Compute the prefix and suffix.
        valuePrefix = (valueNegative ? (sign === "(" ? sign : "-") : sign === "-" || sign === "(" ? "" : sign) + valuePrefix;
        valueSuffix = valueSuffix + (type === "s" ? prefixes[8 + prefixExponent / 3] : "") + (valueNegative && sign === "(" ? ")" : "");

        // Break the formatted value into the integer “value” part that can be
        // grouped, and fractional or exponential “suffix” part that is not.
        if (maybeSuffix) {
          i = -1, n = value.length;
          while (++i < n) {
            if (c = value.charCodeAt(i), 48 > c || c > 57) {
              valueSuffix = (c === 46 ? decimal + value.slice(i + 1) : value.slice(i)) + valueSuffix;
              value = value.slice(0, i);
              break;
            }
          }
        }
      }

      // If the fill character is not "0", grouping is applied before padding.
      if (comma && !zero) value = group(value, Infinity);

      // Compute the padding.
      var length = valuePrefix.length + value.length + valueSuffix.length,
          padding = length < width ? new Array(width - length + 1).join(fill) : "";

      // If the fill character is "0", grouping is applied after padding.
      if (comma && zero) value = group(padding + value, padding.length ? width - valueSuffix.length : Infinity), padding = "";

      // Reconstruct the final output based on the desired alignment.
      switch (align) {
        case "<": value = valuePrefix + value + valueSuffix + padding; break;
        case "=": value = valuePrefix + padding + value + valueSuffix; break;
        case "^": value = padding.slice(0, length = padding.length >> 1) + valuePrefix + value + valueSuffix + padding.slice(length
); break;
        default: value = padding + valuePrefix + value + valueSuffix; break;
      }

      return numerals(value);
    }

    format.toString = function() {
      return specifier + "";
    };

    return format;
  }

  function formatPrefix(spe ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.formatPrefix"></a>[function <span class="apidocSignatureSpan">d3.</span>formatPrefix (specifier, value)](#apidoc.element.d3.formatPrefix)
- description and source-code
```javascript
function formatPrefix(specifier, value) {
  var f = newFormat((specifier = formatSpecifier(specifier), specifier.type = "f", specifier)),
      e = Math.max(-8, Math.min(8, Math.floor(exponent(value) / 3))) * 3,
      k = Math.pow(10, -e),
      prefix = prefixes[8 + e / 3];
  return function(value) {
    return f(k * value) + prefix;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.formatSpecifier"></a>[function <span class="apidocSignatureSpan">d3.</span>formatSpecifier (specifier)](#apidoc.element.d3.formatSpecifier)
- description and source-code
```javascript
function formatSpecifier(specifier) {
  return new FormatSpecifier(specifier);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoAlbers"></a>[function <span class="apidocSignatureSpan">d3.</span>geoAlbers ()](#apidoc.element.d3.geoAlbers)
- description and source-code
```javascript
geoAlbers = function () {
  return conicEqualArea()
      .parallels([29.5, 45.5])
      .scale(1070)
      .translate([480, 250])
      .rotate([96, 0])
      .center([-0.6, 38.7]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoAlbersUsa"></a>[function <span class="apidocSignatureSpan">d3.</span>geoAlbersUsa ()](#apidoc.element.d3.geoAlbersUsa)
- description and source-code
```javascript
geoAlbersUsa = function () {
  var cache,
      cacheStream,
      lower48 = albers(), lower48Point,
      alaska = conicEqualArea().rotate([154, 0]).center([-2, 58.5]).parallels([55, 65]), alaskaPoint, // EPSG:3338
      hawaii = conicEqualArea().rotate([157, 0]).center([-3, 19.9]).parallels([8, 18]), hawaiiPoint, // ESRI:102007
      point, pointStream = {point: function(x, y) { point = [x, y]; }};

  function albersUsa(coordinates) {
    var x = coordinates[0], y = coordinates[1];
    return point = null,
        (lower48Point.point(x, y), point)
        || (alaskaPoint.point(x, y), point)
        || (hawaiiPoint.point(x, y), point);
  }

  albersUsa.invert = function(coordinates) {
    var k = lower48.scale(),
        t = lower48.translate(),
        x = (coordinates[0] - t[0]) / k,
        y = (coordinates[1] - t[1]) / k;
    return (y >= 0.120 && y < 0.234 && x >= -0.425 && x < -0.214 ? alaska
        : y >= 0.166 && y < 0.234 && x >= -0.214 && x < -0.115 ? hawaii
        : lower48).invert(coordinates);
  };

  albersUsa.stream = function(stream) {
    return cache && cacheStream === stream ? cache : cache = multiplex([lower48.stream(cacheStream = stream), alaska.stream(stream
), hawaii.stream(stream)]);
  };

  albersUsa.precision = function(_) {
    if (!arguments.length) return lower48.precision();
    lower48.precision(_), alaska.precision(_), hawaii.precision(_);
    return reset();
  };

  albersUsa.scale = function(_) {
    if (!arguments.length) return lower48.scale();
    lower48.scale(_), alaska.scale(_ * 0.35), hawaii.scale(_);
    return albersUsa.translate(lower48.translate());
  };

  albersUsa.translate = function(_) {
    if (!arguments.length) return lower48.translate();
    var k = lower48.scale(), x = +_[0], y = +_[1];

    lower48Point = lower48
        .translate(_)
        .clipExtent([[x - 0.455 * k, y - 0.238 * k], [x + 0.455 * k, y + 0.238 * k]])
        .stream(pointStream);

    alaskaPoint = alaska
        .translate([x - 0.307 * k, y + 0.201 * k])
        .clipExtent([[x - 0.425 * k + epsilon, y + 0.120 * k + epsilon], [x - 0.214 * k - epsilon, y + 0.234 * k - epsilon]])
        .stream(pointStream);

    hawaiiPoint = hawaii
        .translate([x - 0.205 * k, y + 0.212 * k])
        .clipExtent([[x - 0.214 * k + epsilon, y + 0.166 * k + epsilon], [x - 0.115 * k - epsilon, y + 0.234 * k - epsilon]])
        .stream(pointStream);

    return reset();
  };

  albersUsa.fitExtent = function(extent, object) {
    return fitExtent(albersUsa, extent, object);
  };

  albersUsa.fitSize = function(size, object) {
    return fitSize(albersUsa, size, object);
  };

  function reset() {
    cache = cacheStream = null;
    return albersUsa;
  }

  return albersUsa.scale(1070);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoArea"></a>[function <span class="apidocSignatureSpan">d3.</span>geoArea (object)](#apidoc.element.d3.geoArea)
- description and source-code
```javascript
geoArea = function (object) {
  areaSum.reset();
  geoStream(object, areaStream);
  return areaSum * 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoAzimuthalEqualArea"></a>[function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEqualArea ()](#apidoc.element.d3.geoAzimuthalEqualArea)
- description and source-code
```javascript
geoAzimuthalEqualArea = function () {
  return projection(azimuthalEqualAreaRaw)
      .scale(124.75)
      .clipAngle(180 - 1e-3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoAzimuthalEqualAreaRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEqualAreaRaw (x, y)](#apidoc.element.d3.geoAzimuthalEqualAreaRaw)
- description and source-code
```javascript
geoAzimuthalEqualAreaRaw = function (x, y) {
  var cx = cos(x),
      cy = cos(y),
      k = scale(cx * cy);
  return [
    k * cy * sin(x),
    k * sin(y)
  ];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoAzimuthalEquidistant"></a>[function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEquidistant ()](#apidoc.element.d3.geoAzimuthalEquidistant)
- description and source-code
```javascript
geoAzimuthalEquidistant = function () {
  return projection(azimuthalEquidistantRaw)
      .scale(79.4188)
      .clipAngle(180 - 1e-3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoAzimuthalEquidistantRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEquidistantRaw (x, y)](#apidoc.element.d3.geoAzimuthalEquidistantRaw)
- description and source-code
```javascript
geoAzimuthalEquidistantRaw = function (x, y) {
  var cx = cos(x),
      cy = cos(y),
      k = scale(cx * cy);
  return [
    k * cy * sin(x),
    k * sin(y)
  ];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoBounds"></a>[function <span class="apidocSignatureSpan">d3.</span>geoBounds (feature)](#apidoc.element.d3.geoBounds)
- description and source-code
```javascript
geoBounds = function (feature) {
  var i, n, a, b, merged, deltaMax, delta;

  phi1 = lambda1 = -(lambda0$1 = phi0 = Infinity);
  ranges = [];
  geoStream(feature, boundsStream);

  // First, sort ranges by their minimum longitudes.
  if (n = ranges.length) {
    ranges.sort(rangeCompare);

    // Then, merge any ranges that overlap.
    for (i = 1, a = ranges[0], merged = [a]; i < n; ++i) {
      b = ranges[i];
      if (rangeContains(a, b[0]) || rangeContains(a, b[1])) {
        if (angle(a[0], b[1]) > angle(a[0], a[1])) a[1] = b[1];
        if (angle(b[0], a[1]) > angle(a[0], a[1])) a[0] = b[0];
      } else {
        merged.push(a = b);
      }
    }

    // Finally, find the largest gap between the merged ranges.
    // The final bounding box will be the inverse of this gap.
    for (deltaMax = -Infinity, n = merged.length - 1, i = 0, a = merged[n]; i <= n; a = b, ++i) {
      b = merged[i];
      if ((delta = angle(a[1], b[0])) > deltaMax) deltaMax = delta, lambda0$1 = b[0], lambda1 = a[1];
    }
  }

  ranges = range$1 = null;

  return lambda0$1 === Infinity || phi0 === Infinity
      ? [[NaN, NaN], [NaN, NaN]]
      : [[lambda0$1, phi0], [lambda1, phi1]];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoCentroid"></a>[function <span class="apidocSignatureSpan">d3.</span>geoCentroid (object)](#apidoc.element.d3.geoCentroid)
- description and source-code
```javascript
geoCentroid = function (object) {
  W0 = W1 =
  X0 = Y0 = Z0 =
  X1 = Y1 = Z1 =
  X2 = Y2 = Z2 = 0;
  geoStream(object, centroidStream);

  var x = X2,
      y = Y2,
      z = Z2,
      m = x * x + y * y + z * z;

  // If the area-weighted ccentroid is undefined, fall back to length-weighted ccentroid.
  if (m < epsilon2) {
    x = X1, y = Y1, z = Z1;
    // If the feature has zero length, fall back to arithmetic mean of point vectors.
    if (W1 < epsilon) x = X0, y = Y0, z = Z0;
    m = x * x + y * y + z * z;
    // If the feature still has an undefined ccentroid, then return.
    if (m < epsilon2) return [NaN, NaN];
  }

  return [atan2(y, x) * degrees, asin(z / sqrt(m)) * degrees];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoCircle"></a>[function <span class="apidocSignatureSpan">d3.</span>geoCircle ()](#apidoc.element.d3.geoCircle)
- description and source-code
```javascript
geoCircle = function () {
  var center = constant([0, 0]),
      radius = constant(90),
      precision = constant(6),
      ring,
      rotate,
      stream = {point: point};

  function point(x, y) {
    ring.push(x = rotate(x, y));
    x[0] *= degrees, x[1] *= degrees;
  }

  function circle() {
    var c = center.apply(this, arguments),
        r = radius.apply(this, arguments) * radians,
        p = precision.apply(this, arguments) * radians;
    ring = [];
    rotate = rotateRadians(-c[0] * radians, -c[1] * radians, 0).invert;
    circleStream(stream, r, p, 1);
    c = {type: "Polygon", coordinates: [ring]};
    ring = rotate = null;
    return c;
  }

  circle.center = function(_) {
    return arguments.length ? (center = typeof _ === "function" ? _ : constant([+_[0], +_[1]]), circle) : center;
  };

  circle.radius = function(_) {
    return arguments.length ? (radius = typeof _ === "function" ? _ : constant(+_), circle) : radius;
  };

  circle.precision = function(_) {
    return arguments.length ? (precision = typeof _ === "function" ? _ : constant(+_), circle) : precision;
  };

  return circle;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoClipExtent"></a>[function <span class="apidocSignatureSpan">d3.</span>geoClipExtent ()](#apidoc.element.d3.geoClipExtent)
- description and source-code
```javascript
geoClipExtent = function () {
  var x0 = 0,
      y0 = 0,
      x1 = 960,
      y1 = 500,
      cache,
      cacheStream,
      clip;

  return clip = {
    stream: function(stream) {
      return cache && cacheStream === stream ? cache : cache = clipExtent(x0, y0, x1, y1)(cacheStream = stream);
    },
    extent: function(_) {
      return arguments.length ? (x0 = +_[0][0], y0 = +_[0][1], x1 = +_[1][0], y1 = +_[1][1], cache = cacheStream = null, clip) : [[
x0, y0], [x1, y1]];
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoConicConformal"></a>[function <span class="apidocSignatureSpan">d3.</span>geoConicConformal ()](#apidoc.element.d3.geoConicConformal)
- description and source-code
```javascript
geoConicConformal = function () {
  return conicProjection(conicConformalRaw)
      .scale(109.5)
      .parallels([30, 30]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoConicConformalRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoConicConformalRaw (y0, y1)](#apidoc.element.d3.geoConicConformalRaw)
- description and source-code
```javascript
function conicConformalRaw(y0, y1) {
  var cy0 = cos(y0),
      n = y0 === y1 ? sin(y0) : log(cy0 / cos(y1)) / log(tany(y1) / tany(y0)),
      f = cy0 * pow(tany(y0), n) / n;

  if (!n) return mercatorRaw;

  function project(x, y) {
    if (f > 0) { if (y < -halfPi + epsilon) y = -halfPi + epsilon; }
    else { if (y > halfPi - epsilon) y = halfPi - epsilon; }
    var r = f / pow(tany(y), n);
    return [r * sin(n * x), f - r * cos(n * x)];
  }

  project.invert = function(x, y) {
    var fy = f - y, r = sign(n) * sqrt(x * x + fy * fy);
    return [atan2(x, abs(fy)) / n * sign(fy), 2 * atan(pow(f / r, 1 / n)) - halfPi];
  };

  return project;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoConicEqualArea"></a>[function <span class="apidocSignatureSpan">d3.</span>geoConicEqualArea ()](#apidoc.element.d3.geoConicEqualArea)
- description and source-code
```javascript
geoConicEqualArea = function () {
  return conicProjection(conicEqualAreaRaw)
      .scale(155.424)
      .center([0, 33.6442]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoConicEqualAreaRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoConicEqualAreaRaw (y0, y1)](#apidoc.element.d3.geoConicEqualAreaRaw)
- description and source-code
```javascript
function conicEqualAreaRaw(y0, y1) {
  var sy0 = sin(y0), n = (sy0 + sin(y1)) / 2;

  // Are the parallels symmetrical around the Equator?
  if (abs(n) < epsilon) return cylindricalEqualAreaRaw(y0);

  var c = 1 + sy0 * (2 * n - sy0), r0 = sqrt(c) / n;

  function project(x, y) {
    var r = sqrt(c - 2 * n * sin(y)) / n;
    return [r * sin(x *= n), r0 - r * cos(x)];
  }

  project.invert = function(x, y) {
    var r0y = r0 - y;
    return [atan2(x, abs(r0y)) / n * sign(r0y), asin((c - (x * x + r0y * r0y) * n * n) / (2 * n))];
  };

  return project;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoConicEquidistant"></a>[function <span class="apidocSignatureSpan">d3.</span>geoConicEquidistant ()](#apidoc.element.d3.geoConicEquidistant)
- description and source-code
```javascript
geoConicEquidistant = function () {
  return conicProjection(conicEquidistantRaw)
      .scale(131.154)
      .center([0, 13.9389]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoConicEquidistantRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoConicEquidistantRaw (y0, y1)](#apidoc.element.d3.geoConicEquidistantRaw)
- description and source-code
```javascript
function conicEquidistantRaw(y0, y1) {
  var cy0 = cos(y0),
      n = y0 === y1 ? sin(y0) : (cy0 - cos(y1)) / (y1 - y0),
      g = cy0 / n + y0;

  if (abs(n) < epsilon) return equirectangularRaw;

  function project(x, y) {
    var gy = g - y, nx = n * x;
    return [gy * sin(nx), g - gy * cos(nx)];
  }

  project.invert = function(x, y) {
    var gy = g - y;
    return [atan2(x, abs(gy)) / n * sign(gy), g - sign(n) * sqrt(x * x + gy * gy)];
  };

  return project;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoContains"></a>[function <span class="apidocSignatureSpan">d3.</span>geoContains (object, point)](#apidoc.element.d3.geoContains)
- description and source-code
```javascript
geoContains = function (object, point) {
  return (object && containsObjectType.hasOwnProperty(object.type)
      ? containsObjectType[object.type]
      : containsGeometry)(object, point);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoDistance"></a>[function <span class="apidocSignatureSpan">d3.</span>geoDistance (a, b)](#apidoc.element.d3.geoDistance)
- description and source-code
```javascript
geoDistance = function (a, b) {
  coordinates[0] = a;
  coordinates[1] = b;
  return length(object);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoEquirectangular"></a>[function <span class="apidocSignatureSpan">d3.</span>geoEquirectangular ()](#apidoc.element.d3.geoEquirectangular)
- description and source-code
```javascript
geoEquirectangular = function () {
  return projection(equirectangularRaw)
      .scale(152.63);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoEquirectangularRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoEquirectangularRaw (lambda, phi)](#apidoc.element.d3.geoEquirectangularRaw)
- description and source-code
```javascript
function equirectangularRaw(lambda, phi) {
  return [lambda, phi];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoGnomonic"></a>[function <span class="apidocSignatureSpan">d3.</span>geoGnomonic ()](#apidoc.element.d3.geoGnomonic)
- description and source-code
```javascript
geoGnomonic = function () {
  return projection(gnomonicRaw)
      .scale(144.049)
      .clipAngle(60);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoGnomonicRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoGnomonicRaw (x, y)](#apidoc.element.d3.geoGnomonicRaw)
- description and source-code
```javascript
function gnomonicRaw(x, y) {
  var cy = cos(y), k = cos(x) * cy;
  return [cy * sin(x) / k, sin(y) / k];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoGraticule"></a>[function <span class="apidocSignatureSpan">d3.</span>geoGraticule ()](#apidoc.element.d3.geoGraticule)
- description and source-code
```javascript
function graticule() {
  var x1, x0, X1, X0,
      y1, y0, Y1, Y0,
      dx = 10, dy = dx, DX = 90, DY = 360,
      x, y, X, Y,
      precision = 2.5;

  function graticule() {
    return {type: "MultiLineString", coordinates: lines()};
  }

  function lines() {
    return d3Array.range(ceil(X0 / DX) * DX, X1, DX).map(X)
        .concat(d3Array.range(ceil(Y0 / DY) * DY, Y1, DY).map(Y))
        .concat(d3Array.range(ceil(x0 / dx) * dx, x1, dx).filter(function(x) { return abs(x % DX) > epsilon; }).map(x))
        .concat(d3Array.range(ceil(y0 / dy) * dy, y1, dy).filter(function(y) { return abs(y % DY) > epsilon; }).map(y));
  }

  graticule.lines = function() {
    return lines().map(function(coordinates) { return {type: "LineString", coordinates: coordinates}; });
  };

  graticule.outline = function() {
    return {
      type: "Polygon",
      coordinates: [
        X(X0).concat(
        Y(Y1).slice(1),
        X(X1).reverse().slice(1),
        Y(Y0).reverse().slice(1))
      ]
    };
  };

  graticule.extent = function(_) {
    if (!arguments.length) return graticule.extentMinor();
    return graticule.extentMajor(_).extentMinor(_);
  };

  graticule.extentMajor = function(_) {
    if (!arguments.length) return [[X0, Y0], [X1, Y1]];
    X0 = +_[0][0], X1 = +_[1][0];
    Y0 = +_[0][1], Y1 = +_[1][1];
    if (X0 > X1) _ = X0, X0 = X1, X1 = _;
    if (Y0 > Y1) _ = Y0, Y0 = Y1, Y1 = _;
    return graticule.precision(precision);
  };

  graticule.extentMinor = function(_) {
    if (!arguments.length) return [[x0, y0], [x1, y1]];
    x0 = +_[0][0], x1 = +_[1][0];
    y0 = +_[0][1], y1 = +_[1][1];
    if (x0 > x1) _ = x0, x0 = x1, x1 = _;
    if (y0 > y1) _ = y0, y0 = y1, y1 = _;
    return graticule.precision(precision);
  };

  graticule.step = function(_) {
    if (!arguments.length) return graticule.stepMinor();
    return graticule.stepMajor(_).stepMinor(_);
  };

  graticule.stepMajor = function(_) {
    if (!arguments.length) return [DX, DY];
    DX = +_[0], DY = +_[1];
    return graticule;
  };

  graticule.stepMinor = function(_) {
    if (!arguments.length) return [dx, dy];
    dx = +_[0], dy = +_[1];
    return graticule;
  };

  graticule.precision = function(_) {
    if (!arguments.length) return precision;
    precision = +_;
    x = graticuleX(y0, y1, 90);
    y = graticuleY(x0, x1, precision);
    X = graticuleX(Y0, Y1, 90);
    Y = graticuleY(X0, X1, precision);
    return graticule;
  };

  return graticule
      .extentMajor([[-180, -90 + epsilon], [180, 90 - epsilon]])
      .extentMinor([[-180, -80 - epsilon], [180, 80 + epsilon]]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoGraticule10"></a>[function <span class="apidocSignatureSpan">d3.</span>geoGraticule10 ()](#apidoc.element.d3.geoGraticule10)
- description and source-code
```javascript
function graticule10() {
  return graticule()();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoIdentity"></a>[function <span class="apidocSignatureSpan">d3.</span>geoIdentity ()](#apidoc.element.d3.geoIdentity)
- description and source-code
```javascript
geoIdentity = function () {
  var k = 1, tx = 0, ty = 0, sx = 1, sy = 1, transform = identity, // scale, translate and reflect
      x0 = null, y0, x1, y1, clip = identity, // clip extent
      cache,
      cacheStream,
      projection;

  function reset() {
    cache = cacheStream = null;
    return projection;
  }

  return projection = {
    stream: function(stream) {
      return cache && cacheStream === stream ? cache : cache = transform(clip(cacheStream = stream));
    },
    clipExtent: function(_) {
      return arguments.length ? (clip = _ == null ? (x0 = y0 = x1 = y1 = null, identity) : clipExtent(x0 = +_[0][0], y0 = +_[0][
1], x1 = +_[1][0], y1 = +_[1][1]), reset()) : x0 == null ? null : [[x0, y0], [x1, y1]];
    },
    scale: function(_) {
      return arguments.length ? (transform = scaleTranslate((k = +_) * sx, k * sy, tx, ty), reset()) : k;
    },
    translate: function(_) {
      return arguments.length ? (transform = scaleTranslate(k * sx, k * sy, tx = +_[0], ty = +_[1]), reset()) : [tx, ty];
    },
    reflectX: function(_) {
      return arguments.length ? (transform = scaleTranslate(k * (sx = _ ? -1 : 1), k * sy, tx, ty), reset()) : sx < 0;
    },
    reflectY: function(_) {
      return arguments.length ? (transform = scaleTranslate(k * sx, k * (sy = _ ? -1 : 1), tx, ty), reset()) : sy < 0;
    },
    fitExtent: function(extent, object) {
      return fitExtent(projection, extent, object);
    },
    fitSize: function(size, object) {
      return fitSize(projection, size, object);
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoInterpolate"></a>[function <span class="apidocSignatureSpan">d3.</span>geoInterpolate (a, b)](#apidoc.element.d3.geoInterpolate)
- description and source-code
```javascript
geoInterpolate = function (a, b) {
  var x0 = a[0] * radians,
      y0 = a[1] * radians,
      x1 = b[0] * radians,
      y1 = b[1] * radians,
      cy0 = cos(y0),
      sy0 = sin(y0),
      cy1 = cos(y1),
      sy1 = sin(y1),
      kx0 = cy0 * cos(x0),
      ky0 = cy0 * sin(x0),
      kx1 = cy1 * cos(x1),
      ky1 = cy1 * sin(x1),
      d = 2 * asin(sqrt(haversin(y1 - y0) + cy0 * cy1 * haversin(x1 - x0))),
      k = sin(d);

  var interpolate = d ? function(t) {
    var B = sin(t *= d) / k,
        A = sin(d - t) / k,
        x = A * kx0 + B * kx1,
        y = A * ky0 + B * ky1,
        z = A * sy0 + B * sy1;
    return [
      atan2(y, x) * degrees,
      atan2(z, sqrt(x * x + y * y)) * degrees
    ];
  } : function() {
    return [x0 * degrees, y0 * degrees];
  };

  interpolate.distance = d;

  return interpolate;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoLength"></a>[function <span class="apidocSignatureSpan">d3.</span>geoLength (object)](#apidoc.element.d3.geoLength)
- description and source-code
```javascript
geoLength = function (object) {
  lengthSum.reset();
  geoStream(object, lengthStream);
  return +lengthSum;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoMercator"></a>[function <span class="apidocSignatureSpan">d3.</span>geoMercator ()](#apidoc.element.d3.geoMercator)
- description and source-code
```javascript
geoMercator = function () {
  return mercatorProjection(mercatorRaw)
      .scale(961 / tau);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoMercatorRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoMercatorRaw (lambda, phi)](#apidoc.element.d3.geoMercatorRaw)
- description and source-code
```javascript
function mercatorRaw(lambda, phi) {
  return [lambda, log(tan((halfPi + phi) / 2))];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoOrthographic"></a>[function <span class="apidocSignatureSpan">d3.</span>geoOrthographic ()](#apidoc.element.d3.geoOrthographic)
- description and source-code
```javascript
geoOrthographic = function () {
  return projection(orthographicRaw)
      .scale(249.5)
      .clipAngle(90 + epsilon);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoOrthographicRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoOrthographicRaw (x, y)](#apidoc.element.d3.geoOrthographicRaw)
- description and source-code
```javascript
function orthographicRaw(x, y) {
  return [cos(y) * sin(x), sin(y)];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoPath"></a>[function <span class="apidocSignatureSpan">d3.</span>geoPath (projection, context)](#apidoc.element.d3.geoPath)
- description and source-code
```javascript
geoPath = function (projection, context) {
  var pointRadius = 4.5,
      projectionStream,
      contextStream;

  function path(object) {
    if (object) {
      if (typeof pointRadius === "function") contextStream.pointRadius(+pointRadius.apply(this, arguments));
      geoStream(object, projectionStream(contextStream));
    }
    return contextStream.result();
  }

  path.area = function(object) {
    geoStream(object, projectionStream(areaStream$1));
    return areaStream$1.result();
  };

  path.measure = function(object) {
    geoStream(object, projectionStream(lengthStream$1));
    return lengthStream$1.result();
  };

  path.bounds = function(object) {
    geoStream(object, projectionStream(boundsStream$1));
    return boundsStream$1.result();
  };

  path.centroid = function(object) {
    geoStream(object, projectionStream(centroidStream$1));
    return centroidStream$1.result();
  };

  path.projection = function(_) {
    return arguments.length ? (projectionStream = _ == null ? (projection = null, identity) : (projection = _).stream, path) : projection
;
  };

  path.context = function(_) {
    if (!arguments.length) return context;
    contextStream = _ == null ? (context = null, new PathString) : new PathContext(context = _);
    if (typeof pointRadius !== "function") contextStream.pointRadius(pointRadius);
    return path;
  };

  path.pointRadius = function(_) {
    if (!arguments.length) return pointRadius;
    pointRadius = typeof _ === "function" ? _ : (contextStream.pointRadius(+_), +_);
    return path;
  };

  return path.projection(projection).context(context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoProjection"></a>[function <span class="apidocSignatureSpan">d3.</span>geoProjection (project)](#apidoc.element.d3.geoProjection)
- description and source-code
```javascript
function projection(project) {
  return projectionMutator(function() { return project; })();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoProjectionMutator"></a>[function <span class="apidocSignatureSpan">d3.</span>geoProjectionMutator (projectAt)](#apidoc.element.d3.geoProjectionMutator)
- description and source-code
```javascript
function projectionMutator(projectAt) {
  var project,
      k = 150, // scale
      x = 480, y = 250, // translate
      dx, dy, lambda = 0, phi = 0, // center
      deltaLambda = 0, deltaPhi = 0, deltaGamma = 0, rotate, projectRotate, // rotate
      theta = null, preclip = clipAntimeridian, // clip angle
      x0 = null, y0, x1, y1, postclip = identity, // clip extent
      delta2 = 0.5, projectResample = resample(projectTransform, delta2), // precision
      cache,
      cacheStream;

  function projection(point) {
    point = projectRotate(point[0] * radians, point[1] * radians);
    return [point[0] * k + dx, dy - point[1] * k];
  }

  function invert(point) {
    point = projectRotate.invert((point[0] - dx) / k, (dy - point[1]) / k);
    return point && [point[0] * degrees, point[1] * degrees];
  }

  function projectTransform(x, y) {
    return x = project(x, y), [x[0] * k + dx, dy - x[1] * k];
  }

  projection.stream = function(stream) {
    return cache && cacheStream === stream ? cache : cache = transformRadians(preclip(rotate, projectResample(postclip(cacheStream
 = stream))));
  };

  projection.clipAngle = function(_) {
    return arguments.length ? (preclip = +_ ? clipCircle(theta = _ * radians, 6 * radians) : (theta = null, clipAntimeridian), reset
()) : theta * degrees;
  };

  projection.clipExtent = function(_) {
    return arguments.length ? (postclip = _ == null ? (x0 = y0 = x1 = y1 = null, identity) : clipExtent(x0 = +_[0][0], y0 = +_[0
][1], x1 = +_[1][0], y1 = +_[1][1]), reset()) : x0 == null ? null : [[x0, y0], [x1, y1]];
  };

  projection.scale = function(_) {
    return arguments.length ? (k = +_, recenter()) : k;
  };

  projection.translate = function(_) {
    return arguments.length ? (x = +_[0], y = +_[1], recenter()) : [x, y];
  };

  projection.center = function(_) {
    return arguments.length ? (lambda = _[0] % 360 * radians, phi = _[1] % 360 * radians, recenter()) : [lambda * degrees, phi *
degrees];
  };

  projection.rotate = function(_) {
    return arguments.length ? (deltaLambda = _[0] % 360 * radians, deltaPhi = _[1] % 360 * radians, deltaGamma = _.length > 2 ?
_[2] % 360 * radians : 0, recenter()) : [deltaLambda * degrees, deltaPhi * degrees, deltaGamma * degrees];
  };

  projection.precision = function(_) {
    return arguments.length ? (projectResample = resample(projectTransform, delta2 = _ * _), reset()) : sqrt(delta2);
  };

  projection.fitExtent = function(extent, object) {
    return fitExtent(projection, extent, object);
  };

  projection.fitSize = function(size, object) {
    return fitSize(projection, size, object);
  };

  function recenter() {
    projectRotate = compose(rotate = rotateRadians(deltaLambda, deltaPhi, deltaGamma), project);
    var center = project(lambda, phi);
    dx = x - center[0] * k;
    dy = y + center[1] * k;
    return reset();
  }

  function reset() {
    cache = cacheStream = null;
    return projection;
  }

  return function() {
    project = projectAt.apply(this, arguments);
    projection.invert = project.invert && invert;
    return recenter();
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoRotation"></a>[function <span class="apidocSignatureSpan">d3.</span>geoRotation (rotate)](#apidoc.element.d3.geoRotation)
- description and source-code
```javascript
geoRotation = function (rotate) {
  rotate = rotateRadians(rotate[0] * radians, rotate[1] * radians, rotate.length > 2 ? rotate[2] * radians : 0);

  function forward(coordinates) {
    coordinates = rotate(coordinates[0] * radians, coordinates[1] * radians);
    return coordinates[0] *= degrees, coordinates[1] *= degrees, coordinates;
  }

  forward.invert = function(coordinates) {
    coordinates = rotate.invert(coordinates[0] * radians, coordinates[1] * radians);
    return coordinates[0] *= degrees, coordinates[1] *= degrees, coordinates;
  };

  return forward;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoStereographic"></a>[function <span class="apidocSignatureSpan">d3.</span>geoStereographic ()](#apidoc.element.d3.geoStereographic)
- description and source-code
```javascript
geoStereographic = function () {
  return projection(stereographicRaw)
      .scale(250)
      .clipAngle(142);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoStereographicRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoStereographicRaw (x, y)](#apidoc.element.d3.geoStereographicRaw)
- description and source-code
```javascript
function stereographicRaw(x, y) {
  var cy = cos(y), k = 1 + cos(x) * cy;
  return [cy * sin(x) / k, sin(y) / k];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoStream"></a>[function <span class="apidocSignatureSpan">d3.</span>geoStream (object, stream)](#apidoc.element.d3.geoStream)
- description and source-code
```javascript
geoStream = function (object, stream) {
  if (object && streamObjectType.hasOwnProperty(object.type)) {
    streamObjectType[object.type](object, stream);
  } else {
    streamGeometry(object, stream);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoTransform"></a>[function <span class="apidocSignatureSpan">d3.</span>geoTransform (methods)](#apidoc.element.d3.geoTransform)
- description and source-code
```javascript
geoTransform = function (methods) {
  return {
    stream: transformer(methods)
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoTransverseMercator"></a>[function <span class="apidocSignatureSpan">d3.</span>geoTransverseMercator ()](#apidoc.element.d3.geoTransverseMercator)
- description and source-code
```javascript
geoTransverseMercator = function () {
  var m = mercatorProjection(transverseMercatorRaw),
      center = m.center,
      rotate = m.rotate;

  m.center = function(_) {
    return arguments.length ? center([-_[1], _[0]]) : (_ = center(), [_[1], -_[0]]);
  };

  m.rotate = function(_) {
    return arguments.length ? rotate([_[0], _[1], _.length > 2 ? _[2] + 90 : 90]) : (_ = rotate(), [_[0], _[1], _[2] - 90]);
  };

  return rotate([0, 0, 90])
      .scale(159.155);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoTransverseMercatorRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoTransverseMercatorRaw (lambda, phi)](#apidoc.element.d3.geoTransverseMercatorRaw)
- description and source-code
```javascript
function transverseMercatorRaw(lambda, phi) {
  return [log(tan((halfPi + phi) / 2)), -lambda];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hcl"></a>[function <span class="apidocSignatureSpan">d3.</span>hcl (h, c, l, opacity)](#apidoc.element.d3.hcl)
- description and source-code
```javascript
function hcl(h, c, l, opacity) {
  return arguments.length === 1 ? hclConvert(h) : new Hcl(h, c, l, opacity == null ? 1 : opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hcl.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>hcl.prototype.constructor (h, c, l, opacity)](#apidoc.element.d3.hcl.prototype.constructor)
- description and source-code
```javascript
function Hcl(h, c, l, opacity) {
  this.h = +h;
  this.c = +c;
  this.l = +l;
  this.opacity = +opacity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy"></a>[function <span class="apidocSignatureSpan">d3.</span>hierarchy (data, children)](#apidoc.element.d3.hierarchy)
- description and source-code
```javascript
function hierarchy(data, children) {
  var root = new Node(data),
      valued = +data.value && (root.value = data.value),
      node,
      nodes = [root],
      child,
      childs,
      i,
      n;

  if (children == null) children = defaultChildren;

  while (node = nodes.pop()) {
    if (valued) node.value = +node.data.value;
    if ((childs = children(node.data)) && (n = childs.length)) {
      node.children = new Array(n);
      for (i = n - 1; i >= 0; --i) {
        nodes.push(child = node.children[i] = new Node(childs[i]));
        child.parent = node;
        child.depth = node.depth + 1;
      }
    }
  }

  return root.eachBefore(computeHeight);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>hierarchy.prototype.constructor (data)](#apidoc.element.d3.hierarchy.prototype.constructor)
- description and source-code
```javascript
function Node(data) {
  this.data = data;
  this.depth =
  this.height = 0;
  this.parent = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.histogram"></a>[function <span class="apidocSignatureSpan">d3.</span>histogram ()](#apidoc.element.d3.histogram)
- description and source-code
```javascript
histogram = function () {
  var value = identity,
      domain = extent,
      threshold = sturges;

  function histogram(data) {
    var i,
        n = data.length,
        x,
        values = new Array(n);

    for (i = 0; i < n; ++i) {
      values[i] = value(data[i], i, data);
    }

    var xz = domain(values),
        x0 = xz[0],
        x1 = xz[1],
        tz = threshold(values, x0, x1);

    // Convert number of thresholds into uniform thresholds.
    if (!Array.isArray(tz)) tz = ticks(x0, x1, tz);

    // Remove any thresholds outside the domain.
    var m = tz.length;
    while (tz[0] <= x0) tz.shift(), --m;
    while (tz[m - 1] >= x1) tz.pop(), --m;

    var bins = new Array(m + 1),
        bin;

    // Initialize bins.
    for (i = 0; i <= m; ++i) {
      bin = bins[i] = [];
      bin.x0 = i > 0 ? tz[i - 1] : x0;
      bin.x1 = i < m ? tz[i] : x1;
    }

    // Assign data to bins by value, ignoring any outside the domain.
    for (i = 0; i < n; ++i) {
      x = values[i];
      if (x0 <= x && x <= x1) {
        bins[bisectRight(tz, x, 0, m)].push(data[i]);
      }
    }

    return bins;
  }

  histogram.value = function(_) {
    return arguments.length ? (value = typeof _ === "function" ? _ : constant(_), histogram) : value;
  };

  histogram.domain = function(_) {
    return arguments.length ? (domain = typeof _ === "function" ? _ : constant([_[0], _[1]]), histogram) : domain;
  };

  histogram.thresholds = function(_) {
    return arguments.length ? (threshold = typeof _ === "function" ? _ : Array.isArray(_) ? constant(slice.call(_)) : constant(_
), histogram) : threshold;
  };

  return histogram;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hsl"></a>[function <span class="apidocSignatureSpan">d3.</span>hsl (h, s, l, opacity)](#apidoc.element.d3.hsl)
- description and source-code
```javascript
function hsl(h, s, l, opacity) {
  return arguments.length === 1 ? hslConvert(h) : new Hsl(h, s, l, opacity == null ? 1 : opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hsl.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>hsl.prototype.constructor (h, s, l, opacity)](#apidoc.element.d3.hsl.prototype.constructor)
- description and source-code
```javascript
function Hsl(h, s, l, opacity) {
  this.h = +h;
  this.s = +s;
  this.l = +l;
  this.opacity = +opacity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.html"></a>[function <span class="apidocSignatureSpan">d3.</span>html (url, callback)](#apidoc.element.d3.html)
- description and source-code
```javascript
html = function (url, callback) {
  var r = request(url).mimeType(defaultMimeType).response(response);
  if (callback != null) {
    if (typeof callback !== "function") throw new Error("invalid callback: " + callback);
    return r.get(callback);
  }
  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolate"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolate (a, b)](#apidoc.element.d3.interpolate)
- description and source-code
```javascript
interpolate = function (a, b) {
  var t = typeof b, c;
  return b == null || t === "boolean" ? constant(b)
      : (t === "number" ? number
      : t === "string" ? ((c = d3Color.color(b)) ? (b = c, rgb$1) : string)
      : b instanceof d3Color.color ? rgb$1
      : b instanceof Date ? date
      : Array.isArray(b) ? array
      : isNaN(b) ? object
      : number)(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateArray"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateArray (a, b)](#apidoc.element.d3.interpolateArray)
- description and source-code
```javascript
interpolateArray = function (a, b) {
  var nb = b ? b.length : 0,
      na = a ? Math.min(nb, a.length) : 0,
      x = new Array(nb),
      c = new Array(nb),
      i;

  for (i = 0; i < na; ++i) x[i] = value(a[i], b[i]);
  for (; i < nb; ++i) c[i] = b[i];

  return function(t) {
    for (i = 0; i < na; ++i) c[i] = x[i](t);
    return c;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateBasis"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateBasis (values)](#apidoc.element.d3.interpolateBasis)
- description and source-code
```javascript
interpolateBasis = function (values) {
  var n = values.length - 1;
  return function(t) {
    var i = t <= 0 ? (t = 0) : t >= 1 ? (t = 1, n - 1) : Math.floor(t * n),
        v1 = values[i],
        v2 = values[i + 1],
        v0 = i > 0 ? values[i - 1] : 2 * v1 - v2,
        v3 = i < n - 1 ? values[i + 2] : 2 * v2 - v1;
    return basis((t - i / n) * n, v0, v1, v2, v3);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateBasisClosed"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateBasisClosed (values)](#apidoc.element.d3.interpolateBasisClosed)
- description and source-code
```javascript
interpolateBasisClosed = function (values) {
  var n = values.length;
  return function(t) {
    var i = Math.floor(((t %= 1) < 0 ? ++t : t) * n),
        v0 = values[(i + n - 1) % n],
        v1 = values[i % n],
        v2 = values[(i + 1) % n],
        v3 = values[(i + 2) % n];
    return basis((t - i / n) * n, v0, v1, v2, v3);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateCool"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateCool (t)](#apidoc.element.d3.interpolateCool)
- description and source-code
```javascript
interpolateCool = function (t) {
  start.h = h(t);
  start.s = s(t);
  start.l = l(Math.pow(t, y));
  start.opacity = opacity(t);
  return start + "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateCubehelix"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateCubehelix (start, end)](#apidoc.element.d3.interpolateCubehelix)
- description and source-code
```javascript
function cubehelix$$1(start, end) {
  var h = hue$$1((start = d3Color.cubehelix(start)).h, (end = d3Color.cubehelix(end)).h),
      s = nogamma(start.s, end.s),
      l = nogamma(start.l, end.l),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.h = h(t);
    start.s = s(t);
    start.l = l(Math.pow(t, y));
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateCubehelixDefault"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateCubehelixDefault (t)](#apidoc.element.d3.interpolateCubehelixDefault)
- description and source-code
```javascript
interpolateCubehelixDefault = function (t) {
  start.h = h(t);
  start.s = s(t);
  start.l = l(Math.pow(t, y));
  start.opacity = opacity(t);
  return start + "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateCubehelixLong"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateCubehelixLong (start, end)](#apidoc.element.d3.interpolateCubehelixLong)
- description and source-code
```javascript
function cubehelix$$1(start, end) {
  var h = hue$$1((start = d3Color.cubehelix(start)).h, (end = d3Color.cubehelix(end)).h),
      s = nogamma(start.s, end.s),
      l = nogamma(start.l, end.l),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.h = h(t);
    start.s = s(t);
    start.l = l(Math.pow(t, y));
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateDate"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateDate (a, b)](#apidoc.element.d3.interpolateDate)
- description and source-code
```javascript
interpolateDate = function (a, b) {
  var d = new Date;
  return a = +a, b -= a, function(t) {
    return d.setTime(a + b * t), d;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateHcl"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateHcl (start, end)](#apidoc.element.d3.interpolateHcl)
- description and source-code
```javascript
interpolateHcl = function (start, end) {
  var h = hue$$1((start = d3Color.hcl(start)).h, (end = d3Color.hcl(end)).h),
      c = nogamma(start.c, end.c),
      l = nogamma(start.l, end.l),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.h = h(t);
    start.c = c(t);
    start.l = l(t);
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateHclLong"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateHclLong (start, end)](#apidoc.element.d3.interpolateHclLong)
- description and source-code
```javascript
interpolateHclLong = function (start, end) {
  var h = hue$$1((start = d3Color.hcl(start)).h, (end = d3Color.hcl(end)).h),
      c = nogamma(start.c, end.c),
      l = nogamma(start.l, end.l),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.h = h(t);
    start.c = c(t);
    start.l = l(t);
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateHsl"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateHsl (start, end)](#apidoc.element.d3.interpolateHsl)
- description and source-code
```javascript
interpolateHsl = function (start, end) {
  var h = hue$$1((start = d3Color.hsl(start)).h, (end = d3Color.hsl(end)).h),
      s = nogamma(start.s, end.s),
      l = nogamma(start.l, end.l),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.h = h(t);
    start.s = s(t);
    start.l = l(t);
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateHslLong"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateHslLong (start, end)](#apidoc.element.d3.interpolateHslLong)
- description and source-code
```javascript
interpolateHslLong = function (start, end) {
  var h = hue$$1((start = d3Color.hsl(start)).h, (end = d3Color.hsl(end)).h),
      s = nogamma(start.s, end.s),
      l = nogamma(start.l, end.l),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.h = h(t);
    start.s = s(t);
    start.l = l(t);
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateInferno"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateInferno (t)](#apidoc.element.d3.interpolateInferno)
- description and source-code
```javascript
interpolateInferno = function (t) {
  return range$$1[Math.max(0, Math.min(n - 1, Math.floor(t * n)))];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateLab"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateLab (start, end)](#apidoc.element.d3.interpolateLab)
- description and source-code
```javascript
function lab$1(start, end) {
  var l = nogamma((start = d3Color.lab(start)).l, (end = d3Color.lab(end)).l),
      a = nogamma(start.a, end.a),
      b = nogamma(start.b, end.b),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.l = l(t);
    start.a = a(t);
    start.b = b(t);
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateMagma"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateMagma (t)](#apidoc.element.d3.interpolateMagma)
- description and source-code
```javascript
interpolateMagma = function (t) {
  return range$$1[Math.max(0, Math.min(n - 1, Math.floor(t * n)))];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateNumber"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateNumber (a, b)](#apidoc.element.d3.interpolateNumber)
- description and source-code
```javascript
interpolateNumber = function (a, b) {
  return a = +a, b -= a, function(t) {
    return a + b * t;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateObject"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateObject (a, b)](#apidoc.element.d3.interpolateObject)
- description and source-code
```javascript
interpolateObject = function (a, b) {
  var i = {},
      c = {},
      k;

  if (a === null || typeof a !== "object") a = {};
  if (b === null || typeof b !== "object") b = {};

  for (k in b) {
    if (k in a) {
      i[k] = value(a[k], b[k]);
    } else {
      c[k] = b[k];
    }
  }

  return function(t) {
    for (k in i) c[k] = i[k](t);
    return c;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolatePlasma"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolatePlasma (t)](#apidoc.element.d3.interpolatePlasma)
- description and source-code
```javascript
interpolatePlasma = function (t) {
  return range$$1[Math.max(0, Math.min(n - 1, Math.floor(t * n)))];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateRainbow"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateRainbow (t)](#apidoc.element.d3.interpolateRainbow)
- description and source-code
```javascript
interpolateRainbow = function (t) {
  if (t < 0 || t > 1) t -= Math.floor(t);
  var ts = Math.abs(t - 0.5);
  rainbow.h = 360 * t - 100;
  rainbow.s = 1.5 - 1.5 * ts;
  rainbow.l = 0.8 - 0.9 * ts;
  return rainbow + "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateRgb"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateRgb (start, end)](#apidoc.element.d3.interpolateRgb)
- description and source-code
```javascript
function rgb$$1(start, end) {
  var r = color$$1((start = d3Color.rgb(start)).r, (end = d3Color.rgb(end)).r),
      g = color$$1(start.g, end.g),
      b = color$$1(start.b, end.b),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.r = r(t);
    start.g = g(t);
    start.b = b(t);
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateRgbBasis"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateRgbBasis (colors)](#apidoc.element.d3.interpolateRgbBasis)
- description and source-code
```javascript
interpolateRgbBasis = function (colors) {
  var n = colors.length,
      r = new Array(n),
      g = new Array(n),
      b = new Array(n),
      i, color$$1;
  for (i = 0; i < n; ++i) {
    color$$1 = d3Color.rgb(colors[i]);
    r[i] = color$$1.r || 0;
    g[i] = color$$1.g || 0;
    b[i] = color$$1.b || 0;
  }
  r = spline(r);
  g = spline(g);
  b = spline(b);
  color$$1.opacity = 1;
  return function(t) {
    color$$1.r = r(t);
    color$$1.g = g(t);
    color$$1.b = b(t);
    return color$$1 + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateRgbBasisClosed"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateRgbBasisClosed (colors)](#apidoc.element.d3.interpolateRgbBasisClosed)
- description and source-code
```javascript
interpolateRgbBasisClosed = function (colors) {
  var n = colors.length,
      r = new Array(n),
      g = new Array(n),
      b = new Array(n),
      i, color$$1;
  for (i = 0; i < n; ++i) {
    color$$1 = d3Color.rgb(colors[i]);
    r[i] = color$$1.r || 0;
    g[i] = color$$1.g || 0;
    b[i] = color$$1.b || 0;
  }
  r = spline(r);
  g = spline(g);
  b = spline(b);
  color$$1.opacity = 1;
  return function(t) {
    color$$1.r = r(t);
    color$$1.g = g(t);
    color$$1.b = b(t);
    return color$$1 + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateRound"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateRound (a, b)](#apidoc.element.d3.interpolateRound)
- description and source-code
```javascript
interpolateRound = function (a, b) {
  return a = +a, b -= a, function(t) {
    return Math.round(a + b * t);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateString"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateString (a, b)](#apidoc.element.d3.interpolateString)
- description and source-code
```javascript
interpolateString = function (a, b) {
  var bi = reA.lastIndex = reB.lastIndex = 0, // scan index for next number in b
      am, // current match in a
      bm, // current match in b
      bs, // string preceding current number in b, if any
      i = -1, // index in s
      s = [], // string constants and placeholders
      q = []; // number interpolators

  // Coerce inputs to strings.
  a = a + "", b = b + "";

  // Interpolate pairs of numbers in a & b.
  while ((am = reA.exec(a))
      && (bm = reB.exec(b))) {
    if ((bs = bm.index) > bi) { // a string precedes the next number in b
      bs = b.slice(bi, bs);
      if (s[i]) s[i] += bs; // coalesce with previous string
      else s[++i] = bs;
    }
    if ((am = am[0]) === (bm = bm[0])) { // numbers in a & b match
      if (s[i]) s[i] += bm; // coalesce with previous string
      else s[++i] = bm;
    } else { // interpolate non-matching numbers
      s[++i] = null;
      q.push({i: i, x: number(am, bm)});
    }
    bi = reB.lastIndex;
  }

  // Add remains of b.
  if (bi < b.length) {
    bs = b.slice(bi);
    if (s[i]) s[i] += bs; // coalesce with previous string
    else s[++i] = bs;
  }

  // Special optimization for only a single match.
  // Otherwise, interpolate each of the numbers and rejoin the string.
  return s.length < 2 ? (q[0]
      ? one(q[0].x)
      : zero(b))
      : (b = q.length, function(t) {
          for (var i = 0, o; i < b; ++i) s[(o = q[i]).i] = o.x(t);
          return s.join("");
        });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateTransformCss"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateTransformCss (a, b)](#apidoc.element.d3.interpolateTransformCss)
- description and source-code
```javascript
interpolateTransformCss = function (a, b) {
  var s = [], // string constants and placeholders
      q = []; // number interpolators
  a = parse(a), b = parse(b);
  translate(a.translateX, a.translateY, b.translateX, b.translateY, s, q);
  rotate(a.rotate, b.rotate, s, q);
  skewX(a.skewX, b.skewX, s, q);
  scale(a.scaleX, a.scaleY, b.scaleX, b.scaleY, s, q);
  a = b = null; // gc
  return function(t) {
    var i = -1, n = q.length, o;
    while (++i < n) s[(o = q[i]).i] = o.x(t);
    return s.join("");
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateTransformSvg"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateTransformSvg (a, b)](#apidoc.element.d3.interpolateTransformSvg)
- description and source-code
```javascript
interpolateTransformSvg = function (a, b) {
  var s = [], // string constants and placeholders
      q = []; // number interpolators
  a = parse(a), b = parse(b);
  translate(a.translateX, a.translateY, b.translateX, b.translateY, s, q);
  rotate(a.rotate, b.rotate, s, q);
  skewX(a.skewX, b.skewX, s, q);
  scale(a.scaleX, a.scaleY, b.scaleX, b.scaleY, s, q);
  a = b = null; // gc
  return function(t) {
    var i = -1, n = q.length, o;
    while (++i < n) s[(o = q[i]).i] = o.x(t);
    return s.join("");
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateViridis"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateViridis (t)](#apidoc.element.d3.interpolateViridis)
- description and source-code
```javascript
interpolateViridis = function (t) {
  return range$$1[Math.max(0, Math.min(n - 1, Math.floor(t * n)))];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateWarm"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateWarm (t)](#apidoc.element.d3.interpolateWarm)
- description and source-code
```javascript
interpolateWarm = function (t) {
  start.h = h(t);
  start.s = s(t);
  start.l = l(Math.pow(t, y));
  start.opacity = opacity(t);
  return start + "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateZoom"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateZoom (p0, p1)](#apidoc.element.d3.interpolateZoom)
- description and source-code
```javascript
interpolateZoom = function (p0, p1) {
  var ux0 = p0[0], uy0 = p0[1], w0 = p0[2],
      ux1 = p1[0], uy1 = p1[1], w1 = p1[2],
      dx = ux1 - ux0,
      dy = uy1 - uy0,
      d2 = dx * dx + dy * dy,
      i,
      S;

  // Special case for u0 ≅ u1.
  if (d2 < epsilon2) {
    S = Math.log(w1 / w0) / rho;
    i = function(t) {
      return [
        ux0 + t * dx,
        uy0 + t * dy,
        w0 * Math.exp(rho * t * S)
      ];
    };
  }

  // General case.
  else {
    var d1 = Math.sqrt(d2),
        b0 = (w1 * w1 - w0 * w0 + rho4 * d2) / (2 * w0 * rho2 * d1),
        b1 = (w1 * w1 - w0 * w0 - rho4 * d2) / (2 * w1 * rho2 * d1),
        r0 = Math.log(Math.sqrt(b0 * b0 + 1) - b0),
        r1 = Math.log(Math.sqrt(b1 * b1 + 1) - b1);
    S = (r1 - r0) / rho;
    i = function(t) {
      var s = t * S,
          coshr0 = cosh(r0),
          u = w0 / (rho2 * d1) * (coshr0 * tanh(rho * s + r0) - sinh(r0));
      return [
        ux0 + u * dx,
        uy0 + u * dy,
        w0 * coshr0 / cosh(rho * s + r0)
      ];
    };
  }

  i.duration = S * 1000;

  return i;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interrupt"></a>[function <span class="apidocSignatureSpan">d3.</span>interrupt (node, name)](#apidoc.element.d3.interrupt)
- description and source-code
```javascript
interrupt = function (node, name) {
  var schedules = node.__transition,
      schedule,
      active,
      empty = true,
      i;

  if (!schedules) return;

  name = name == null ? null : name + "";

  for (i in schedules) {
    if ((schedule = schedules[i]).name !== name) { empty = false; continue; }
    active = schedule.state > STARTING && schedule.state < ENDING;
    schedule.state = ENDED;
    schedule.timer.stop();
    if (active) schedule.on.call("interrupt", node, node.__data__, schedule.index, schedule.group);
    delete schedules[i];
  }

  if (empty) delete node.__transition;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interval"></a>[function <span class="apidocSignatureSpan">d3.</span>interval (callback, delay, time)](#apidoc.element.d3.interval)
- description and source-code
```javascript
interval = function (callback, delay, time) {
  var t = new Timer, total = delay;
  if (delay == null) return t.restart(callback, delay, time), t;
  delay = +delay, time = time == null ? now() : +time;
  t.restart(function tick(elapsed) {
    elapsed += total;
    t.restart(tick, total += delay, time);
    callback(elapsed);
  }, delay, time);
  return t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.isoFormat"></a>[function <span class="apidocSignatureSpan">d3.</span>isoFormat (date)](#apidoc.element.d3.isoFormat)
- description and source-code
```javascript
function formatIsoNative(date) {
  return date.toISOString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.isoParse"></a>[function <span class="apidocSignatureSpan">d3.</span>isoParse (string)](#apidoc.element.d3.isoParse)
- description and source-code
```javascript
function parseIsoNative(string) {
  var date = new Date(string);
  return isNaN(date) ? null : date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.json"></a>[function <span class="apidocSignatureSpan">d3.</span>json (url, callback)](#apidoc.element.d3.json)
- description and source-code
```javascript
json = function (url, callback) {
  var r = request(url).mimeType(defaultMimeType).response(response);
  if (callback != null) {
    if (typeof callback !== "function") throw new Error("invalid callback: " + callback);
    return r.get(callback);
  }
  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.keys"></a>[function <span class="apidocSignatureSpan">d3.</span>keys (map)](#apidoc.element.d3.keys)
- description and source-code
```javascript
keys = function (map) {
  var keys = [];
  for (var key in map) keys.push(key);
  return keys;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.lab"></a>[function <span class="apidocSignatureSpan">d3.</span>lab (l, a, b, opacity)](#apidoc.element.d3.lab)
- description and source-code
```javascript
function lab(l, a, b, opacity) {
  return arguments.length === 1 ? labConvert(l) : new Lab(l, a, b, opacity == null ? 1 : opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.lab.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>lab.prototype.constructor (l, a, b, opacity)](#apidoc.element.d3.lab.prototype.constructor)
- description and source-code
```javascript
function Lab(l, a, b, opacity) {
  this.l = +l;
  this.a = +a;
  this.b = +b;
  this.opacity = +opacity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.line"></a>[function <span class="apidocSignatureSpan">d3.</span>line ()](#apidoc.element.d3.line)
- description and source-code
```javascript
line = function () {
  var x$$1 = x,
      y$$1 = y,
      defined = constant(true),
      context = null,
      curve = curveLinear,
      output = null;

  function line(data) {
    var i,
        n = data.length,
        d,
        defined0 = false,
        buffer;

    if (context == null) output = curve(buffer = d3Path.path());

    for (i = 0; i <= n; ++i) {
      if (!(i < n && defined(d = data[i], i, data)) === defined0) {
        if (defined0 = !defined0) output.lineStart();
        else output.lineEnd();
      }
      if (defined0) output.point(+x$$1(d, i, data), +y$$1(d, i, data));
    }

    if (buffer) return output = null, buffer + "" || null;
  }

  line.x = function(_) {
    return arguments.length ? (x$$1 = typeof _ === "function" ? _ : constant(+_), line) : x$$1;
  };

  line.y = function(_) {
    return arguments.length ? (y$$1 = typeof _ === "function" ? _ : constant(+_), line) : y$$1;
  };

  line.defined = function(_) {
    return arguments.length ? (defined = typeof _ === "function" ? _ : constant(!!_), line) : defined;
  };

  line.curve = function(_) {
    return arguments.length ? (curve = _, context != null && (output = curve(context)), line) : curve;
  };

  line.context = function(_) {
    return arguments.length ? (_ == null ? context = output = null : output = curve(context = _), line) : context;
  };

  return line;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.local"></a>[function <span class="apidocSignatureSpan">d3.</span>local ()](#apidoc.element.d3.local)
- description and source-code
```javascript
function local() {
  return new Local;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.local.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>local.prototype.constructor ()](#apidoc.element.d3.local.prototype.constructor)
- description and source-code
```javascript
function Local() {
  this._ = "@" + (++nextId).toString(36);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map"></a>[function <span class="apidocSignatureSpan">d3.</span>map (object, f)](#apidoc.element.d3.map)
- description and source-code
```javascript
function map(object, f) {
  var map = new Map;

  // Copy constructor.
  if (object instanceof Map) object.each(function(value, key) { map.set(key, value); });

  // Index array by numeric index or specified key function.
  else if (Array.isArray(object)) {
    var i = -1,
        n = object.length,
        o;

    if (f == null) while (++i < n) map.set(i, object[i]);
    else while (++i < n) map.set(f(o = object[i], i, object), o);
  }

  // Convert object to map.
  else if (object) for (var key in object) map.set(key, object[key]);

  return map;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>map.prototype.constructor ()](#apidoc.element.d3.map.prototype.constructor)
- description and source-code
```javascript
function Map() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.matcher"></a>[function <span class="apidocSignatureSpan">d3.</span>matcher (selector)](#apidoc.element.d3.matcher)
- description and source-code
```javascript
matcher = function (selector) {
  return function() {
    return this.matches(selector);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.max"></a>[function <span class="apidocSignatureSpan">d3.</span>max (array, f)](#apidoc.element.d3.max)
- description and source-code
```javascript
max = function (array, f) {
  var i = -1,
      n = array.length,
      a,
      b;

  if (f == null) {
    while (++i < n) if ((b = array[i]) != null && b >= b) { a = b; break; }
    while (++i < n) if ((b = array[i]) != null && b > a) a = b;
  }

  else {
    while (++i < n) if ((b = f(array[i], i, array)) != null && b >= b) { a = b; break; }
    while (++i < n) if ((b = f(array[i], i, array)) != null && b > a) a = b;
  }

  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.mean"></a>[function <span class="apidocSignatureSpan">d3.</span>mean (array, f)](#apidoc.element.d3.mean)
- description and source-code
```javascript
mean = function (array, f) {
  var s = 0,
      n = array.length,
      a,
      i = -1,
      j = n;

  if (f == null) {
    while (++i < n) if (!isNaN(a = number(array[i]))) s += a; else --j;
  }

  else {
    while (++i < n) if (!isNaN(a = number(f(array[i], i, array)))) s += a; else --j;
  }

  if (j) return s / j;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.median"></a>[function <span class="apidocSignatureSpan">d3.</span>median (array, f)](#apidoc.element.d3.median)
- description and source-code
```javascript
median = function (array, f) {
  var numbers = [],
      n = array.length,
      a,
      i = -1;

  if (f == null) {
    while (++i < n) if (!isNaN(a = number(array[i]))) numbers.push(a);
  }

  else {
    while (++i < n) if (!isNaN(a = number(f(array[i], i, array)))) numbers.push(a);
  }

  return quantile(numbers.sort(ascending), 0.5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.merge"></a>[function <span class="apidocSignatureSpan">d3.</span>merge (arrays)](#apidoc.element.d3.merge)
- description and source-code
```javascript
merge = function (arrays) {
  var n = arrays.length,
      m,
      i = -1,
      j = 0,
      merged,
      array;

  while (++i < n) j += arrays[i].length;
  merged = new Array(j);

  while (--n >= 0) {
    array = arrays[n];
    m = array.length;
    while (--m >= 0) {
      merged[--j] = array[m];
    }
  }

  return merged;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.min"></a>[function <span class="apidocSignatureSpan">d3.</span>min (array, f)](#apidoc.element.d3.min)
- description and source-code
```javascript
min = function (array, f) {
  var i = -1,
      n = array.length,
      a,
      b;

  if (f == null) {
    while (++i < n) if ((b = array[i]) != null && b >= b) { a = b; break; }
    while (++i < n) if ((b = array[i]) != null && a > b) a = b;
  }

  else {
    while (++i < n) if ((b = f(array[i], i, array)) != null && b >= b) { a = b; break; }
    while (++i < n) if ((b = f(array[i], i, array)) != null && a > b) a = b;
  }

  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.mouse"></a>[function <span class="apidocSignatureSpan">d3.</span>mouse (node)](#apidoc.element.d3.mouse)
- description and source-code
```javascript
mouse = function (node) {
  var event = sourceEvent();
  if (event.changedTouches) event = event.changedTouches[0];
  return point(node, event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.namespace"></a>[function <span class="apidocSignatureSpan">d3.</span>namespace (name)](#apidoc.element.d3.namespace)
- description and source-code
```javascript
namespace = function (name) {
  var prefix = name += "", i = prefix.indexOf(":");
  if (i >= 0 && (prefix = name.slice(0, i)) !== "xmlns") name = name.slice(i + 1);
  return namespaces.hasOwnProperty(prefix) ? {space: namespaces[prefix], local: name} : name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.nest"></a>[function <span class="apidocSignatureSpan">d3.</span>nest ()](#apidoc.element.d3.nest)
- description and source-code
```javascript
nest = function () {
  var keys = [],
      sortKeys = [],
      sortValues,
      rollup,
      nest;

  function apply(array, depth, createResult, setResult) {
    if (depth >= keys.length) return rollup != null
        ? rollup(array) : (sortValues != null
        ? array.sort(sortValues)
        : array);

    var i = -1,
        n = array.length,
        key = keys[depth++],
        keyValue,
        value,
        valuesByKey = map(),
        values,
        result = createResult();

    while (++i < n) {
      if (values = valuesByKey.get(keyValue = key(value = array[i]) + "")) {
        values.push(value);
      } else {
        valuesByKey.set(keyValue, [value]);
      }
    }

    valuesByKey.each(function(values, key) {
      setResult(result, key, apply(values, depth, createResult, setResult));
    });

    return result;
  }

  function entries(map$$1, depth) {
    if (++depth > keys.length) return map$$1;
    var array, sortKey = sortKeys[depth - 1];
    if (rollup != null && depth >= keys.length) array = map$$1.entries();
    else array = [], map$$1.each(function(v, k) { array.push({key: k, values: entries(v, depth)}); });
    return sortKey != null ? array.sort(function(a, b) { return sortKey(a.key, b.key); }) : array;
  }

  return nest = {
    object: function(array) { return apply(array, 0, createObject, setObject); },
    map: function(array) { return apply(array, 0, createMap, setMap); },
    entries: function(array) { return entries(apply(array, 0, createMap, setMap), 0); },
    key: function(d) { keys.push(d); return nest; },
    sortKeys: function(order) { sortKeys[keys.length - 1] = order; return nest; },
    sortValues: function(order) { sortValues = order; return nest; },
    rollup: function(f) { rollup = f; return nest; }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.now"></a>[function <span class="apidocSignatureSpan">d3.</span>now ()](#apidoc.element.d3.now)
- description and source-code
```javascript
function now() {
  return clockNow || (setFrame(clearNow), clockNow = clock.now() + clockSkew);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.pack"></a>[function <span class="apidocSignatureSpan">d3.</span>pack ()](#apidoc.element.d3.pack)
- description and source-code
```javascript
pack = function () {
  var radius = null,
      dx = 1,
      dy = 1,
      padding = constantZero;

  function pack(root) {
    root.x = dx / 2, root.y = dy / 2;
    if (radius) {
      root.eachBefore(radiusLeaf(radius))
          .eachAfter(packChildren(padding, 0.5))
          .eachBefore(translateChild(1));
    } else {
      root.eachBefore(radiusLeaf(defaultRadius))
          .eachAfter(packChildren(constantZero, 1))
          .eachAfter(packChildren(padding, root.r / Math.min(dx, dy)))
          .eachBefore(translateChild(Math.min(dx, dy) / (2 * root.r)));
    }
    return root;
  }

  pack.radius = function(x) {
    return arguments.length ? (radius = optional(x), pack) : radius;
  };

  pack.size = function(x) {
    return arguments.length ? (dx = +x[0], dy = +x[1], pack) : [dx, dy];
  };

  pack.padding = function(x) {
    return arguments.length ? (padding = typeof x === "function" ? x : constant(+x), pack) : padding;
  };

  return pack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.packEnclose"></a>[function <span class="apidocSignatureSpan">d3.</span>packEnclose (circles)](#apidoc.element.d3.packEnclose)
- description and source-code
```javascript
packEnclose = function (circles) {
  return encloseN(shuffle(circles), []);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.packSiblings"></a>[function <span class="apidocSignatureSpan">d3.</span>packSiblings (circles)](#apidoc.element.d3.packSiblings)
- description and source-code
```javascript
packSiblings = function (circles) {
  packEnclose(circles);
  return circles;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.pairs"></a>[function <span class="apidocSignatureSpan">d3.</span>pairs (array, f)](#apidoc.element.d3.pairs)
- description and source-code
```javascript
pairs = function (array, f) {
  if (f == null) f = pair;
  var i = 0, n = array.length - 1, p = array[0], pairs = new Array(n < 0 ? 0 : n);
  while (i < n) pairs[i] = f(p, p = array[++i]);
  return pairs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.partition"></a>[function <span class="apidocSignatureSpan">d3.</span>partition ()](#apidoc.element.d3.partition)
- description and source-code
```javascript
partition = function () {
  var dx = 1,
      dy = 1,
      padding = 0,
      round = false;

  function partition(root) {
    var n = root.height + 1;
    root.x0 =
    root.y0 = padding;
    root.x1 = dx;
    root.y1 = dy / n;
    root.eachBefore(positionNode(dy, n));
    if (round) root.eachBefore(roundNode);
    return root;
  }

  function positionNode(dy, n) {
    return function(node) {
      if (node.children) {
        treemapDice(node, node.x0, dy * (node.depth + 1) / n, node.x1, dy * (node.depth + 2) / n);
      }
      var x0 = node.x0,
          y0 = node.y0,
          x1 = node.x1 - padding,
          y1 = node.y1 - padding;
      if (x1 < x0) x0 = x1 = (x0 + x1) / 2;
      if (y1 < y0) y0 = y1 = (y0 + y1) / 2;
      node.x0 = x0;
      node.y0 = y0;
      node.x1 = x1;
      node.y1 = y1;
    };
  }

  partition.round = function(x) {
    return arguments.length ? (round = !!x, partition) : round;
  };

  partition.size = function(x) {
    return arguments.length ? (dx = +x[0], dy = +x[1], partition) : [dx, dy];
  };

  partition.padding = function(x) {
    return arguments.length ? (padding = +x, partition) : padding;
  };

  return partition;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path"></a>[function <span class="apidocSignatureSpan">d3.</span>path ()](#apidoc.element.d3.path)
- description and source-code
```javascript
function path() {
  return new Path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>path.prototype.constructor ()](#apidoc.element.d3.path.prototype.constructor)
- description and source-code
```javascript
function Path() {
  this._x0 = this._y0 = // start of current subpath
  this._x1 = this._y1 = null; // end of current subpath
  this._ = "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.permute"></a>[function <span class="apidocSignatureSpan">d3.</span>permute (array, indexes)](#apidoc.element.d3.permute)
- description and source-code
```javascript
permute = function (array, indexes) {
  var i = indexes.length, permutes = new Array(i);
  while (i--) permutes[i] = array[indexes[i]];
  return permutes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.pie"></a>[function <span class="apidocSignatureSpan">d3.</span>pie ()](#apidoc.element.d3.pie)
- description and source-code
```javascript
pie = function () {
  var value = identity,
      sortValues = descending,
      sort = null,
      startAngle = constant(0),
      endAngle = constant(tau),
      padAngle = constant(0);

  function pie(data) {
    var i,
        n = data.length,
        j,
        k,
        sum = 0,
        index = new Array(n),
        arcs = new Array(n),
        a0 = +startAngle.apply(this, arguments),
        da = Math.min(tau, Math.max(-tau, endAngle.apply(this, arguments) - a0)),
        a1,
        p = Math.min(Math.abs(da) / n, padAngle.apply(this, arguments)),
        pa = p * (da < 0 ? -1 : 1),
        v;

    for (i = 0; i < n; ++i) {
      if ((v = arcs[index[i] = i] = +value(data[i], i, data)) > 0) {
        sum += v;
      }
    }

    // Optionally sort the arcs by previously-computed values or by data.
    if (sortValues != null) index.sort(function(i, j) { return sortValues(arcs[i], arcs[j]); });
    else if (sort != null) index.sort(function(i, j) { return sort(data[i], data[j]); });

    // Compute the arcs! They are stored in the original data's order.
    for (i = 0, k = sum ? (da - n * pa) / sum : 0; i < n; ++i, a0 = a1) {
      j = index[i], v = arcs[j], a1 = a0 + (v > 0 ? v * k : 0) + pa, arcs[j] = {
        data: data[j],
        index: i,
        value: v,
        startAngle: a0,
        endAngle: a1,
        padAngle: p
      };
    }

    return arcs;
  }

  pie.value = function(_) {
    return arguments.length ? (value = typeof _ === "function" ? _ : constant(+_), pie) : value;
  };

  pie.sortValues = function(_) {
    return arguments.length ? (sortValues = _, sort = null, pie) : sortValues;
  };

  pie.sort = function(_) {
    return arguments.length ? (sort = _, sortValues = null, pie) : sort;
  };

  pie.startAngle = function(_) {
    return arguments.length ? (startAngle = typeof _ === "function" ? _ : constant(+_), pie) : startAngle;
  };

  pie.endAngle = function(_) {
    return arguments.length ? (endAngle = typeof _ === "function" ? _ : constant(+_), pie) : endAngle;
  };

  pie.padAngle = function(_) {
    return arguments.length ? (padAngle = typeof _ === "function" ? _ : constant(+_), pie) : padAngle;
  };

  return pie;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.polygonArea"></a>[function <span class="apidocSignatureSpan">d3.</span>polygonArea (polygon)](#apidoc.element.d3.polygonArea)
- description and source-code
```javascript
polygonArea = function (polygon) {
  var i = -1,
      n = polygon.length,
      a,
      b = polygon[n - 1],
      area = 0;

  while (++i < n) {
    a = b;
    b = polygon[i];
    area += a[1] * b[0] - a[0] * b[1];
  }

  return area / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.polygonCentroid"></a>[function <span class="apidocSignatureSpan">d3.</span>polygonCentroid (polygon)](#apidoc.element.d3.polygonCentroid)
- description and source-code
```javascript
polygonCentroid = function (polygon) {
  var i = -1,
      n = polygon.length,
      x = 0,
      y = 0,
      a,
      b = polygon[n - 1],
      c,
      k = 0;

  while (++i < n) {
    a = b;
    b = polygon[i];
    k += c = a[0] * b[1] - b[0] * a[1];
    x += (a[0] + b[0]) * c;
    y += (a[1] + b[1]) * c;
  }

  return k *= 3, [x / k, y / k];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.polygonContains"></a>[function <span class="apidocSignatureSpan">d3.</span>polygonContains (polygon, point)](#apidoc.element.d3.polygonContains)
- description and source-code
```javascript
polygonContains = function (polygon, point) {
  var n = polygon.length,
      p = polygon[n - 1],
      x = point[0], y = point[1],
      x0 = p[0], y0 = p[1],
      x1, y1,
      inside = false;

  for (var i = 0; i < n; ++i) {
    p = polygon[i], x1 = p[0], y1 = p[1];
    if (((y1 > y) !== (y0 > y)) && (x < (x0 - x1) * (y - y1) / (y0 - y1) + x1)) inside = !inside;
    x0 = x1, y0 = y1;
  }

  return inside;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.polygonHull"></a>[function <span class="apidocSignatureSpan">d3.</span>polygonHull (points)](#apidoc.element.d3.polygonHull)
- description and source-code
```javascript
polygonHull = function (points) {
  if ((n = points.length) < 3) return null;

  var i,
      n,
      sortedPoints = new Array(n),
      flippedPoints = new Array(n);

  for (i = 0; i < n; ++i) sortedPoints[i] = [+points[i][0], +points[i][1], i];
  sortedPoints.sort(lexicographicOrder);
  for (i = 0; i < n; ++i) flippedPoints[i] = [sortedPoints[i][0], -sortedPoints[i][1]];

  var upperIndexes = computeUpperHullIndexes(sortedPoints),
      lowerIndexes = computeUpperHullIndexes(flippedPoints);

  // Construct the hull polygon, removing possible duplicate endpoints.
  var skipLeft = lowerIndexes[0] === upperIndexes[0],
      skipRight = lowerIndexes[lowerIndexes.length - 1] === upperIndexes[upperIndexes.length - 1],
      hull = [];

  // Add upper hull in right-to-l order.
  // Then add lower hull in left-to-right order.
  for (i = upperIndexes.length - 1; i >= 0; --i) hull.push(points[sortedPoints[upperIndexes[i]][2]]);
  for (i = +skipLeft; i < lowerIndexes.length - skipRight; ++i) hull.push(points[sortedPoints[lowerIndexes[i]][2]]);

  return hull;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.polygonLength"></a>[function <span class="apidocSignatureSpan">d3.</span>polygonLength (polygon)](#apidoc.element.d3.polygonLength)
- description and source-code
```javascript
polygonLength = function (polygon) {
  var i = -1,
      n = polygon.length,
      b = polygon[n - 1],
      xa,
      ya,
      xb = b[0],
      yb = b[1],
      perimeter = 0;

  while (++i < n) {
    xa = xb;
    ya = yb;
    b = polygon[i];
    xb = b[0];
    yb = b[1];
    xa -= xb;
    ya -= yb;
    perimeter += Math.sqrt(xa * xa + ya * ya);
  }

  return perimeter;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.precisionFixed"></a>[function <span class="apidocSignatureSpan">d3.</span>precisionFixed (step)](#apidoc.element.d3.precisionFixed)
- description and source-code
```javascript
precisionFixed = function (step) {
  return Math.max(0, -exponent(Math.abs(step)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.precisionPrefix"></a>[function <span class="apidocSignatureSpan">d3.</span>precisionPrefix (step, value)](#apidoc.element.d3.precisionPrefix)
- description and source-code
```javascript
precisionPrefix = function (step, value) {
  return Math.max(0, Math.max(-8, Math.min(8, Math.floor(exponent(value) / 3))) * 3 - exponent(Math.abs(step)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.precisionRound"></a>[function <span class="apidocSignatureSpan">d3.</span>precisionRound (step, max)](#apidoc.element.d3.precisionRound)
- description and source-code
```javascript
precisionRound = function (step, max) {
  step = Math.abs(step), max = Math.abs(max) - step;
  return Math.max(0, exponent(max) - exponent(step)) + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree"></a>[function <span class="apidocSignatureSpan">d3.</span>quadtree (nodes, x, y)](#apidoc.element.d3.quadtree)
- description and source-code
```javascript
function quadtree(nodes, x, y) {
  var tree = new Quadtree(x == null ? defaultX : x, y == null ? defaultY : y, NaN, NaN, NaN, NaN);
  return nodes == null ? tree : tree.addAll(nodes);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quantile"></a>[function <span class="apidocSignatureSpan">d3.</span>quantile (array, p, f)](#apidoc.element.d3.quantile)
- description and source-code
```javascript
quantile = function (array, p, f) {
  if (f == null) f = number;
  if (!(n = array.length)) return;
  if ((p = +p) <= 0 || n < 2) return +f(array[0], 0, array);
  if (p >= 1) return +f(array[n - 1], n - 1, array);
  var n,
      h = (n - 1) * p,
      i = Math.floor(h),
      a = +f(array[i], i, array),
      b = +f(array[i + 1], i + 1, array);
  return a + (b - a) * (h - i);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quantize"></a>[function <span class="apidocSignatureSpan">d3.</span>quantize (interpolator, n)](#apidoc.element.d3.quantize)
- description and source-code
```javascript
quantize = function (interpolator, n) {
  var samples = new Array(n);
  for (var i = 0; i < n; ++i) samples[i] = interpolator(i / (n - 1));
  return samples;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.queue"></a>[function <span class="apidocSignatureSpan">d3.</span>queue (concurrency)](#apidoc.element.d3.queue)
- description and source-code
```javascript
function queue(concurrency) {
  return new Queue(arguments.length ? +concurrency : Infinity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.queue.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>queue.prototype.constructor (size)](#apidoc.element.d3.queue.prototype.constructor)
- description and source-code
```javascript
function Queue(size) {
  if (!(size >= 1)) throw new Error;
  this._size = size;
  this._call =
  this._error = null;
  this._tasks = [];
  this._data = [];
  this._waiting =
  this._active =
  this._ended =
  this._start = 0; // inside a synchronous task callback?
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.radialArea"></a>[function <span class="apidocSignatureSpan">d3.</span>radialArea ()](#apidoc.element.d3.radialArea)
- description and source-code
```javascript
radialArea = function () {
  var a = area().curve(curveRadialLinear),
      c = a.curve,
      x0 = a.lineX0,
      x1 = a.lineX1,
      y0 = a.lineY0,
      y1 = a.lineY1;

  a.angle = a.x, delete a.x;
  a.startAngle = a.x0, delete a.x0;
  a.endAngle = a.x1, delete a.x1;
  a.radius = a.y, delete a.y;
  a.innerRadius = a.y0, delete a.y0;
  a.outerRadius = a.y1, delete a.y1;
  a.lineStartAngle = function() { return radialLine(x0()); }, delete a.lineX0;
  a.lineEndAngle = function() { return radialLine(x1()); }, delete a.lineX1;
  a.lineInnerRadius = function() { return radialLine(y0()); }, delete a.lineY0;
  a.lineOuterRadius = function() { return radialLine(y1()); }, delete a.lineY1;

  a.curve = function(_) {
    return arguments.length ? c(curveRadial(_)) : c()._curve;
  };

  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.radialLine"></a>[function <span class="apidocSignatureSpan">d3.</span>radialLine ()](#apidoc.element.d3.radialLine)
- description and source-code
```javascript
radialLine = function () {
  return radialLine(line().curve(curveRadialLinear));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.randomBates"></a>[function <span class="apidocSignatureSpan">d3.</span>randomBates (n)](#apidoc.element.d3.randomBates)
- description and source-code
```javascript
randomBates = function (n) {
  var randomIrwinHall = irwinHall(n);
  return function() {
    return randomIrwinHall() / n;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.randomExponential"></a>[function <span class="apidocSignatureSpan">d3.</span>randomExponential (lambda)](#apidoc.element.d3.randomExponential)
- description and source-code
```javascript
randomExponential = function (lambda) {
  return function() {
    return -Math.log(1 - Math.random()) / lambda;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.randomIrwinHall"></a>[function <span class="apidocSignatureSpan">d3.</span>randomIrwinHall (n)](#apidoc.element.d3.randomIrwinHall)
- description and source-code
```javascript
randomIrwinHall = function (n) {
  return function() {
    for (var sum = 0, i = 0; i < n; ++i) sum += Math.random();
    return sum;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.randomLogNormal"></a>[function <span class="apidocSignatureSpan">d3.</span>randomLogNormal ()](#apidoc.element.d3.randomLogNormal)
- description and source-code
```javascript
randomLogNormal = function () {
  var randomNormal = normal.apply(this, arguments);
  return function() {
    return Math.exp(randomNormal());
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.randomNormal"></a>[function <span class="apidocSignatureSpan">d3.</span>randomNormal (mu, sigma)](#apidoc.element.d3.randomNormal)
- description and source-code
```javascript
randomNormal = function (mu, sigma) {
  var x, r;
  mu = mu == null ? 0 : +mu;
  sigma = sigma == null ? 1 : +sigma;
  return function() {
    var y;

    // If available, use the second previously-generated uniform random.
    if (x != null) y = x, x = null;

    // Otherwise, generate a new x and y.
    else do {
      x = Math.random() * 2 - 1;
      y = Math.random() * 2 - 1;
      r = x * x + y * y;
    } while (!r || r > 1);

    return mu + sigma * y * Math.sqrt(-2 * Math.log(r) / r);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.randomUniform"></a>[function <span class="apidocSignatureSpan">d3.</span>randomUniform (min, max)](#apidoc.element.d3.randomUniform)
- description and source-code
```javascript
randomUniform = function (min, max) {
  min = min == null ? 0 : +min;
  max = max == null ? 1 : +max;
  if (arguments.length === 1) max = min, min = 0;
  else max -= min;
  return function() {
    return Math.random() * max + min;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.range"></a>[function <span class="apidocSignatureSpan">d3.</span>range (start, stop, step)](#apidoc.element.d3.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  start = +start, stop = +stop, step = (n = arguments.length) < 2 ? (stop = start, start = 0, 1) : n < 3 ? 1 : +step;

  var i = -1,
      n = Math.max(0, Math.ceil((stop - start) / step)) | 0,
      range = new Array(n);

  while (++i < n) {
    range[i] = start + i * step;
  }

  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.request"></a>[function <span class="apidocSignatureSpan">d3.</span>request (url, callback)](#apidoc.element.d3.request)
- description and source-code
```javascript
request = function (url, callback) {
  var request,
      event = d3Dispatch.dispatch("beforesend", "progress", "load", "error"),
      mimeType,
      headers = d3Collection.map(),
      xhr = new XMLHttpRequest,
      user = null,
      password = null,
      response,
      responseType,
      timeout = 0;

  // If IE does not support CORS, use XDomainRequest.
  if (typeof XDomainRequest !== "undefined"
      && !("withCredentials" in xhr)
      && /^(http(s)?:)?\/\//.test(url)) xhr = new XDomainRequest;

  "onload" in xhr
      ? xhr.onload = xhr.onerror = xhr.ontimeout = respond
      : xhr.onreadystatechange = function(o) { xhr.readyState > 3 && respond(o); };

  function respond(o) {
    var status = xhr.status, result;
    if (!status && hasResponse(xhr)
        || status >= 200 && status < 300
        || status === 304) {
      if (response) {
        try {
          result = response.call(request, xhr);
        } catch (e) {
          event.call("error", request, e);
          return;
        }
      } else {
        result = xhr;
      }
      event.call("load", request, result);
    } else {
      event.call("error", request, o);
    }
  }

  xhr.onprogress = function(e) {
    event.call("progress", request, e);
  };

  request = {
    header: function(name, value) {
      name = (name + "").toLowerCase();
      if (arguments.length < 2) return headers.get(name);
      if (value == null) headers.remove(name);
      else headers.set(name, value + "");
      return request;
    },

    // If mimeType is non-null and no Accept header is set, a default is used.
    mimeType: function(value) {
      if (!arguments.length) return mimeType;
      mimeType = value == null ? null : value + "";
      return request;
    },

    // Specifies what type the response value should take;
    // for instance, arraybuffer, blob, document, or text.
    responseType: function(value) {
      if (!arguments.length) return responseType;
      responseType = value;
      return request;
    },

    timeout: function(value) {
      if (!arguments.length) return timeout;
      timeout = +value;
      return request;
    },

    user: function(value) {
      return arguments.length < 1 ? user : (user = value == null ? null : value + "", request);
    },

    password: function(value) {
      return arguments.length < 1 ? password : (password = value == null ? null : value + "", request);
    },

    // Specify how to convert the response content to a specific type;
    // changes the callback value on "load" events.
    response: function(value) {
      response = value;
      return request;
    },

    // Alias for send("GET", …).
    get: function(data, callback) {
      return request.send("GET", data, callback);
    },

    // Alias for send("POST", …).
    post: function(data, callback) {
      return request.send("POST", data, callback);
    },

    // If callback is non-null, it will be used for error and load events.
    send: function(method, data, callback) {
      xhr.open(method, url, true, user, password);
      if (mimeType != null && !headers.has("accept")) headers.set("accept", mimeType + ",*/*");
      if (xhr.setRequestHeader) headers.each(function(value, name) { xhr.setRequestHeader(name, value); });
      if (mimeType != null && xhr.overrideMimeType) xhr.overrideMimeType(mimeType);
      if (responseType != null) xhr.responseType = responseType;
      if (timeout > 0) xhr.timeout = timeout;
      if (callback == null && typeof data === "function") callback = data, data = null;
      if (callback != null && callback.length === 1) callback = fixCallback(callback);
      if (callback != null) request.on("error", callback).on("load", function(xhr) { callback(null, xhr); });
      event.call("beforesend", request, xhr);
      xhr.send(data == null ? null : data);
      return request;
    },

    abort: function() {
      xhr.abort();
      return request;
    },

    on: function() {
      var value = event.on.apply(event, arguments);
      return value === event ? request : value;
    }
  };

  if (callback != null) {
    if (t ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.rgb"></a>[function <span class="apidocSignatureSpan">d3.</span>rgb (r, g, b, opacity)](#apidoc.element.d3.rgb)
- description and source-code
```javascript
function rgb(r, g, b, opacity) {
  return arguments.length === 1 ? rgbConvert(r) : new Rgb(r, g, b, opacity == null ? 1 : opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.rgb.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>rgb.prototype.constructor (r, g, b, opacity)](#apidoc.element.d3.rgb.prototype.constructor)
- description and source-code
```javascript
function Rgb(r, g, b, opacity) {
  this.r = +r;
  this.g = +g;
  this.b = +b;
  this.opacity = +opacity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.ribbon"></a>[function <span class="apidocSignatureSpan">d3.</span>ribbon ()](#apidoc.element.d3.ribbon)
- description and source-code
```javascript
ribbon = function () {
  var source = defaultSource,
      target = defaultTarget,
      radius = defaultRadius,
      startAngle = defaultStartAngle,
      endAngle = defaultEndAngle,
      context = null;

  function ribbon() {
    var buffer,
        argv = slice.call(arguments),
        s = source.apply(this, argv),
        t = target.apply(this, argv),
        sr = +radius.apply(this, (argv[0] = s, argv)),
        sa0 = startAngle.apply(this, argv) - halfPi,
        sa1 = endAngle.apply(this, argv) - halfPi,
        sx0 = sr * cos(sa0),
        sy0 = sr * sin(sa0),
        tr = +radius.apply(this, (argv[0] = t, argv)),
        ta0 = startAngle.apply(this, argv) - halfPi,
        ta1 = endAngle.apply(this, argv) - halfPi;

    if (!context) context = buffer = d3Path.path();

    context.moveTo(sx0, sy0);
    context.arc(0, 0, sr, sa0, sa1);
    if (sa0 !== ta0 || sa1 !== ta1) { // TODO sr !== tr?
      context.quadraticCurveTo(0, 0, tr * cos(ta0), tr * sin(ta0));
      context.arc(0, 0, tr, ta0, ta1);
    }
    context.quadraticCurveTo(0, 0, sx0, sy0);
    context.closePath();

    if (buffer) return context = null, buffer + "" || null;
  }

  ribbon.radius = function(_) {
    return arguments.length ? (radius = typeof _ === "function" ? _ : constant(+_), ribbon) : radius;
  };

  ribbon.startAngle = function(_) {
    return arguments.length ? (startAngle = typeof _ === "function" ? _ : constant(+_), ribbon) : startAngle;
  };

  ribbon.endAngle = function(_) {
    return arguments.length ? (endAngle = typeof _ === "function" ? _ : constant(+_), ribbon) : endAngle;
  };

  ribbon.source = function(_) {
    return arguments.length ? (source = _, ribbon) : source;
  };

  ribbon.target = function(_) {
    return arguments.length ? (target = _, ribbon) : target;
  };

  ribbon.context = function(_) {
    return arguments.length ? ((context = _ == null ? null : _), ribbon) : context;
  };

  return ribbon;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleBand"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleBand ()](#apidoc.element.d3.scaleBand)
- description and source-code
```javascript
function band() {
  var scale = ordinal().unknown(undefined),
      domain = scale.domain,
      ordinalRange = scale.range,
      range$$1 = [0, 1],
      step,
      bandwidth,
      round = false,
      paddingInner = 0,
      paddingOuter = 0,
      align = 0.5;

  delete scale.unknown;

  function rescale() {
    var n = domain().length,
        reverse = range$$1[1] < range$$1[0],
        start = range$$1[reverse - 0],
        stop = range$$1[1 - reverse];
    step = (stop - start) / Math.max(1, n - paddingInner + paddingOuter * 2);
    if (round) step = Math.floor(step);
    start += (stop - start - step * (n - paddingInner)) * align;
    bandwidth = step * (1 - paddingInner);
    if (round) start = Math.round(start), bandwidth = Math.round(bandwidth);
    var values = d3Array.range(n).map(function(i) { return start + step * i; });
    return ordinalRange(reverse ? values.reverse() : values);
  }

  scale.domain = function(_) {
    return arguments.length ? (domain(_), rescale()) : domain();
  };

  scale.range = function(_) {
    return arguments.length ? (range$$1 = [+_[0], +_[1]], rescale()) : range$$1.slice();
  };

  scale.rangeRound = function(_) {
    return range$$1 = [+_[0], +_[1]], round = true, rescale();
  };

  scale.bandwidth = function() {
    return bandwidth;
  };

  scale.step = function() {
    return step;
  };

  scale.round = function(_) {
    return arguments.length ? (round = !!_, rescale()) : round;
  };

  scale.padding = function(_) {
    return arguments.length ? (paddingInner = paddingOuter = Math.max(0, Math.min(1, _)), rescale()) : paddingInner;
  };

  scale.paddingInner = function(_) {
    return arguments.length ? (paddingInner = Math.max(0, Math.min(1, _)), rescale()) : paddingInner;
  };

  scale.paddingOuter = function(_) {
    return arguments.length ? (paddingOuter = Math.max(0, Math.min(1, _)), rescale()) : paddingOuter;
  };

  scale.align = function(_) {
    return arguments.length ? (align = Math.max(0, Math.min(1, _)), rescale()) : align;
  };

  scale.copy = function() {
    return band()
        .domain(domain())
        .range(range$$1)
        .round(round)
        .paddingInner(paddingInner)
        .paddingOuter(paddingOuter)
        .align(align);
  };

  return rescale();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleIdentity"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleIdentity ()](#apidoc.element.d3.scaleIdentity)
- description and source-code
```javascript
function identity() {
  var domain = [0, 1];

  function scale(x) {
    return +x;
  }

  scale.invert = scale;

  scale.domain = scale.range = function(_) {
    return arguments.length ? (domain = map$1.call(_, number), scale) : domain.slice();
  };

  scale.copy = function() {
    return identity().domain(domain);
  };

  return linearish(scale);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleLinear"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleLinear ()](#apidoc.element.d3.scaleLinear)
- description and source-code
```javascript
function linear() {
  var scale = continuous(deinterpolateLinear, d3Interpolate.interpolateNumber);

  scale.copy = function() {
    return copy(scale, linear());
  };

  return linearish(scale);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleLog"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleLog ()](#apidoc.element.d3.scaleLog)
- description and source-code
```javascript
function log() {
  var scale = continuous(deinterpolate, reinterpolate).domain([1, 10]),
      domain = scale.domain,
      base = 10,
      logs = logp(10),
      pows = powp(10);

  function rescale() {
    logs = logp(base), pows = powp(base);
    if (domain()[0] < 0) logs = reflect(logs), pows = reflect(pows);
    return scale;
  }

  scale.base = function(_) {
    return arguments.length ? (base = +_, rescale()) : base;
  };

  scale.domain = function(_) {
    return arguments.length ? (domain(_), rescale()) : domain();
  };

  scale.ticks = function(count) {
    var d = domain(),
        u = d[0],
        v = d[d.length - 1],
        r;

    if (r = v < u) i = u, u = v, v = i;

    var i = logs(u),
        j = logs(v),
        p,
        k,
        t,
        n = count == null ? 10 : +count,
        z = [];

    if (!(base % 1) && j - i < n) {
      i = Math.round(i) - 1, j = Math.round(j) + 1;
      if (u > 0) for (; i < j; ++i) {
        for (k = 1, p = pows(i); k < base; ++k) {
          t = p * k;
          if (t < u) continue;
          if (t > v) break;
          z.push(t);
        }
      } else for (; i < j; ++i) {
        for (k = base - 1, p = pows(i); k >= 1; --k) {
          t = p * k;
          if (t < u) continue;
          if (t > v) break;
          z.push(t);
        }
      }
    } else {
      z = d3Array.ticks(i, j, Math.min(j - i, n)).map(pows);
    }

    return r ? z.reverse() : z;
  };

  scale.tickFormat = function(count, specifier) {
    if (specifier == null) specifier = base === 10 ? ".0e" : ",";
    if (typeof specifier !== "function") specifier = d3Format.format(specifier);
    if (count === Infinity) return specifier;
    if (count == null) count = 10;
    var k = Math.max(1, base * count / scale.ticks().length); // TODO fast estimate?
    return function(d) {
      var i = d / pows(Math.round(logs(d)));
      if (i * base < base - 0.5) i *= base;
      return i <= k ? specifier(d) : "";
    };
  };

  scale.nice = function() {
    return domain(nice(domain(), {
      floor: function(x) { return pows(Math.floor(logs(x))); },
      ceil: function(x) { return pows(Math.ceil(logs(x))); }
    }));
  };

  scale.copy = function() {
    return copy(scale, log().base(base));
  };

  return scale;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleOrdinal"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleOrdinal (range$$1)](#apidoc.element.d3.scaleOrdinal)
- description and source-code
```javascript
function ordinal(range$$1) {
  var index = d3Collection.map(),
      domain = [],
      unknown = implicit;

  range$$1 = range$$1 == null ? [] : slice.call(range$$1);

  function scale(d) {
    var key = d + "", i = index.get(key);
    if (!i) {
      if (unknown !== implicit) return unknown;
      index.set(key, i = domain.push(d));
    }
    return range$$1[(i - 1) % range$$1.length];
  }

  scale.domain = function(_) {
    if (!arguments.length) return domain.slice();
    domain = [], index = d3Collection.map();
    var i = -1, n = _.length, d, key;
    while (++i < n) if (!index.has(key = (d = _[i]) + "")) index.set(key, domain.push(d));
    return scale;
  };

  scale.range = function(_) {
    return arguments.length ? (range$$1 = slice.call(_), scale) : range$$1.slice();
  };

  scale.unknown = function(_) {
    return arguments.length ? (unknown = _, scale) : unknown;
  };

  scale.copy = function() {
    return ordinal()
        .domain(domain)
        .range(range$$1)
        .unknown(unknown);
  };

  return scale;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scalePoint"></a>[function <span class="apidocSignatureSpan">d3.</span>scalePoint ()](#apidoc.element.d3.scalePoint)
- description and source-code
```javascript
function point() {
  return pointish(band().paddingInner(1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scalePow"></a>[function <span class="apidocSignatureSpan">d3.</span>scalePow ()](#apidoc.element.d3.scalePow)
- description and source-code
```javascript
function pow() {
  var exponent = 1,
      scale = continuous(deinterpolate, reinterpolate),
      domain = scale.domain;

  function deinterpolate(a, b) {
    return (b = raise(b, exponent) - (a = raise(a, exponent)))
        ? function(x) { return (raise(x, exponent) - a) / b; }
        : constant(b);
  }

  function reinterpolate(a, b) {
    b = raise(b, exponent) - (a = raise(a, exponent));
    return function(t) { return raise(a + b * t, 1 / exponent); };
  }

  scale.exponent = function(_) {
    return arguments.length ? (exponent = +_, domain(domain())) : exponent;
  };

  scale.copy = function() {
    return copy(scale, pow().exponent(exponent));
  };

  return linearish(scale);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleQuantile"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleQuantile ()](#apidoc.element.d3.scaleQuantile)
- description and source-code
```javascript
function quantile$1() {
  var domain = [],
      range$$1 = [],
      thresholds = [];

  function rescale() {
    var i = 0, n = Math.max(1, range$$1.length);
    thresholds = new Array(n - 1);
    while (++i < n) thresholds[i - 1] = d3Array.quantile(domain, i / n);
    return scale;
  }

  function scale(x) {
    if (!isNaN(x = +x)) return range$$1[d3Array.bisect(thresholds, x)];
  }

  scale.invertExtent = function(y) {
    var i = range$$1.indexOf(y);
    return i < 0 ? [NaN, NaN] : [
      i > 0 ? thresholds[i - 1] : domain[0],
      i < thresholds.length ? thresholds[i] : domain[domain.length - 1]
    ];
  };

  scale.domain = function(_) {
    if (!arguments.length) return domain.slice();
    domain = [];
    for (var i = 0, n = _.length, d; i < n; ++i) if (d = _[i], d != null && !isNaN(d = +d)) domain.push(d);
    domain.sort(d3Array.ascending);
    return rescale();
  };

  scale.range = function(_) {
    return arguments.length ? (range$$1 = slice.call(_), rescale()) : range$$1.slice();
  };

  scale.quantiles = function() {
    return thresholds.slice();
  };

  scale.copy = function() {
    return quantile$1()
        .domain(domain)
        .range(range$$1);
  };

  return scale;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleQuantize"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleQuantize ()](#apidoc.element.d3.scaleQuantize)
- description and source-code
```javascript
function quantize() {
  var x0 = 0,
      x1 = 1,
      n = 1,
      domain = [0.5],
      range$$1 = [0, 1];

  function scale(x) {
    if (x <= x) return range$$1[d3Array.bisect(domain, x, 0, n)];
  }

  function rescale() {
    var i = -1;
    domain = new Array(n);
    while (++i < n) domain[i] = ((i + 1) * x1 - (i - n) * x0) / (n + 1);
    return scale;
  }

  scale.domain = function(_) {
    return arguments.length ? (x0 = +_[0], x1 = +_[1], rescale()) : [x0, x1];
  };

  scale.range = function(_) {
    return arguments.length ? (n = (range$$1 = slice.call(_)).length - 1, rescale()) : range$$1.slice();
  };

  scale.invertExtent = function(y) {
    var i = range$$1.indexOf(y);
    return i < 0 ? [NaN, NaN]
        : i < 1 ? [x0, domain[0]]
        : i >= n ? [domain[n - 1], x1]
        : [domain[i - 1], domain[i]];
  };

  scale.copy = function() {
    return quantize()
        .domain([x0, x1])
        .range(range$$1);
  };

  return linearish(scale);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleSequential"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleSequential (interpolator)](#apidoc.element.d3.scaleSequential)
- description and source-code
```javascript
function sequential(interpolator) {
  var x0 = 0,
      x1 = 1,
      clamp = false;

  function scale(x) {
    var t = (x - x0) / (x1 - x0);
    return interpolator(clamp ? Math.max(0, Math.min(1, t)) : t);
  }

  scale.domain = function(_) {
    return arguments.length ? (x0 = +_[0], x1 = +_[1], scale) : [x0, x1];
  };

  scale.clamp = function(_) {
    return arguments.length ? (clamp = !!_, scale) : clamp;
  };

  scale.interpolator = function(_) {
    return arguments.length ? (interpolator = _, scale) : interpolator;
  };

  scale.copy = function() {
    return sequential(interpolator).domain([x0, x1]).clamp(clamp);
  };

  return linearish(scale);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleSqrt"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleSqrt ()](#apidoc.element.d3.scaleSqrt)
- description and source-code
```javascript
function sqrt() {
  return pow().exponent(0.5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleThreshold"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleThreshold ()](#apidoc.element.d3.scaleThreshold)
- description and source-code
```javascript
function threshold() {
  var domain = [0.5],
      range$$1 = [0, 1],
      n = 1;

  function scale(x) {
    if (x <= x) return range$$1[d3Array.bisect(domain, x, 0, n)];
  }

  scale.domain = function(_) {
    return arguments.length ? (domain = slice.call(_), n = Math.min(domain.length, range$$1.length - 1), scale) : domain.slice();
  };

  scale.range = function(_) {
    return arguments.length ? (range$$1 = slice.call(_), n = Math.min(domain.length, range$$1.length - 1), scale) : range$$1.slice
();
  };

  scale.invertExtent = function(y) {
    var i = range$$1.indexOf(y);
    return [domain[i - 1], domain[i]];
  };

  scale.copy = function() {
    return threshold()
        .domain(domain)
        .range(range$$1);
  };

  return scale;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleTime"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleTime ()](#apidoc.element.d3.scaleTime)
- description and source-code
```javascript
scaleTime = function () {
  return calendar(d3Time.timeYear, d3Time.timeMonth, d3Time.timeWeek, d3Time.timeDay, d3Time.timeHour, d3Time.timeMinute, d3Time
.timeSecond, d3Time.timeMillisecond, d3TimeFormat.timeFormat).domain([new Date(2000, 0, 1), new Date(2000, 0, 2)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scaleUtc"></a>[function <span class="apidocSignatureSpan">d3.</span>scaleUtc ()](#apidoc.element.d3.scaleUtc)
- description and source-code
```javascript
scaleUtc = function () {
  return calendar(d3Time.utcYear, d3Time.utcMonth, d3Time.utcWeek, d3Time.utcDay, d3Time.utcHour, d3Time.utcMinute, d3Time.utcSecond
, d3Time.utcMillisecond, d3TimeFormat.utcFormat).domain([Date.UTC(2000, 0, 1), Date.UTC(2000, 0, 2)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.scan"></a>[function <span class="apidocSignatureSpan">d3.</span>scan (array, compare)](#apidoc.element.d3.scan)
- description and source-code
```javascript
scan = function (array, compare) {
  if (!(n = array.length)) return;
  var i = 0,
      n,
      j = 0,
      xi,
      xj = array[j];

  if (!compare) compare = ascending;

  while (++i < n) if (compare(xi = array[i], xj) < 0 || compare(xj, xj) !== 0) xj = xi, j = i;

  if (compare(xj, xj) === 0) return j;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.select"></a>[function <span class="apidocSignatureSpan">d3.</span>select (selector)](#apidoc.element.d3.select)
- description and source-code
```javascript
select = function (selector) {
  return typeof selector === "string"
      ? new Selection([[document.querySelector(selector)]], [document.documentElement])
      : new Selection([[selector]], root);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selectAll"></a>[function <span class="apidocSignatureSpan">d3.</span>selectAll (selector)](#apidoc.element.d3.selectAll)
- description and source-code
```javascript
selectAll = function (selector) {
  return typeof selector === "string"
      ? new Selection([document.querySelectorAll(selector)], [document.documentElement])
      : new Selection([selector == null ? [] : selector], root);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection"></a>[function <span class="apidocSignatureSpan">d3.</span>selection ()](#apidoc.element.d3.selection)
- description and source-code
```javascript
function selection() {
  return new Selection([[document.documentElement]], root);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>selection.prototype.constructor (groups, parents)](#apidoc.element.d3.selection.prototype.constructor)
- description and source-code
```javascript
function Selection(groups, parents) {
  this._groups = groups;
  this._parents = parents;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selector"></a>[function <span class="apidocSignatureSpan">d3.</span>selector (selector)](#apidoc.element.d3.selector)
- description and source-code
```javascript
selector = function (selector) {
  return selector == null ? none : function() {
    return this.querySelector(selector);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selectorAll"></a>[function <span class="apidocSignatureSpan">d3.</span>selectorAll (selector)](#apidoc.element.d3.selectorAll)
- description and source-code
```javascript
selectorAll = function (selector) {
  return selector == null ? empty : function() {
    return this.querySelectorAll(selector);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.set"></a>[function <span class="apidocSignatureSpan">d3.</span>set (object, f)](#apidoc.element.d3.set)
- description and source-code
```javascript
function set(object, f) {
  var set = new Set;

  // Copy constructor.
  if (object instanceof Set) object.each(function(value) { set.add(value); });

  // Otherwise, assume it’s an array.
  else if (object) {
    var i = -1, n = object.length;
    if (f == null) while (++i < n) set.add(object[i]);
    else while (++i < n) set.add(f(object[i], i, object));
  }

  return set;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.set.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>set.prototype.constructor ()](#apidoc.element.d3.set.prototype.constructor)
- description and source-code
```javascript
function Set() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.shuffle"></a>[function <span class="apidocSignatureSpan">d3.</span>shuffle (array, i0, i1)](#apidoc.element.d3.shuffle)
- description and source-code
```javascript
shuffle = function (array, i0, i1) {
  var m = (i1 == null ? array.length : i1) - (i0 = i0 == null ? 0 : +i0),
      t,
      i;

  while (m) {
    i = Math.random() * m-- | 0;
    t = array[m + i0];
    array[m + i0] = array[i + i0];
    array[i + i0] = t;
  }

  return array;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stack"></a>[function <span class="apidocSignatureSpan">d3.</span>stack ()](#apidoc.element.d3.stack)
- description and source-code
```javascript
stack = function () {
  var keys = constant([]),
      order = none$1,
      offset = none,
      value = stackValue;

  function stack(data) {
    var kz = keys.apply(this, arguments),
        i,
        m = data.length,
        n = kz.length,
        sz = new Array(n),
        oz;

    for (i = 0; i < n; ++i) {
      for (var ki = kz[i], si = sz[i] = new Array(m), j = 0, sij; j < m; ++j) {
        si[j] = sij = [0, +value(data[j], ki, j, data)];
        sij.data = data[j];
      }
      si.key = ki;
    }

    for (i = 0, oz = order(sz); i < n; ++i) {
      sz[oz[i]].index = i;
    }

    offset(sz, oz);
    return sz;
  }

  stack.keys = function(_) {
    return arguments.length ? (keys = typeof _ === "function" ? _ : constant(slice.call(_)), stack) : keys;
  };

  stack.value = function(_) {
    return arguments.length ? (value = typeof _ === "function" ? _ : constant(+_), stack) : value;
  };

  stack.order = function(_) {
    return arguments.length ? (order = _ == null ? none$1 : typeof _ === "function" ? _ : constant(slice.call(_)), stack) : order
;
  };

  stack.offset = function(_) {
    return arguments.length ? (offset = _ == null ? none : _, stack) : offset;
  };

  return stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stackOffsetExpand"></a>[function <span class="apidocSignatureSpan">d3.</span>stackOffsetExpand (series, order)](#apidoc.element.d3.stackOffsetExpand)
- description and source-code
```javascript
stackOffsetExpand = function (series, order) {
  if (!((n = series.length) > 0)) return;
  for (var i, n, j = 0, m = series[0].length, y; j < m; ++j) {
    for (y = i = 0; i < n; ++i) y += series[i][j][1] || 0;
    if (y) for (i = 0; i < n; ++i) series[i][j][1] /= y;
  }
  none(series, order);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stackOffsetNone"></a>[function <span class="apidocSignatureSpan">d3.</span>stackOffsetNone (series, order)](#apidoc.element.d3.stackOffsetNone)
- description and source-code
```javascript
stackOffsetNone = function (series, order) {
  if (!((n = series.length) > 1)) return;
  for (var i = 1, s0, s1 = series[order[0]], n, m = s1.length; i < n; ++i) {
    s0 = s1, s1 = series[order[i]];
    for (var j = 0; j < m; ++j) {
      s1[j][1] += s1[j][0] = isNaN(s0[j][1]) ? s0[j][0] : s0[j][1];
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stackOffsetSilhouette"></a>[function <span class="apidocSignatureSpan">d3.</span>stackOffsetSilhouette (series, order)](#apidoc.element.d3.stackOffsetSilhouette)
- description and source-code
```javascript
stackOffsetSilhouette = function (series, order) {
  if (!((n = series.length) > 0)) return;
  for (var j = 0, s0 = series[order[0]], n, m = s0.length; j < m; ++j) {
    for (var i = 0, y = 0; i < n; ++i) y += series[i][j][1] || 0;
    s0[j][1] += s0[j][0] = -y / 2;
  }
  none(series, order);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stackOffsetWiggle"></a>[function <span class="apidocSignatureSpan">d3.</span>stackOffsetWiggle (series, order)](#apidoc.element.d3.stackOffsetWiggle)
- description and source-code
```javascript
stackOffsetWiggle = function (series, order) {
  if (!((n = series.length) > 0) || !((m = (s0 = series[order[0]]).length) > 0)) return;
  for (var y = 0, j = 1, s0, m, n; j < m; ++j) {
    for (var i = 0, s1 = 0, s2 = 0; i < n; ++i) {
      var si = series[order[i]],
          sij0 = si[j][1] || 0,
          sij1 = si[j - 1][1] || 0,
          s3 = (sij0 - sij1) / 2;
      for (var k = 0; k < i; ++k) {
        var sk = series[order[k]],
            skj0 = sk[j][1] || 0,
            skj1 = sk[j - 1][1] || 0;
        s3 += skj0 - skj1;
      }
      s1 += sij0, s2 += s3 * sij0;
    }
    s0[j - 1][1] += s0[j - 1][0] = y;
    if (s1) y -= s2 / s1;
  }
  s0[j - 1][1] += s0[j - 1][0] = y;
  none(series, order);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stackOrderAscending"></a>[function <span class="apidocSignatureSpan">d3.</span>stackOrderAscending (series)](#apidoc.element.d3.stackOrderAscending)
- description and source-code
```javascript
stackOrderAscending = function (series) {
  var sums = series.map(sum);
  return none$1(series).sort(function(a, b) { return sums[a] - sums[b]; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stackOrderDescending"></a>[function <span class="apidocSignatureSpan">d3.</span>stackOrderDescending (series)](#apidoc.element.d3.stackOrderDescending)
- description and source-code
```javascript
stackOrderDescending = function (series) {
  return ascending(series).reverse();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stackOrderInsideOut"></a>[function <span class="apidocSignatureSpan">d3.</span>stackOrderInsideOut (series)](#apidoc.element.d3.stackOrderInsideOut)
- description and source-code
```javascript
stackOrderInsideOut = function (series) {
  var n = series.length,
      i,
      j,
      sums = series.map(sum),
      order = none$1(series).sort(function(a, b) { return sums[b] - sums[a]; }),
      top = 0,
      bottom = 0,
      tops = [],
      bottoms = [];

  for (i = 0; i < n; ++i) {
    j = order[i];
    if (top < bottom) {
      top += sums[j];
      tops.push(j);
    } else {
      bottom += sums[j];
      bottoms.push(j);
    }
  }

  return bottoms.reverse().concat(tops);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stackOrderNone"></a>[function <span class="apidocSignatureSpan">d3.</span>stackOrderNone (series)](#apidoc.element.d3.stackOrderNone)
- description and source-code
```javascript
stackOrderNone = function (series) {
  var n = series.length, o = new Array(n);
  while (--n >= 0) o[n] = n;
  return o;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stackOrderReverse"></a>[function <span class="apidocSignatureSpan">d3.</span>stackOrderReverse (series)](#apidoc.element.d3.stackOrderReverse)
- description and source-code
```javascript
stackOrderReverse = function (series) {
  return none$1(series).reverse();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.stratify"></a>[function <span class="apidocSignatureSpan">d3.</span>stratify ()](#apidoc.element.d3.stratify)
- description and source-code
```javascript
stratify = function () {
  var id = defaultId,
      parentId = defaultParentId;

  function stratify(data) {
    var d,
        i,
        n = data.length,
        root,
        parent,
        node,
        nodes = new Array(n),
        nodeId,
        nodeKey,
        nodeByKey = {};

    for (i = 0; i < n; ++i) {
      d = data[i], node = nodes[i] = new Node(d);
      if ((nodeId = id(d, i, data)) != null && (nodeId += "")) {
        nodeKey = keyPrefix + (node.id = nodeId);
        nodeByKey[nodeKey] = nodeKey in nodeByKey ? ambiguous : node;
      }
    }

    for (i = 0; i < n; ++i) {
      node = nodes[i], nodeId = parentId(data[i], i, data);
      if (nodeId == null || !(nodeId += "")) {
        if (root) throw new Error("multiple roots");
        root = node;
      } else {
        parent = nodeByKey[keyPrefix + nodeId];
        if (!parent) throw new Error("missing: " + nodeId);
        if (parent === ambiguous) throw new Error("ambiguous: " + nodeId);
        if (parent.children) parent.children.push(node);
        else parent.children = [node];
        node.parent = parent;
      }
    }

    if (!root) throw new Error("no root");
    root.parent = preroot;
    root.eachBefore(function(node) { node.depth = node.parent.depth + 1; --n; }).eachBefore(computeHeight);
    root.parent = null;
    if (n > 0) throw new Error("cycle");

    return root;
  }

  stratify.id = function(x) {
    return arguments.length ? (id = required(x), stratify) : id;
  };

  stratify.parentId = function(x) {
    return arguments.length ? (parentId = required(x), stratify) : parentId;
  };

  return stratify;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.sum"></a>[function <span class="apidocSignatureSpan">d3.</span>sum (array, f)](#apidoc.element.d3.sum)
- description and source-code
```javascript
sum = function (array, f) {
  var s = 0,
      n = array.length,
      a,
      i = -1;

  if (f == null) {
    while (++i < n) if (a = +array[i]) s += a; // Note: zero and null are equivalent.
  }

  else {
    while (++i < n) if (a = +f(array[i], i, array)) s += a;
  }

  return s;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.symbol"></a>[function <span class="apidocSignatureSpan">d3.</span>symbol ()](#apidoc.element.d3.symbol)
- description and source-code
```javascript
symbol = function () {
  var type = constant(circle),
      size = constant(64),
      context = null;

  function symbol() {
    var buffer;
    if (!context) context = buffer = d3Path.path();
    type.apply(this, arguments).draw(context, +size.apply(this, arguments));
    if (buffer) return context = null, buffer + "" || null;
  }

  symbol.type = function(_) {
    return arguments.length ? (type = typeof _ === "function" ? _ : constant(_), symbol) : type;
  };

  symbol.size = function(_) {
    return arguments.length ? (size = typeof _ === "function" ? _ : constant(+_), symbol) : size;
  };

  symbol.context = function(_) {
    return arguments.length ? (context = _ == null ? null : _, symbol) : context;
  };

  return symbol;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.text"></a>[function <span class="apidocSignatureSpan">d3.</span>text (url, callback)](#apidoc.element.d3.text)
- description and source-code
```javascript
text = function (url, callback) {
  var r = request(url).mimeType(defaultMimeType).response(response);
  if (callback != null) {
    if (typeof callback !== "function") throw new Error("invalid callback: " + callback);
    return r.get(callback);
  }
  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.thresholdFreedmanDiaconis"></a>[function <span class="apidocSignatureSpan">d3.</span>thresholdFreedmanDiaconis (values, min, max)](#apidoc.element.d3.thresholdFreedmanDiaconis)
- description and source-code
```javascript
thresholdFreedmanDiaconis = function (values, min, max) {
  values = map.call(values, number).sort(ascending);
  return Math.ceil((max - min) / (2 * (quantile(values, 0.75) - quantile(values, 0.25)) * Math.pow(values.length, -1 / 3)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.thresholdScott"></a>[function <span class="apidocSignatureSpan">d3.</span>thresholdScott (values, min, max)](#apidoc.element.d3.thresholdScott)
- description and source-code
```javascript
thresholdScott = function (values, min, max) {
  return Math.ceil((max - min) / (3.5 * deviation(values) * Math.pow(values.length, -1 / 3)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.thresholdSturges"></a>[function <span class="apidocSignatureSpan">d3.</span>thresholdSturges (values)](#apidoc.element.d3.thresholdSturges)
- description and source-code
```javascript
thresholdSturges = function (values) {
  return Math.ceil(Math.log(values.length) / Math.LN2) + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.tickStep"></a>[function <span class="apidocSignatureSpan">d3.</span>tickStep (start, stop, count)](#apidoc.element.d3.tickStep)
- description and source-code
```javascript
function tickStep(start, stop, count) {
  var step0 = Math.abs(stop - start) / Math.max(0, count),
      step1 = Math.pow(10, Math.floor(Math.log(step0) / Math.LN10)),
      error = step0 / step1;
  if (error >= e10) step1 *= 10;
  else if (error >= e5) step1 *= 5;
  else if (error >= e2) step1 *= 2;
  return stop < start ? -step1 : step1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.ticks"></a>[function <span class="apidocSignatureSpan">d3.</span>ticks (start, stop, count)](#apidoc.element.d3.ticks)
- description and source-code
```javascript
ticks = function (start, stop, count) {
  var step = tickStep(start, stop, count);
  return range(
    Math.ceil(start / step) * step,
    Math.floor(stop / step) * step + step / 2, // inclusive
    step
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeDay"></a>[function <span class="apidocSignatureSpan">d3.</span>timeDay (date)](#apidoc.element.d3.timeDay)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeDays"></a>[function <span class="apidocSignatureSpan">d3.</span>timeDays (start, stop, step)](#apidoc.element.d3.timeDays)
- description and source-code
```javascript
timeDays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFormat"></a>[function <span class="apidocSignatureSpan">d3.</span>timeFormat (specifier)](#apidoc.element.d3.timeFormat)
- description and source-code
```javascript
timeFormat = function (specifier) {
  var f = newFormat(specifier += "", formats);
  f.toString = function() { return specifier; };
  return f;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFormatDefaultLocale"></a>[function <span class="apidocSignatureSpan">d3.</span>timeFormatDefaultLocale (definition)](#apidoc.element.d3.timeFormatDefaultLocale)
- description and source-code
```javascript
function defaultLocale(definition) {
  locale$1 = formatLocale(definition);
  exports.timeFormat = locale$1.format;
  exports.timeParse = locale$1.parse;
  exports.utcFormat = locale$1.utcFormat;
  exports.utcParse = locale$1.utcParse;
  return locale$1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFormatLocale"></a>[function <span class="apidocSignatureSpan">d3.</span>timeFormatLocale (locale)](#apidoc.element.d3.timeFormatLocale)
- description and source-code
```javascript
function formatLocale(locale) {
  var locale_dateTime = locale.dateTime,
      locale_date = locale.date,
      locale_time = locale.time,
      locale_periods = locale.periods,
      locale_weekdays = locale.days,
      locale_shortWeekdays = locale.shortDays,
      locale_months = locale.months,
      locale_shortMonths = locale.shortMonths;

  var periodRe = formatRe(locale_periods),
      periodLookup = formatLookup(locale_periods),
      weekdayRe = formatRe(locale_weekdays),
      weekdayLookup = formatLookup(locale_weekdays),
      shortWeekdayRe = formatRe(locale_shortWeekdays),
      shortWeekdayLookup = formatLookup(locale_shortWeekdays),
      monthRe = formatRe(locale_months),
      monthLookup = formatLookup(locale_months),
      shortMonthRe = formatRe(locale_shortMonths),
      shortMonthLookup = formatLookup(locale_shortMonths);

  var formats = {
    "a": formatShortWeekday,
    "A": formatWeekday,
    "b": formatShortMonth,
    "B": formatMonth,
    "c": null,
    "d": formatDayOfMonth,
    "e": formatDayOfMonth,
    "H": formatHour24,
    "I": formatHour12,
    "j": formatDayOfYear,
    "L": formatMilliseconds,
    "m": formatMonthNumber,
    "M": formatMinutes,
    "p": formatPeriod,
    "S": formatSeconds,
    "U": formatWeekNumberSunday,
    "w": formatWeekdayNumber,
    "W": formatWeekNumberMonday,
    "x": null,
    "X": null,
    "y": formatYear,
    "Y": formatFullYear,
    "Z": formatZone,
    "%": formatLiteralPercent
  };

  var utcFormats = {
    "a": formatUTCShortWeekday,
    "A": formatUTCWeekday,
    "b": formatUTCShortMonth,
    "B": formatUTCMonth,
    "c": null,
    "d": formatUTCDayOfMonth,
    "e": formatUTCDayOfMonth,
    "H": formatUTCHour24,
    "I": formatUTCHour12,
    "j": formatUTCDayOfYear,
    "L": formatUTCMilliseconds,
    "m": formatUTCMonthNumber,
    "M": formatUTCMinutes,
    "p": formatUTCPeriod,
    "S": formatUTCSeconds,
    "U": formatUTCWeekNumberSunday,
    "w": formatUTCWeekdayNumber,
    "W": formatUTCWeekNumberMonday,
    "x": null,
    "X": null,
    "y": formatUTCYear,
    "Y": formatUTCFullYear,
    "Z": formatUTCZone,
    "%": formatLiteralPercent
  };

  var parses = {
    "a": parseShortWeekday,
    "A": parseWeekday,
    "b": parseShortMonth,
    "B": parseMonth,
    "c": parseLocaleDateTime,
    "d": parseDayOfMonth,
    "e": parseDayOfMonth,
    "H": parseHour24,
    "I": parseHour24,
    "j": parseDayOfYear,
    "L": parseMilliseconds,
    "m": parseMonthNumber,
    "M": parseMinutes,
    "p": parsePeriod,
    "S": parseSeconds,
    "U": parseWeekNumberSunday,
    "w": parseWeekdayNumber,
    "W": parseWeekNumberMonday,
    "x": parseLocaleDate,
    "X": parseLocaleTime,
    "y": parseYear,
    "Y": parseFullYear,
    "Z": parseZone,
    "%": parseLiteralPercent
  };

  // These recursive directive definitions must be deferred.
  formats.x = newFormat(locale_date, formats);
  formats.X = newFormat(locale_time, formats);
  formats.c = newFormat(locale_dateTime, formats);
  utcFormats.x = newFormat(locale_date, utcFormats);
  utcFormats.X = newFormat(locale_time, utcFormats);
  utcFormats.c = newFormat(locale_dateTime, utcFormats);

  function newFormat(specifier, formats) {
    return function(date) {
      var string = [],
          i = -1,
          j = 0,
          n = specifier.length,
          c,
          pad,
          format;

      if (!(date instanceof Date)) date = new Date(+date);

      while (++i < n) {
        if (specifier.charCodeAt(i) === 37) {
          string.push(specifier.slice(j, i));
          if ((pad = pads[c = specifier.charAt(++i)]) != null) c = specifier.charAt(++i);
          else pad = c === "e" ? " " : "0";
          if (format = formats[c]) c = format(date, pad);
          string.push(c);
          j = i + 1;
        }
      }

      string.push(specifier.slice(j, i));
      return string.join("");
    };
  }

  function newParse(specifier, newDate) {
    return function(string) {
      var d = newYear(1900),
          i = parseSpecifier(d, specifier, string += "", 0);
      if (i != string.length) return null; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFriday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeFriday (date)](#apidoc.element.d3.timeFriday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFridays"></a>[function <span class="apidocSignatureSpan">d3.</span>timeFridays (start, stop, step)](#apidoc.element.d3.timeFridays)
- description and source-code
```javascript
timeFridays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeHour"></a>[function <span class="apidocSignatureSpan">d3.</span>timeHour (date)](#apidoc.element.d3.timeHour)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeHours"></a>[function <span class="apidocSignatureSpan">d3.</span>timeHours (start, stop, step)](#apidoc.element.d3.timeHours)
- description and source-code
```javascript
timeHours = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeInterval"></a>[function <span class="apidocSignatureSpan">d3.</span>timeInterval (floori, offseti, count, field)](#apidoc.element.d3.timeInterval)
- description and source-code
```javascript
function newInterval(floori, offseti, count, field) {

  function interval(date) {
    return floori(date = new Date(+date)), date;
  }

  interval.floor = interval;

  interval.ceil = function(date) {
    return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
  };

  interval.round = function(date) {
    var d0 = interval(date),
        d1 = interval.ceil(date);
    return date - d0 < d1 - date ? d0 : d1;
  };

  interval.offset = function(date, step) {
    return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
  };

  interval.range = function(start, stop, step) {
    var range = [];
    start = interval.ceil(start);
    step = step == null ? 1 : Math.floor(step);
    if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
    do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
    return range;
  };

  interval.filter = function(test) {
    return newInterval(function(date) {
      if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
    }, function(date, step) {
      if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
    });
  };

  if (count) {
    interval.count = function(start, end) {
      t0.setTime(+start), t1.setTime(+end);
      floori(t0), floori(t1);
      return Math.floor(count(t0, t1));
    };

    interval.every = function(step) {
      step = Math.floor(step);
      return !isFinite(step) || !(step > 0) ? null
          : !(step > 1) ? interval
          : interval.filter(field
              ? function(d) { return field(d) % step === 0; }
              : function(d) { return interval.count(0, d) % step === 0; });
    };
  }

  return interval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMillisecond"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMillisecond (date)](#apidoc.element.d3.timeMillisecond)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMilliseconds"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMilliseconds (start, stop, step)](#apidoc.element.d3.timeMilliseconds)
- description and source-code
```javascript
timeMilliseconds = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMinute"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMinute (date)](#apidoc.element.d3.timeMinute)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMinutes"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMinutes (start, stop, step)](#apidoc.element.d3.timeMinutes)
- description and source-code
```javascript
timeMinutes = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMonday (date)](#apidoc.element.d3.timeMonday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMondays"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMondays (start, stop, step)](#apidoc.element.d3.timeMondays)
- description and source-code
```javascript
timeMondays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonth"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMonth (date)](#apidoc.element.d3.timeMonth)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonths"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMonths (start, stop, step)](#apidoc.element.d3.timeMonths)
- description and source-code
```javascript
timeMonths = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeParse"></a>[function <span class="apidocSignatureSpan">d3.</span>timeParse (specifier)](#apidoc.element.d3.timeParse)
- description and source-code
```javascript
timeParse = function (specifier) {
  var p = newParse(specifier += "", localDate);
  p.toString = function() { return specifier; };
  return p;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSaturday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeSaturday (date)](#apidoc.element.d3.timeSaturday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSaturdays"></a>[function <span class="apidocSignatureSpan">d3.</span>timeSaturdays (start, stop, step)](#apidoc.element.d3.timeSaturdays)
- description and source-code
```javascript
timeSaturdays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSecond"></a>[function <span class="apidocSignatureSpan">d3.</span>timeSecond (date)](#apidoc.element.d3.timeSecond)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSeconds"></a>[function <span class="apidocSignatureSpan">d3.</span>timeSeconds (start, stop, step)](#apidoc.element.d3.timeSeconds)
- description and source-code
```javascript
timeSeconds = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSunday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeSunday (date)](#apidoc.element.d3.timeSunday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSundays"></a>[function <span class="apidocSignatureSpan">d3.</span>timeSundays (start, stop, step)](#apidoc.element.d3.timeSundays)
- description and source-code
```javascript
timeSundays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeThursday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeThursday (date)](#apidoc.element.d3.timeThursday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeThursdays"></a>[function <span class="apidocSignatureSpan">d3.</span>timeThursdays (start, stop, step)](#apidoc.element.d3.timeThursdays)
- description and source-code
```javascript
timeThursdays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeTuesday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeTuesday (date)](#apidoc.element.d3.timeTuesday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeTuesdays"></a>[function <span class="apidocSignatureSpan">d3.</span>timeTuesdays (start, stop, step)](#apidoc.element.d3.timeTuesdays)
- description and source-code
```javascript
timeTuesdays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWednesday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeWednesday (date)](#apidoc.element.d3.timeWednesday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWednesdays"></a>[function <span class="apidocSignatureSpan">d3.</span>timeWednesdays (start, stop, step)](#apidoc.element.d3.timeWednesdays)
- description and source-code
```javascript
timeWednesdays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWeek"></a>[function <span class="apidocSignatureSpan">d3.</span>timeWeek (date)](#apidoc.element.d3.timeWeek)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWeeks"></a>[function <span class="apidocSignatureSpan">d3.</span>timeWeeks (start, stop, step)](#apidoc.element.d3.timeWeeks)
- description and source-code
```javascript
timeWeeks = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeYear"></a>[function <span class="apidocSignatureSpan">d3.</span>timeYear (date)](#apidoc.element.d3.timeYear)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeYears"></a>[function <span class="apidocSignatureSpan">d3.</span>timeYears (start, stop, step)](#apidoc.element.d3.timeYears)
- description and source-code
```javascript
timeYears = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeout"></a>[function <span class="apidocSignatureSpan">d3.</span>timeout (callback, delay, time)](#apidoc.element.d3.timeout)
- description and source-code
```javascript
timeout = function (callback, delay, time) {
  var t = new Timer;
  delay = delay == null ? 0 : +delay;
  t.restart(function(elapsed) {
    t.stop();
    callback(elapsed + delay);
  }, delay, time);
  return t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timer"></a>[function <span class="apidocSignatureSpan">d3.</span>timer (callback, delay, time)](#apidoc.element.d3.timer)
- description and source-code
```javascript
function timer(callback, delay, time) {
  var t = new Timer;
  t.restart(callback, delay, time);
  return t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timer.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>timer.prototype.constructor ()](#apidoc.element.d3.timer.prototype.constructor)
- description and source-code
```javascript
function Timer() {
  this._call =
  this._time =
  this._next = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timerFlush"></a>[function <span class="apidocSignatureSpan">d3.</span>timerFlush ()](#apidoc.element.d3.timerFlush)
- description and source-code
```javascript
function timerFlush() {
  now(); // Get the current time, if not already set.
  ++frame; // Pretend we’ve set an alarm, if we haven’t already.
  var t = taskHead, e;
  while (t) {
    if ((e = clockNow - t._time) >= 0) t._call.call(null, e);
    t = t._next;
  }
  --frame;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.touch"></a>[function <span class="apidocSignatureSpan">d3.</span>touch (node, touches, identifier)](#apidoc.element.d3.touch)
- description and source-code
```javascript
touch = function (node, touches, identifier) {
  if (arguments.length < 3) identifier = touches, touches = sourceEvent().changedTouches;

  for (var i = 0, n = touches ? touches.length : 0, touch; i < n; ++i) {
    if ((touch = touches[i]).identifier === identifier) {
      return point(node, touch);
    }
  }

  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.touches"></a>[function <span class="apidocSignatureSpan">d3.</span>touches (node, touches)](#apidoc.element.d3.touches)
- description and source-code
```javascript
touches = function (node, touches) {
  if (touches == null) touches = sourceEvent().touches;

  for (var i = 0, n = touches ? touches.length : 0, points = new Array(n); i < n; ++i) {
    points[i] = point(node, touches[i]);
  }

  return points;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition"></a>[function <span class="apidocSignatureSpan">d3.</span>transition (name)](#apidoc.element.d3.transition)
- description and source-code
```javascript
function transition(name) {
  return d3Selection.selection().transition(name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>transition.prototype.constructor (groups, parents, name, id)](#apidoc.element.d3.transition.prototype.constructor)
- description and source-code
```javascript
function Transition(groups, parents, name, id) {
  this._groups = groups;
  this._parents = parents;
  this._name = name;
  this._id = id;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transpose"></a>[function <span class="apidocSignatureSpan">d3.</span>transpose (matrix)](#apidoc.element.d3.transpose)
- description and source-code
```javascript
transpose = function (matrix) {
  if (!(n = matrix.length)) return [];
  for (var i = -1, m = min(matrix, length), transpose = new Array(m); ++i < m;) {
    for (var j = -1, n, row = transpose[i] = new Array(n); ++j < n;) {
      row[j] = matrix[j][i];
    }
  }
  return transpose;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.tree"></a>[function <span class="apidocSignatureSpan">d3.</span>tree ()](#apidoc.element.d3.tree)
- description and source-code
```javascript
tree = function () {
  var separation = defaultSeparation$1,
      dx = 1,
      dy = 1,
      nodeSize = null;

  function tree(root) {
    var t = treeRoot(root);

    // Compute the layout using Buchheim et al.’s algorithm.
    t.eachAfter(firstWalk), t.parent.m = -t.z;
    t.eachBefore(secondWalk);

    // If a fixed node size is specified, scale x and y.
    if (nodeSize) root.eachBefore(sizeNode);

    // If a fixed tree size is specified, scale x and y based on the extent.
    // Compute the left-most, right-most, and depth-most nodes for extents.
    else {
      var left = root,
          right = root,
          bottom = root;
      root.eachBefore(function(node) {
        if (node.x < left.x) left = node;
        if (node.x > right.x) right = node;
        if (node.depth > bottom.depth) bottom = node;
      });
      var s = left === right ? 1 : separation(left, right) / 2,
          tx = s - left.x,
          kx = dx / (right.x + s + tx),
          ky = dy / (bottom.depth || 1);
      root.eachBefore(function(node) {
        node.x = (node.x + tx) * kx;
        node.y = node.depth * ky;
      });
    }

    return root;
  }

  // Computes a preliminary x-coordinate for v. Before that, FIRST WALK is
  // applied recursively to the children of v, as well as the function
  // APPORTION. After spacing out the children by calling EXECUTE SHIFTS, the
  // node v is placed to the midpoint of its outermost children.
  function firstWalk(v) {
    var children = v.children,
        siblings = v.parent.children,
        w = v.i ? siblings[v.i - 1] : null;
    if (children) {
      executeShifts(v);
      var midpoint = (children[0].z + children[children.length - 1].z) / 2;
      if (w) {
        v.z = w.z + separation(v._, w._);
        v.m = v.z - midpoint;
      } else {
        v.z = midpoint;
      }
    } else if (w) {
      v.z = w.z + separation(v._, w._);
    }
    v.parent.A = apportion(v, w, v.parent.A || siblings[0]);
  }

  // Computes all real x-coordinates by summing up the modifiers recursively.
  function secondWalk(v) {
    v._.x = v.z + v.parent.m;
    v.m += v.parent.m;
  }

  // The core of the algorithm. Here, a new subtree is combined with the
  // previous subtrees. Threads are used to traverse the inside and outside
  // contours of the left and right subtree up to the highest common level. The
  // vertices used for the traversals are vi+, vi-, vo-, and vo+, where the
  // superscript o means outside and i means inside, the subscript - means left
  // subtree and + means right subtree. For summing up the modifiers along the
  // contour, we use respective variables si+, si-, so-, and so+. Whenever two
  // nodes of the inside contours conflict, we compute the left one of the
  // greatest uncommon ancestors using the function ANCESTOR and call MOVE
  // SUBTREE to shift the subtree and prepare the shifts of smaller subtrees.
  // Finally, we add a new thread (if necessary).
  function apportion(v, w, ancestor) {
    if (w) {
      var vip = v,
          vop = v,
          vim = w,
          vom = vip.parent.children[0],
          sip = vip.m,
          sop = vop.m,
          sim = vim.m,
          som = vom.m,
          shift;
      while (vim = nextRight(vim), vip = nextLeft(vip), vim && vip) {
        vom = nextLeft(vom);
        vop = nextRight(vop);
        vop.a = v;
        shift = vim.z + sim - vip.z - sip + separation(vim._, vip._);
        if (shift > 0) {
          moveSubtree(nextAncestor(vim, v, ancestor), v, shift);
          sip += shift;
          sop += shift;
        }
        sim += vim.m;
        sip += vip.m;
        som += vom.m;
        sop += vop.m;
      }
      if (vim && !nextRight(vop)) {
        vop.t = vim;
        vop.m += sim - sop;
      }
      if (vip && !nextLeft(vom)) {
        vom.t = vip;
        vom.m += sip - som;
        ancestor = v;
      }
    }
    return ancestor;
  }

  function sizeNode(node) {
    node.x *= dx;
    node.y = node.depth * dy;
  }

  tree.separation = function(x) {
    return arguments.length ? (separation = x, tree) : separation;
  };

  tr ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.treemap"></a>[function <span class="apidocSignatureSpan">d3.</span>treemap ()](#apidoc.element.d3.treemap)
- description and source-code
```javascript
treemap = function () {
  var tile = squarify,
      round = false,
      dx = 1,
      dy = 1,
      paddingStack = [0],
      paddingInner = constantZero,
      paddingTop = constantZero,
      paddingRight = constantZero,
      paddingBottom = constantZero,
      paddingLeft = constantZero;

  function treemap(root) {
    root.x0 =
    root.y0 = 0;
    root.x1 = dx;
    root.y1 = dy;
    root.eachBefore(positionNode);
    paddingStack = [0];
    if (round) root.eachBefore(roundNode);
    return root;
  }

  function positionNode(node) {
    var p = paddingStack[node.depth],
        x0 = node.x0 + p,
        y0 = node.y0 + p,
        x1 = node.x1 - p,
        y1 = node.y1 - p;
    if (x1 < x0) x0 = x1 = (x0 + x1) / 2;
    if (y1 < y0) y0 = y1 = (y0 + y1) / 2;
    node.x0 = x0;
    node.y0 = y0;
    node.x1 = x1;
    node.y1 = y1;
    if (node.children) {
      p = paddingStack[node.depth + 1] = paddingInner(node) / 2;
      x0 += paddingLeft(node) - p;
      y0 += paddingTop(node) - p;
      x1 -= paddingRight(node) - p;
      y1 -= paddingBottom(node) - p;
      if (x1 < x0) x0 = x1 = (x0 + x1) / 2;
      if (y1 < y0) y0 = y1 = (y0 + y1) / 2;
      tile(node, x0, y0, x1, y1);
    }
  }

  treemap.round = function(x) {
    return arguments.length ? (round = !!x, treemap) : round;
  };

  treemap.size = function(x) {
    return arguments.length ? (dx = +x[0], dy = +x[1], treemap) : [dx, dy];
  };

  treemap.tile = function(x) {
    return arguments.length ? (tile = required(x), treemap) : tile;
  };

  treemap.padding = function(x) {
    return arguments.length ? treemap.paddingInner(x).paddingOuter(x) : treemap.paddingInner();
  };

  treemap.paddingInner = function(x) {
    return arguments.length ? (paddingInner = typeof x === "function" ? x : constant(+x), treemap) : paddingInner;
  };

  treemap.paddingOuter = function(x) {
    return arguments.length ? treemap.paddingTop(x).paddingRight(x).paddingBottom(x).paddingLeft(x) : treemap.paddingTop();
  };

  treemap.paddingTop = function(x) {
    return arguments.length ? (paddingTop = typeof x === "function" ? x : constant(+x), treemap) : paddingTop;
  };

  treemap.paddingRight = function(x) {
    return arguments.length ? (paddingRight = typeof x === "function" ? x : constant(+x), treemap) : paddingRight;
  };

  treemap.paddingBottom = function(x) {
    return arguments.length ? (paddingBottom = typeof x === "function" ? x : constant(+x), treemap) : paddingBottom;
  };

  treemap.paddingLeft = function(x) {
    return arguments.length ? (paddingLeft = typeof x === "function" ? x : constant(+x), treemap) : paddingLeft;
  };

  return treemap;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.treemapBinary"></a>[function <span class="apidocSignatureSpan">d3.</span>treemapBinary (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapBinary)
- description and source-code
```javascript
treemapBinary = function (parent, x0, y0, x1, y1) {
  var nodes = parent.children,
      i, n = nodes.length,
      sum, sums = new Array(n + 1);

  for (sums[0] = sum = i = 0; i < n; ++i) {
    sums[i + 1] = sum += nodes[i].value;
  }

  partition(0, n, parent.value, x0, y0, x1, y1);

  function partition(i, j, value, x0, y0, x1, y1) {
    if (i >= j - 1) {
      var node = nodes[i];
      node.x0 = x0, node.y0 = y0;
      node.x1 = x1, node.y1 = y1;
      return;
    }

    var valueOffset = sums[i],
        valueTarget = (value / 2) + valueOffset,
        k = i + 1,
        hi = j - 1;

    while (k < hi) {
      var mid = k + hi >>> 1;
      if (sums[mid] < valueTarget) k = mid + 1;
      else hi = mid;
    }

    if ((valueTarget - sums[k - 1]) < (sums[k] - valueTarget) && i + 1 < k) --k;

    var valueLeft = sums[k] - valueOffset,
        valueRight = value - valueLeft;

    if ((x1 - x0) > (y1 - y0)) {
      var xk = (x0 * valueRight + x1 * valueLeft) / value;
      partition(i, k, valueLeft, x0, y0, xk, y1);
      partition(k, j, valueRight, xk, y0, x1, y1);
    } else {
      var yk = (y0 * valueRight + y1 * valueLeft) / value;
      partition(i, k, valueLeft, x0, y0, x1, yk);
      partition(k, j, valueRight, x0, yk, x1, y1);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.treemapDice"></a>[function <span class="apidocSignatureSpan">d3.</span>treemapDice (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapDice)
- description and source-code
```javascript
treemapDice = function (parent, x0, y0, x1, y1) {
  var nodes = parent.children,
      node,
      i = -1,
      n = nodes.length,
      k = parent.value && (x1 - x0) / parent.value;

  while (++i < n) {
    node = nodes[i], node.y0 = y0, node.y1 = y1;
    node.x0 = x0, node.x1 = x0 += node.value * k;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.treemapResquarify"></a>[function <span class="apidocSignatureSpan">d3.</span>treemapResquarify (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapResquarify)
- description and source-code
```javascript
function resquarify(parent, x0, y0, x1, y1) {
  if ((rows = parent._squarify) && (rows.ratio === ratio)) {
    var rows,
        row,
        nodes,
        i,
        j = -1,
        n,
        m = rows.length,
        value = parent.value;

    while (++j < m) {
      row = rows[j], nodes = row.children;
      for (i = row.value = 0, n = nodes.length; i < n; ++i) row.value += nodes[i].value;
      if (row.dice) treemapDice(row, x0, y0, x1, y0 += (y1 - y0) * row.value / value);
      else treemapSlice(row, x0, y0, x0 += (x1 - x0) * row.value / value, y1);
      value -= row.value;
    }
  } else {
    parent._squarify = rows = squarifyRatio(ratio, parent, x0, y0, x1, y1);
    rows.ratio = ratio;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.treemapSlice"></a>[function <span class="apidocSignatureSpan">d3.</span>treemapSlice (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapSlice)
- description and source-code
```javascript
treemapSlice = function (parent, x0, y0, x1, y1) {
  var nodes = parent.children,
      node,
      i = -1,
      n = nodes.length,
      k = parent.value && (y1 - y0) / parent.value;

  while (++i < n) {
    node = nodes[i], node.x0 = x0, node.x1 = x1;
    node.y0 = y0, node.y1 = y0 += node.value * k;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.treemapSliceDice"></a>[function <span class="apidocSignatureSpan">d3.</span>treemapSliceDice (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapSliceDice)
- description and source-code
```javascript
treemapSliceDice = function (parent, x0, y0, x1, y1) {
  (parent.depth & 1 ? treemapSlice : treemapDice)(parent, x0, y0, x1, y1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.treemapSquarify"></a>[function <span class="apidocSignatureSpan">d3.</span>treemapSquarify (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapSquarify)
- description and source-code
```javascript
function squarify(parent, x0, y0, x1, y1) {
  squarifyRatio(ratio, parent, x0, y0, x1, y1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.tsv"></a>[function <span class="apidocSignatureSpan">d3.</span>tsv (url, row, callback)](#apidoc.element.d3.tsv)
- description and source-code
```javascript
tsv = function (url, row, callback) {
  if (arguments.length < 3) callback = row, row = null;
  var r = request(url).mimeType(defaultMimeType);
  r.row = function(_) { return arguments.length ? r.response(responseOf(parse, row = _)) : row; };
  r.row(row);
  return callback ? r.get(callback) : r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.tsvFormat"></a>[function <span class="apidocSignatureSpan">d3.</span>tsvFormat (rows, columns)](#apidoc.element.d3.tsvFormat)
- description and source-code
```javascript
function format(rows, columns) {
  if (columns == null) columns = inferColumns(rows);
  return [columns.map(formatValue).join(delimiter)].concat(rows.map(function(row) {
    return columns.map(function(column) {
      return formatValue(row[column]);
    }).join(delimiter);
  })).join("\n");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.tsvFormatRows"></a>[function <span class="apidocSignatureSpan">d3.</span>tsvFormatRows (rows)](#apidoc.element.d3.tsvFormatRows)
- description and source-code
```javascript
function formatRows(rows) {
  return rows.map(formatRow).join("\n");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.tsvParse"></a>[function <span class="apidocSignatureSpan">d3.</span>tsvParse (text, f)](#apidoc.element.d3.tsvParse)
- description and source-code
```javascript
function parse(text, f) {
  var convert, columns, rows = parseRows(text, function(row, i) {
    if (convert) return convert(row, i - 1);
    columns = row, convert = f ? customConverter(row, f) : objectConverter(row);
  });
  rows.columns = columns;
  return rows;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.tsvParseRows"></a>[function <span class="apidocSignatureSpan">d3.</span>tsvParseRows (text, f)](#apidoc.element.d3.tsvParseRows)
- description and source-code
```javascript
function parseRows(text, f) {
  var EOL = {}, // sentinel value for end-of-line
      EOF = {}, // sentinel value for end-of-file
      rows = [], // output rows
      N = text.length,
      I = 0, // current character index
      n = 0, // the current line number
      t, // the current token
      eol; // is the current token followed by EOL?

  function token() {
    if (I >= N) return EOF; // special case: end of file
    if (eol) return eol = false, EOL; // special case: end of line

    // special case: quotes
    var j = I, c;
    if (text.charCodeAt(j) === 34) {
      var i = j;
      while (i++ < N) {
        if (text.charCodeAt(i) === 34) {
          if (text.charCodeAt(i + 1) !== 34) break;
          ++i;
        }
      }
      I = i + 2;
      c = text.charCodeAt(i + 1);
      if (c === 13) {
        eol = true;
        if (text.charCodeAt(i + 2) === 10) ++I;
      } else if (c === 10) {
        eol = true;
      }
      return text.slice(j + 1, i).replace(/""/g, "\"");
    }

    // common case: find next delimiter or newline
    while (I < N) {
      var k = 1;
      c = text.charCodeAt(I++);
      if (c === 10) eol = true; // \n
      else if (c === 13) { eol = true; if (text.charCodeAt(I) === 10) ++I, ++k; } // \r|\r\n
      else if (c !== delimiterCode) continue;
      return text.slice(j, I - k);
    }

    // special case: last token before EOF
    return text.slice(j);
  }

  while ((t = token()) !== EOF) {
    var a = [];
    while (t !== EOL && t !== EOF) {
      a.push(t);
      t = token();
    }
    if (f && (a = f(a, n++)) == null) continue;
    rows.push(a);
  }

  return rows;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcDay"></a>[function <span class="apidocSignatureSpan">d3.</span>utcDay (date)](#apidoc.element.d3.utcDay)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcDays"></a>[function <span class="apidocSignatureSpan">d3.</span>utcDays (start, stop, step)](#apidoc.element.d3.utcDays)
- description and source-code
```javascript
utcDays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFormat"></a>[function <span class="apidocSignatureSpan">d3.</span>utcFormat (specifier)](#apidoc.element.d3.utcFormat)
- description and source-code
```javascript
utcFormat = function (specifier) {
  var f = newFormat(specifier += "", utcFormats);
  f.toString = function() { return specifier; };
  return f;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFriday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcFriday (date)](#apidoc.element.d3.utcFriday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFridays"></a>[function <span class="apidocSignatureSpan">d3.</span>utcFridays (start, stop, step)](#apidoc.element.d3.utcFridays)
- description and source-code
```javascript
utcFridays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcHour"></a>[function <span class="apidocSignatureSpan">d3.</span>utcHour (date)](#apidoc.element.d3.utcHour)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcHours"></a>[function <span class="apidocSignatureSpan">d3.</span>utcHours (start, stop, step)](#apidoc.element.d3.utcHours)
- description and source-code
```javascript
utcHours = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMillisecond"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMillisecond (date)](#apidoc.element.d3.utcMillisecond)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMilliseconds"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMilliseconds (start, stop, step)](#apidoc.element.d3.utcMilliseconds)
- description and source-code
```javascript
utcMilliseconds = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMinute"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMinute (date)](#apidoc.element.d3.utcMinute)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMinutes"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMinutes (start, stop, step)](#apidoc.element.d3.utcMinutes)
- description and source-code
```javascript
utcMinutes = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMonday (date)](#apidoc.element.d3.utcMonday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMondays"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMondays (start, stop, step)](#apidoc.element.d3.utcMondays)
- description and source-code
```javascript
utcMondays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonth"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMonth (date)](#apidoc.element.d3.utcMonth)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonths"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMonths (start, stop, step)](#apidoc.element.d3.utcMonths)
- description and source-code
```javascript
utcMonths = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcParse"></a>[function <span class="apidocSignatureSpan">d3.</span>utcParse (specifier)](#apidoc.element.d3.utcParse)
- description and source-code
```javascript
utcParse = function (specifier) {
  var p = newParse(specifier, utcDate);
  p.toString = function() { return specifier; };
  return p;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSaturday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcSaturday (date)](#apidoc.element.d3.utcSaturday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSaturdays"></a>[function <span class="apidocSignatureSpan">d3.</span>utcSaturdays (start, stop, step)](#apidoc.element.d3.utcSaturdays)
- description and source-code
```javascript
utcSaturdays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSecond"></a>[function <span class="apidocSignatureSpan">d3.</span>utcSecond (date)](#apidoc.element.d3.utcSecond)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSeconds"></a>[function <span class="apidocSignatureSpan">d3.</span>utcSeconds (start, stop, step)](#apidoc.element.d3.utcSeconds)
- description and source-code
```javascript
utcSeconds = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSunday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcSunday (date)](#apidoc.element.d3.utcSunday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSundays"></a>[function <span class="apidocSignatureSpan">d3.</span>utcSundays (start, stop, step)](#apidoc.element.d3.utcSundays)
- description and source-code
```javascript
utcSundays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcThursday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcThursday (date)](#apidoc.element.d3.utcThursday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcThursdays"></a>[function <span class="apidocSignatureSpan">d3.</span>utcThursdays (start, stop, step)](#apidoc.element.d3.utcThursdays)
- description and source-code
```javascript
utcThursdays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcTuesday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcTuesday (date)](#apidoc.element.d3.utcTuesday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcTuesdays"></a>[function <span class="apidocSignatureSpan">d3.</span>utcTuesdays (start, stop, step)](#apidoc.element.d3.utcTuesdays)
- description and source-code
```javascript
utcTuesdays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWednesday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcWednesday (date)](#apidoc.element.d3.utcWednesday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWednesdays"></a>[function <span class="apidocSignatureSpan">d3.</span>utcWednesdays (start, stop, step)](#apidoc.element.d3.utcWednesdays)
- description and source-code
```javascript
utcWednesdays = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWeek"></a>[function <span class="apidocSignatureSpan">d3.</span>utcWeek (date)](#apidoc.element.d3.utcWeek)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWeeks"></a>[function <span class="apidocSignatureSpan">d3.</span>utcWeeks (start, stop, step)](#apidoc.element.d3.utcWeeks)
- description and source-code
```javascript
utcWeeks = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcYear"></a>[function <span class="apidocSignatureSpan">d3.</span>utcYear (date)](#apidoc.element.d3.utcYear)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcYears"></a>[function <span class="apidocSignatureSpan">d3.</span>utcYears (start, stop, step)](#apidoc.element.d3.utcYears)
- description and source-code
```javascript
utcYears = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.values"></a>[function <span class="apidocSignatureSpan">d3.</span>values (map)](#apidoc.element.d3.values)
- description and source-code
```javascript
values = function (map) {
  var values = [];
  for (var key in map) values.push(map[key]);
  return values;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.variance"></a>[function <span class="apidocSignatureSpan">d3.</span>variance (array, f)](#apidoc.element.d3.variance)
- description and source-code
```javascript
variance = function (array, f) {
  var n = array.length,
      m = 0,
      a,
      d,
      s = 0,
      i = -1,
      j = 0;

  if (f == null) {
    while (++i < n) {
      if (!isNaN(a = number(array[i]))) {
        d = a - m;
        m += d / ++j;
        s += d * (a - m);
      }
    }
  }

  else {
    while (++i < n) {
      if (!isNaN(a = number(f(array[i], i, array)))) {
        d = a - m;
        m += d / ++j;
        s += d * (a - m);
      }
    }
  }

  if (j > 1) return s / (j - 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.voronoi"></a>[function <span class="apidocSignatureSpan">d3.</span>voronoi ()](#apidoc.element.d3.voronoi)
- description and source-code
```javascript
voronoi = function () {
  var x$$1 = x,
      y$$1 = y,
      extent = null;

  function voronoi(data) {
    return new Diagram(data.map(function(d, i) {
      var s = [Math.round(x$$1(d, i, data) / epsilon) * epsilon, Math.round(y$$1(d, i, data) / epsilon) * epsilon];
      s.index = i;
      s.data = d;
      return s;
    }), extent);
  }

  voronoi.polygons = function(data) {
    return voronoi(data).polygons();
  };

  voronoi.links = function(data) {
    return voronoi(data).links();
  };

  voronoi.triangles = function(data) {
    return voronoi(data).triangles();
  };

  voronoi.x = function(_) {
    return arguments.length ? (x$$1 = typeof _ === "function" ? _ : constant(+_), voronoi) : x$$1;
  };

  voronoi.y = function(_) {
    return arguments.length ? (y$$1 = typeof _ === "function" ? _ : constant(+_), voronoi) : y$$1;
  };

  voronoi.extent = function(_) {
    return arguments.length ? (extent = _ == null ? null : [[+_[0][0], +_[0][1]], [+_[1][0], +_[1][1]]], voronoi) : extent && [[
extent[0][0], extent[0][1]], [extent[1][0], extent[1][1]]];
  };

  voronoi.size = function(_) {
    return arguments.length ? (extent = _ == null ? null : [[0, 0], [+_[0], +_[1]]], voronoi) : extent && [extent[1][0] - extent
[0][0], extent[1][1] - extent[0][1]];
  };

  return voronoi;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.window"></a>[function <span class="apidocSignatureSpan">d3.</span>window (node)](#apidoc.element.d3.window)
- description and source-code
```javascript
window = function (node) {
  return (node.ownerDocument && node.ownerDocument.defaultView) // node is a Node
      || (node.document && node) // node is a Window
      || node.defaultView; // node is a Document
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.xml"></a>[function <span class="apidocSignatureSpan">d3.</span>xml (url, callback)](#apidoc.element.d3.xml)
- description and source-code
```javascript
xml = function (url, callback) {
  var r = request(url).mimeType(defaultMimeType).response(response);
  if (callback != null) {
    if (typeof callback !== "function") throw new Error("invalid callback: " + callback);
    return r.get(callback);
  }
  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zip"></a>[function <span class="apidocSignatureSpan">d3.</span>zip ()](#apidoc.element.d3.zip)
- description and source-code
```javascript
zip = function () {
  return transpose(arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoom"></a>[function <span class="apidocSignatureSpan">d3.</span>zoom ()](#apidoc.element.d3.zoom)
- description and source-code
```javascript
zoom = function () {
  var filter = defaultFilter,
      extent = defaultExtent,
      k0 = 0,
      k1 = Infinity,
      x0 = -k1,
      x1 = k1,
      y0 = x0,
      y1 = x1,
      duration = 250,
      interpolate = d3Interpolate.interpolateZoom,
      gestures = [],
      listeners = d3Dispatch.dispatch("start", "zoom", "end"),
      touchstarting,
      touchending,
      touchDelay = 500,
      wheelDelay = 150;

  function zoom(selection) {
    selection
        .on("wheel.zoom", wheeled)
        .on("mousedown.zoom", mousedowned)
        .on("dblclick.zoom", dblclicked)
        .on("touchstart.zoom", touchstarted)
        .on("touchmove.zoom", touchmoved)
        .on("touchend.zoom touchcancel.zoom", touchended)
        .style("-webkit-tap-highlight-color", "rgba(0,0,0,0)")
        .property("__zoom", defaultTransform);
  }

  zoom.transform = function(collection, transform) {
    var selection = collection.selection ? collection.selection() : collection;
    selection.property("__zoom", defaultTransform);
    if (collection !== selection) {
      schedule(collection, transform);
    } else {
      selection.interrupt().each(function() {
        gesture(this, arguments)
            .start()
            .zoom(null, typeof transform === "function" ? transform.apply(this, arguments) : transform)
            .end();
      });
    }
  };

  zoom.scaleBy = function(selection, k) {
    zoom.scaleTo(selection, function() {
      var k0 = this.__zoom.k,
          k1 = typeof k === "function" ? k.apply(this, arguments) : k;
      return k0 * k1;
    });
  };

  zoom.scaleTo = function(selection, k) {
    zoom.transform(selection, function() {
      var e = extent.apply(this, arguments),
          t0 = this.__zoom,
          p0 = centroid(e),
          p1 = t0.invert(p0),
          k1 = typeof k === "function" ? k.apply(this, arguments) : k;
      return constrain(translate(scale(t0, k1), p0, p1), e);
    });
  };

  zoom.translateBy = function(selection, x, y) {
    zoom.transform(selection, function() {
      return constrain(this.__zoom.translate(
        typeof x === "function" ? x.apply(this, arguments) : x,
        typeof y === "function" ? y.apply(this, arguments) : y
      ), extent.apply(this, arguments));
    });
  };

  function scale(transform, k) {
    k = Math.max(k0, Math.min(k1, k));
    return k === transform.k ? transform : new Transform(k, transform.x, transform.y);
  }

  function translate(transform, p0, p1) {
    var x = p0[0] - p1[0] * transform.k, y = p0[1] - p1[1] * transform.k;
    return x === transform.x && y === transform.y ? transform : new Transform(transform.k, x, y);
  }

  function constrain(transform, extent) {
    var dx0 = transform.invertX(extent[0][0]) - x0,
        dx1 = transform.invertX(extent[1][0]) - x1,
        dy0 = transform.invertY(extent[0][1]) - y0,
        dy1 = transform.invertY(extent[1][1]) - y1;
    return transform.translate(
      dx1 > dx0 ? (dx0 + dx1) / 2 : Math.min(0, dx0) || Math.max(0, dx1),
      dy1 > dy0 ? (dy0 + dy1) / 2 : Math.min(0, dy0) || Math.max(0, dy1)
    );
  }

  function centroid(extent) {
    return [(+extent[0][0] + +extent[1][0]) / 2, (+extent[0][1] + +extent[1][1]) / 2];
  }

  function schedule(transition, transform, center) {
    transition
        .on("start.zoom", function() { gesture(this, arguments).start(); })
        .on("interrupt.zoom end.zoom", function() { gesture(this, arguments).end(); })
        .tween("zoom", function() {
          var that = this,
              args = arguments,
              g = gesture(that, args),
              e = extent.apply(that, args),
              p = center || centroid(e),
              w = Math.max(e[1][0] - e[0][0], e[1][1] - e[0][1]),
              a = that.__zoom,
              b = typeof transform === "function" ? transform.apply(that, args) : transform,
              i = interpolate(a.invert(p).concat(w / a.k), b.invert(p).concat(w / b.k));
          return function(t) {
            if (t === 1) t = b; // Avoid rounding error on end.
            else { var l = i(t), k = w / l[2]; t = new Transform(k, ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform"></a>[function <span class="apidocSignatureSpan">d3.</span>zoomTransform (node)](#apidoc.element.d3.zoomTransform)
- description and source-code
```javascript
function transform(node) {
  return node.__zoom || identity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.</span>zoomTransform.prototype.constructor (k, x, y)](#apidoc.element.d3.zoomTransform.prototype.constructor)
- description and source-code
```javascript
function Transform(k, x, y) {
  this.k = k;
  this.x = x;
  this.y = y;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.color"></a>[module d3.color](#apidoc.module.d3.color)

#### <a name="apidoc.element.d3.color.color"></a>[function <span class="apidocSignatureSpan">d3.</span>color (format)](#apidoc.element.d3.color.color)
- description and source-code
```javascript
function color(format) {
  var m;
  format = (format + "").trim().toLowerCase();
  return (m = reHex3.exec(format)) ? (m = parseInt(m[1], 16), new Rgb((m >> 8 & 0xf) | (m >> 4 & 0x0f0), (m >> 4 & 0xf) | (m & 0xf0
), ((m & 0xf) << 4) | (m & 0xf), 1)) // #f00
      : (m = reHex6.exec(format)) ? rgbn(parseInt(m[1], 16)) // #ff0000
      : (m = reRgbInteger.exec(format)) ? new Rgb(m[1], m[2], m[3], 1) // rgb(255, 0, 0)
      : (m = reRgbPercent.exec(format)) ? new Rgb(m[1] * 255 / 100, m[2] * 255 / 100, m[3] * 255 / 100, 1) // rgb(100%, 0%, 0%)
      : (m = reRgbaInteger.exec(format)) ? rgba(m[1], m[2], m[3], m[4]) // rgba(255, 0, 0, 1)
      : (m = reRgbaPercent.exec(format)) ? rgba(m[1] * 255 / 100, m[2] * 255 / 100, m[3] * 255 / 100, m[4]) // rgb(100%, 0%, 0%,
1)
      : (m = reHslPercent.exec(format)) ? hsla(m[1], m[2] / 100, m[3] / 100, 1) // hsl(120, 50%, 50%)
      : (m = reHslaPercent.exec(format)) ? hsla(m[1], m[2] / 100, m[3] / 100, m[4]) // hsla(120, 50%, 50%, 1)
      : named.hasOwnProperty(format) ? rgbn(named[format])
      : format === "transparent" ? new Rgb(NaN, NaN, NaN, 0)
      : null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.color.prototype"></a>[module d3.color.prototype](#apidoc.module.d3.color.prototype)

#### <a name="apidoc.element.d3.color.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.color.prototype.</span>constructor ()](#apidoc.element.d3.color.prototype.constructor)
- description and source-code
```javascript
function Color() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.color.prototype.displayable"></a>[function <span class="apidocSignatureSpan">d3.color.prototype.</span>displayable ()](#apidoc.element.d3.color.prototype.displayable)
- description and source-code
```javascript
displayable = function () {
  return this.rgb().displayable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.color.prototype.toString"></a>[function <span class="apidocSignatureSpan">d3.color.prototype.</span>toString ()](#apidoc.element.d3.color.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.rgb() + "";
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.color.prototype.constructor"></a>[module d3.color.prototype.constructor](#apidoc.module.d3.color.prototype.constructor)

#### <a name="apidoc.element.d3.color.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.color.prototype.</span>constructor ()](#apidoc.element.d3.color.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.cubehelix"></a>[module d3.cubehelix](#apidoc.module.d3.cubehelix)

#### <a name="apidoc.element.d3.cubehelix.cubehelix"></a>[function <span class="apidocSignatureSpan">d3.</span>cubehelix (h, s, l, opacity)](#apidoc.element.d3.cubehelix.cubehelix)
- description and source-code
```javascript
function cubehelix(h, s, l, opacity) {
  return arguments.length === 1 ? cubehelixConvert(h) : new Cubehelix(h, s, l, opacity == null ? 1 : opacity);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.cubehelix.prototype"></a>[module d3.cubehelix.prototype](#apidoc.module.d3.cubehelix.prototype)

#### <a name="apidoc.element.d3.cubehelix.prototype.brighter"></a>[function <span class="apidocSignatureSpan">d3.cubehelix.prototype.</span>brighter (k)](#apidoc.element.d3.cubehelix.prototype.brighter)
- description and source-code
```javascript
brighter = function (k) {
  k = k == null ? brighter : Math.pow(brighter, k);
  return new Cubehelix(this.h, this.s, this.l * k, this.opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.cubehelix.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.cubehelix.prototype.</span>constructor (h, s, l, opacity)](#apidoc.element.d3.cubehelix.prototype.constructor)
- description and source-code
```javascript
function Cubehelix(h, s, l, opacity) {
  this.h = +h;
  this.s = +s;
  this.l = +l;
  this.opacity = +opacity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.cubehelix.prototype.darker"></a>[function <span class="apidocSignatureSpan">d3.cubehelix.prototype.</span>darker (k)](#apidoc.element.d3.cubehelix.prototype.darker)
- description and source-code
```javascript
darker = function (k) {
  k = k == null ? darker : Math.pow(darker, k);
  return new Cubehelix(this.h, this.s, this.l * k, this.opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.cubehelix.prototype.rgb"></a>[function <span class="apidocSignatureSpan">d3.cubehelix.prototype.</span>rgb ()](#apidoc.element.d3.cubehelix.prototype.rgb)
- description and source-code
```javascript
rgb = function () {
  var h = isNaN(this.h) ? 0 : (this.h + 120) * deg2rad,
      l = +this.l,
      a = isNaN(this.s) ? 0 : this.s * l * (1 - l),
      cosh = Math.cos(h),
      sinh = Math.sin(h);
  return new Rgb(
    255 * (l + a * (A * cosh + B * sinh)),
    255 * (l + a * (C * cosh + D * sinh)),
    255 * (l + a * (E * cosh)),
    this.opacity
  );
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.cubehelix.prototype.constructor"></a>[module d3.cubehelix.prototype.constructor](#apidoc.module.d3.cubehelix.prototype.constructor)

#### <a name="apidoc.element.d3.cubehelix.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.cubehelix.prototype.</span>constructor ()](#apidoc.element.d3.cubehelix.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.curveBundle"></a>[module d3.curveBundle](#apidoc.module.d3.curveBundle)

#### <a name="apidoc.element.d3.curveBundle.curveBundle"></a>[function <span class="apidocSignatureSpan">d3.</span>curveBundle (context)](#apidoc.element.d3.curveBundle.curveBundle)
- description and source-code
```javascript
function bundle(context) {
  return beta === 1 ? new Basis(context) : new Bundle(context, beta);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveBundle.beta"></a>[function <span class="apidocSignatureSpan">d3.curveBundle.</span>beta (beta)](#apidoc.element.d3.curveBundle.beta)
- description and source-code
```javascript
beta = function (beta) {
  return custom(+beta);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.curveCardinal"></a>[module d3.curveCardinal](#apidoc.module.d3.curveCardinal)

#### <a name="apidoc.element.d3.curveCardinal.curveCardinal"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCardinal (context)](#apidoc.element.d3.curveCardinal.curveCardinal)
- description and source-code
```javascript
function cardinal(context) {
  return new Cardinal(context, tension);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCardinal.tension"></a>[function <span class="apidocSignatureSpan">d3.curveCardinal.</span>tension (tension)](#apidoc.element.d3.curveCardinal.tension)
- description and source-code
```javascript
tension = function (tension) {
  return custom(+tension);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.curveCardinalClosed"></a>[module d3.curveCardinalClosed](#apidoc.module.d3.curveCardinalClosed)

#### <a name="apidoc.element.d3.curveCardinalClosed.curveCardinalClosed"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCardinalClosed (context)](#apidoc.element.d3.curveCardinalClosed.curveCardinalClosed)
- description and source-code
```javascript
function cardinal(context) {
  return new CardinalClosed(context, tension);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCardinalClosed.tension"></a>[function <span class="apidocSignatureSpan">d3.curveCardinalClosed.</span>tension (tension)](#apidoc.element.d3.curveCardinalClosed.tension)
- description and source-code
```javascript
tension = function (tension) {
  return custom(+tension);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.curveCardinalOpen"></a>[module d3.curveCardinalOpen](#apidoc.module.d3.curveCardinalOpen)

#### <a name="apidoc.element.d3.curveCardinalOpen.curveCardinalOpen"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCardinalOpen (context)](#apidoc.element.d3.curveCardinalOpen.curveCardinalOpen)
- description and source-code
```javascript
function cardinal(context) {
  return new CardinalOpen(context, tension);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCardinalOpen.tension"></a>[function <span class="apidocSignatureSpan">d3.curveCardinalOpen.</span>tension (tension)](#apidoc.element.d3.curveCardinalOpen.tension)
- description and source-code
```javascript
tension = function (tension) {
  return custom(+tension);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.curveCatmullRom"></a>[module d3.curveCatmullRom](#apidoc.module.d3.curveCatmullRom)

#### <a name="apidoc.element.d3.curveCatmullRom.curveCatmullRom"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCatmullRom (context)](#apidoc.element.d3.curveCatmullRom.curveCatmullRom)
- description and source-code
```javascript
function catmullRom(context) {
  return alpha ? new CatmullRom(context, alpha) : new Cardinal(context, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCatmullRom.alpha"></a>[function <span class="apidocSignatureSpan">d3.curveCatmullRom.</span>alpha (alpha)](#apidoc.element.d3.curveCatmullRom.alpha)
- description and source-code
```javascript
alpha = function (alpha) {
  return custom(+alpha);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.curveCatmullRomClosed"></a>[module d3.curveCatmullRomClosed](#apidoc.module.d3.curveCatmullRomClosed)

#### <a name="apidoc.element.d3.curveCatmullRomClosed.curveCatmullRomClosed"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCatmullRomClosed (context)](#apidoc.element.d3.curveCatmullRomClosed.curveCatmullRomClosed)
- description and source-code
```javascript
function catmullRom(context) {
  return alpha ? new CatmullRomClosed(context, alpha) : new CardinalClosed(context, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCatmullRomClosed.alpha"></a>[function <span class="apidocSignatureSpan">d3.curveCatmullRomClosed.</span>alpha (alpha)](#apidoc.element.d3.curveCatmullRomClosed.alpha)
- description and source-code
```javascript
alpha = function (alpha) {
  return custom(+alpha);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.curveCatmullRomOpen"></a>[module d3.curveCatmullRomOpen](#apidoc.module.d3.curveCatmullRomOpen)

#### <a name="apidoc.element.d3.curveCatmullRomOpen.curveCatmullRomOpen"></a>[function <span class="apidocSignatureSpan">d3.</span>curveCatmullRomOpen (context)](#apidoc.element.d3.curveCatmullRomOpen.curveCatmullRomOpen)
- description and source-code
```javascript
function catmullRom(context) {
  return alpha ? new CatmullRomOpen(context, alpha) : new CardinalOpen(context, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.curveCatmullRomOpen.alpha"></a>[function <span class="apidocSignatureSpan">d3.curveCatmullRomOpen.</span>alpha (alpha)](#apidoc.element.d3.curveCatmullRomOpen.alpha)
- description and source-code
```javascript
alpha = function (alpha) {
  return custom(+alpha);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.dispatch"></a>[module d3.dispatch](#apidoc.module.d3.dispatch)

#### <a name="apidoc.element.d3.dispatch.dispatch"></a>[function <span class="apidocSignatureSpan">d3.</span>dispatch ()](#apidoc.element.d3.dispatch.dispatch)
- description and source-code
```javascript
function dispatch() {
  for (var i = 0, n = arguments.length, _ = {}, t; i < n; ++i) {
    if (!(t = arguments[i] + "") || (t in _)) throw new Error("illegal type: " + t);
    _[t] = [];
  }
  return new Dispatch(_);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.dispatch.prototype"></a>[module d3.dispatch.prototype](#apidoc.module.d3.dispatch.prototype)

#### <a name="apidoc.element.d3.dispatch.prototype.apply"></a>[function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>apply (type, that, args)](#apidoc.element.d3.dispatch.prototype.apply)
- description and source-code
```javascript
apply = function (type, that, args) {
  if (!this._.hasOwnProperty(type)) throw new Error("unknown type: " + type);
  for (var t = this._[type], i = 0, n = t.length; i < n; ++i) t[i].value.apply(that, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.dispatch.prototype.call"></a>[function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>call (type, that)](#apidoc.element.d3.dispatch.prototype.call)
- description and source-code
```javascript
call = function (type, that) {
  if ((n = arguments.length - 2) > 0) for (var args = new Array(n), i = 0, n, t; i < n; ++i) args[i] = arguments[i + 2];
  if (!this._.hasOwnProperty(type)) throw new Error("unknown type: " + type);
  for (t = this._[type], i = 0, n = t.length; i < n; ++i) t[i].value.apply(that, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.dispatch.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>constructor (_)](#apidoc.element.d3.dispatch.prototype.constructor)
- description and source-code
```javascript
function Dispatch(_) {
  this._ = _;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.dispatch.prototype.copy"></a>[function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>copy ()](#apidoc.element.d3.dispatch.prototype.copy)
- description and source-code
```javascript
copy = function () {
  var copy = {}, _ = this._;
  for (var t in _) copy[t] = _[t].slice();
  return new Dispatch(copy);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.dispatch.prototype.on"></a>[function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>on (typename, callback)](#apidoc.element.d3.dispatch.prototype.on)
- description and source-code
```javascript
on = function (typename, callback) {
  var _ = this._,
      T = parseTypenames(typename + "", _),
      t,
      i = -1,
      n = T.length;

  // If no callback was specified, return the callback of the given type and name.
  if (arguments.length < 2) {
    while (++i < n) if ((t = (typename = T[i]).type) && (t = get(_[t], typename.name))) return t;
    return;
  }

  // If a type was specified, set the callback for the given type and name.
  // Otherwise, if a null callback was specified, remove callbacks of the given name.
  if (callback != null && typeof callback !== "function") throw new Error("invalid callback: " + callback);
  while (++i < n) {
    if (t = (typename = T[i]).type) _[t] = set(_[t], typename.name, callback);
    else if (callback == null) for (t in _) _[t] = set(_[t], typename.name, null);
  }

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.dispatch.prototype.constructor"></a>[module d3.dispatch.prototype.constructor](#apidoc.module.d3.dispatch.prototype.constructor)

#### <a name="apidoc.element.d3.dispatch.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.dispatch.prototype.</span>constructor ()](#apidoc.element.d3.dispatch.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.easeBack"></a>[module d3.easeBack](#apidoc.module.d3.easeBack)

#### <a name="apidoc.element.d3.easeBack.easeBack"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBack (t)](#apidoc.element.d3.easeBack.easeBack)
- description and source-code
```javascript
function backInOut(t) {
  return ((t *= 2) < 1 ? t * t * ((s + 1) * t - s) : (t -= 2) * t * ((s + 1) * t + s) + 2) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBack.overshoot"></a>[function <span class="apidocSignatureSpan">d3.easeBack.</span>overshoot (s)](#apidoc.element.d3.easeBack.overshoot)
- description and source-code
```javascript
function custom(s) {
  s = +s;

  function backInOut(t) {
    return ((t *= 2) < 1 ? t * t * ((s + 1) * t - s) : (t -= 2) * t * ((s + 1) * t + s) + 2) / 2;
  }

  backInOut.overshoot = custom;

  return backInOut;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.easeBackIn"></a>[module d3.easeBackIn](#apidoc.module.d3.easeBackIn)

#### <a name="apidoc.element.d3.easeBackIn.easeBackIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBackIn (t)](#apidoc.element.d3.easeBackIn.easeBackIn)
- description and source-code
```javascript
function backIn(t) {
  return t * t * ((s + 1) * t - s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBackIn.overshoot"></a>[function <span class="apidocSignatureSpan">d3.easeBackIn.</span>overshoot (s)](#apidoc.element.d3.easeBackIn.overshoot)
- description and source-code
```javascript
function custom(s) {
  s = +s;

  function backIn(t) {
    return t * t * ((s + 1) * t - s);
  }

  backIn.overshoot = custom;

  return backIn;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.easeBackOut"></a>[module d3.easeBackOut](#apidoc.module.d3.easeBackOut)

#### <a name="apidoc.element.d3.easeBackOut.easeBackOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeBackOut (t)](#apidoc.element.d3.easeBackOut.easeBackOut)
- description and source-code
```javascript
function backOut(t) {
  return --t * t * ((s + 1) * t + s) + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeBackOut.overshoot"></a>[function <span class="apidocSignatureSpan">d3.easeBackOut.</span>overshoot (s)](#apidoc.element.d3.easeBackOut.overshoot)
- description and source-code
```javascript
function custom(s) {
  s = +s;

  function backOut(t) {
    return --t * t * ((s + 1) * t + s) + 1;
  }

  backOut.overshoot = custom;

  return backOut;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.easeElastic"></a>[module d3.easeElastic](#apidoc.module.d3.easeElastic)

#### <a name="apidoc.element.d3.easeElastic.easeElastic"></a>[function <span class="apidocSignatureSpan">d3.</span>easeElastic (t)](#apidoc.element.d3.easeElastic.easeElastic)
- description and source-code
```javascript
function elasticOut(t) {
  return 1 - a * Math.pow(2, -10 * (t = +t)) * Math.sin((t + s) / p);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeElastic.amplitude"></a>[function <span class="apidocSignatureSpan">d3.easeElastic.</span>amplitude (a)](#apidoc.element.d3.easeElastic.amplitude)
- description and source-code
```javascript
amplitude = function (a) { return custom(a, p * tau); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeElastic.period"></a>[function <span class="apidocSignatureSpan">d3.easeElastic.</span>period (p)](#apidoc.element.d3.easeElastic.period)
- description and source-code
```javascript
period = function (p) { return custom(a, p); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.easeElasticIn"></a>[module d3.easeElasticIn](#apidoc.module.d3.easeElasticIn)

#### <a name="apidoc.element.d3.easeElasticIn.easeElasticIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easeElasticIn (t)](#apidoc.element.d3.easeElasticIn.easeElasticIn)
- description and source-code
```javascript
function elasticIn(t) {
  return a * Math.pow(2, 10 * --t) * Math.sin((s - t) / p);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeElasticIn.amplitude"></a>[function <span class="apidocSignatureSpan">d3.easeElasticIn.</span>amplitude (a)](#apidoc.element.d3.easeElasticIn.amplitude)
- description and source-code
```javascript
amplitude = function (a) { return custom(a, p * tau); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeElasticIn.period"></a>[function <span class="apidocSignatureSpan">d3.easeElasticIn.</span>period (p)](#apidoc.element.d3.easeElasticIn.period)
- description and source-code
```javascript
period = function (p) { return custom(a, p); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.easeElasticInOut"></a>[module d3.easeElasticInOut](#apidoc.module.d3.easeElasticInOut)

#### <a name="apidoc.element.d3.easeElasticInOut.easeElasticInOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easeElasticInOut (t)](#apidoc.element.d3.easeElasticInOut.easeElasticInOut)
- description and source-code
```javascript
function elasticInOut(t) {
  return ((t = t * 2 - 1) < 0
      ? a * Math.pow(2, 10 * t) * Math.sin((s - t) / p)
      : 2 - a * Math.pow(2, -10 * t) * Math.sin((s + t) / p)) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeElasticInOut.amplitude"></a>[function <span class="apidocSignatureSpan">d3.easeElasticInOut.</span>amplitude (a)](#apidoc.element.d3.easeElasticInOut.amplitude)
- description and source-code
```javascript
amplitude = function (a) { return custom(a, p * tau); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easeElasticInOut.period"></a>[function <span class="apidocSignatureSpan">d3.easeElasticInOut.</span>period (p)](#apidoc.element.d3.easeElasticInOut.period)
- description and source-code
```javascript
period = function (p) { return custom(a, p); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.easePoly"></a>[module d3.easePoly](#apidoc.module.d3.easePoly)

#### <a name="apidoc.element.d3.easePoly.easePoly"></a>[function <span class="apidocSignatureSpan">d3.</span>easePoly (t)](#apidoc.element.d3.easePoly.easePoly)
- description and source-code
```javascript
function polyInOut(t) {
  return ((t *= 2) <= 1 ? Math.pow(t, e) : 2 - Math.pow(2 - t, e)) / 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easePoly.exponent"></a>[function <span class="apidocSignatureSpan">d3.easePoly.</span>exponent (e)](#apidoc.element.d3.easePoly.exponent)
- description and source-code
```javascript
function custom(e) {
  e = +e;

  function polyInOut(t) {
    return ((t *= 2) <= 1 ? Math.pow(t, e) : 2 - Math.pow(2 - t, e)) / 2;
  }

  polyInOut.exponent = custom;

  return polyInOut;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.easePolyIn"></a>[module d3.easePolyIn](#apidoc.module.d3.easePolyIn)

#### <a name="apidoc.element.d3.easePolyIn.easePolyIn"></a>[function <span class="apidocSignatureSpan">d3.</span>easePolyIn (t)](#apidoc.element.d3.easePolyIn.easePolyIn)
- description and source-code
```javascript
function polyIn(t) {
  return Math.pow(t, e);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easePolyIn.exponent"></a>[function <span class="apidocSignatureSpan">d3.easePolyIn.</span>exponent (e)](#apidoc.element.d3.easePolyIn.exponent)
- description and source-code
```javascript
function custom(e) {
  e = +e;

  function polyIn(t) {
    return Math.pow(t, e);
  }

  polyIn.exponent = custom;

  return polyIn;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.easePolyOut"></a>[module d3.easePolyOut](#apidoc.module.d3.easePolyOut)

#### <a name="apidoc.element.d3.easePolyOut.easePolyOut"></a>[function <span class="apidocSignatureSpan">d3.</span>easePolyOut (t)](#apidoc.element.d3.easePolyOut.easePolyOut)
- description and source-code
```javascript
function polyOut(t) {
  return 1 - Math.pow(1 - t, e);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.easePolyOut.exponent"></a>[function <span class="apidocSignatureSpan">d3.easePolyOut.</span>exponent (e)](#apidoc.element.d3.easePolyOut.exponent)
- description and source-code
```javascript
function custom(e) {
  e = +e;

  function polyOut(t) {
    return 1 - Math.pow(1 - t, e);
  }

  polyOut.exponent = custom;

  return polyOut;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.formatSpecifier"></a>[module d3.formatSpecifier](#apidoc.module.d3.formatSpecifier)

#### <a name="apidoc.element.d3.formatSpecifier.formatSpecifier"></a>[function <span class="apidocSignatureSpan">d3.</span>formatSpecifier (specifier)](#apidoc.element.d3.formatSpecifier.formatSpecifier)
- description and source-code
```javascript
function formatSpecifier(specifier) {
  return new FormatSpecifier(specifier);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.formatSpecifier.prototype"></a>[module d3.formatSpecifier.prototype](#apidoc.module.d3.formatSpecifier.prototype)

#### <a name="apidoc.element.d3.formatSpecifier.prototype.toString"></a>[function <span class="apidocSignatureSpan">d3.formatSpecifier.prototype.</span>toString ()](#apidoc.element.d3.formatSpecifier.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.fill
      + this.align
      + this.sign
      + this.symbol
      + (this.zero ? "0" : "")
      + (this.width == null ? "" : Math.max(1, this.width | 0))
      + (this.comma ? "," : "")
      + (this.precision == null ? "" : "." + Math.max(0, this.precision | 0))
      + this.type;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.geoAzimuthalEqualAreaRaw"></a>[module d3.geoAzimuthalEqualAreaRaw](#apidoc.module.d3.geoAzimuthalEqualAreaRaw)

#### <a name="apidoc.element.d3.geoAzimuthalEqualAreaRaw.geoAzimuthalEqualAreaRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEqualAreaRaw (x, y)](#apidoc.element.d3.geoAzimuthalEqualAreaRaw.geoAzimuthalEqualAreaRaw)
- description and source-code
```javascript
geoAzimuthalEqualAreaRaw = function (x, y) {
  var cx = cos(x),
      cy = cos(y),
      k = scale(cx * cy);
  return [
    k * cy * sin(x),
    k * sin(y)
  ];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoAzimuthalEqualAreaRaw.invert"></a>[function <span class="apidocSignatureSpan">d3.geoAzimuthalEqualAreaRaw.</span>invert (x, y)](#apidoc.element.d3.geoAzimuthalEqualAreaRaw.invert)
- description and source-code
```javascript
invert = function (x, y) {
  var z = sqrt(x * x + y * y),
      c = angle(z),
      sc = sin(c),
      cc = cos(c);
  return [
    atan2(x * sc, z * cc),
    asin(z && y * sc / z)
  ];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.geoAzimuthalEquidistantRaw"></a>[module d3.geoAzimuthalEquidistantRaw](#apidoc.module.d3.geoAzimuthalEquidistantRaw)

#### <a name="apidoc.element.d3.geoAzimuthalEquidistantRaw.geoAzimuthalEquidistantRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoAzimuthalEquidistantRaw (x, y)](#apidoc.element.d3.geoAzimuthalEquidistantRaw.geoAzimuthalEquidistantRaw)
- description and source-code
```javascript
geoAzimuthalEquidistantRaw = function (x, y) {
  var cx = cos(x),
      cy = cos(y),
      k = scale(cx * cy);
  return [
    k * cy * sin(x),
    k * sin(y)
  ];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoAzimuthalEquidistantRaw.invert"></a>[function <span class="apidocSignatureSpan">d3.geoAzimuthalEquidistantRaw.</span>invert (x, y)](#apidoc.element.d3.geoAzimuthalEquidistantRaw.invert)
- description and source-code
```javascript
invert = function (x, y) {
  var z = sqrt(x * x + y * y),
      c = angle(z),
      sc = sin(c),
      cc = cos(c);
  return [
    atan2(x * sc, z * cc),
    asin(z && y * sc / z)
  ];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.geoEquirectangularRaw"></a>[module d3.geoEquirectangularRaw](#apidoc.module.d3.geoEquirectangularRaw)

#### <a name="apidoc.element.d3.geoEquirectangularRaw.geoEquirectangularRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoEquirectangularRaw (lambda, phi)](#apidoc.element.d3.geoEquirectangularRaw.geoEquirectangularRaw)
- description and source-code
```javascript
function equirectangularRaw(lambda, phi) {
  return [lambda, phi];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoEquirectangularRaw.invert"></a>[function <span class="apidocSignatureSpan">d3.geoEquirectangularRaw.</span>invert (lambda, phi)](#apidoc.element.d3.geoEquirectangularRaw.invert)
- description and source-code
```javascript
function equirectangularRaw(lambda, phi) {
  return [lambda, phi];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.geoGnomonicRaw"></a>[module d3.geoGnomonicRaw](#apidoc.module.d3.geoGnomonicRaw)

#### <a name="apidoc.element.d3.geoGnomonicRaw.geoGnomonicRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoGnomonicRaw (x, y)](#apidoc.element.d3.geoGnomonicRaw.geoGnomonicRaw)
- description and source-code
```javascript
function gnomonicRaw(x, y) {
  var cy = cos(y), k = cos(x) * cy;
  return [cy * sin(x) / k, sin(y) / k];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoGnomonicRaw.invert"></a>[function <span class="apidocSignatureSpan">d3.geoGnomonicRaw.</span>invert (x, y)](#apidoc.element.d3.geoGnomonicRaw.invert)
- description and source-code
```javascript
invert = function (x, y) {
  var z = sqrt(x * x + y * y),
      c = angle(z),
      sc = sin(c),
      cc = cos(c);
  return [
    atan2(x * sc, z * cc),
    asin(z && y * sc / z)
  ];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.geoMercatorRaw"></a>[module d3.geoMercatorRaw](#apidoc.module.d3.geoMercatorRaw)

#### <a name="apidoc.element.d3.geoMercatorRaw.geoMercatorRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoMercatorRaw (lambda, phi)](#apidoc.element.d3.geoMercatorRaw.geoMercatorRaw)
- description and source-code
```javascript
function mercatorRaw(lambda, phi) {
  return [lambda, log(tan((halfPi + phi) / 2))];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoMercatorRaw.invert"></a>[function <span class="apidocSignatureSpan">d3.geoMercatorRaw.</span>invert (x, y)](#apidoc.element.d3.geoMercatorRaw.invert)
- description and source-code
```javascript
invert = function (x, y) {
  return [x, 2 * atan(exp(y)) - halfPi];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.geoOrthographicRaw"></a>[module d3.geoOrthographicRaw](#apidoc.module.d3.geoOrthographicRaw)

#### <a name="apidoc.element.d3.geoOrthographicRaw.geoOrthographicRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoOrthographicRaw (x, y)](#apidoc.element.d3.geoOrthographicRaw.geoOrthographicRaw)
- description and source-code
```javascript
function orthographicRaw(x, y) {
  return [cos(y) * sin(x), sin(y)];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoOrthographicRaw.invert"></a>[function <span class="apidocSignatureSpan">d3.geoOrthographicRaw.</span>invert (x, y)](#apidoc.element.d3.geoOrthographicRaw.invert)
- description and source-code
```javascript
invert = function (x, y) {
  var z = sqrt(x * x + y * y),
      c = angle(z),
      sc = sin(c),
      cc = cos(c);
  return [
    atan2(x * sc, z * cc),
    asin(z && y * sc / z)
  ];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.geoStereographicRaw"></a>[module d3.geoStereographicRaw](#apidoc.module.d3.geoStereographicRaw)

#### <a name="apidoc.element.d3.geoStereographicRaw.geoStereographicRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoStereographicRaw (x, y)](#apidoc.element.d3.geoStereographicRaw.geoStereographicRaw)
- description and source-code
```javascript
function stereographicRaw(x, y) {
  var cy = cos(y), k = 1 + cos(x) * cy;
  return [cy * sin(x) / k, sin(y) / k];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoStereographicRaw.invert"></a>[function <span class="apidocSignatureSpan">d3.geoStereographicRaw.</span>invert (x, y)](#apidoc.element.d3.geoStereographicRaw.invert)
- description and source-code
```javascript
invert = function (x, y) {
  var z = sqrt(x * x + y * y),
      c = angle(z),
      sc = sin(c),
      cc = cos(c);
  return [
    atan2(x * sc, z * cc),
    asin(z && y * sc / z)
  ];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.geoTransverseMercatorRaw"></a>[module d3.geoTransverseMercatorRaw](#apidoc.module.d3.geoTransverseMercatorRaw)

#### <a name="apidoc.element.d3.geoTransverseMercatorRaw.geoTransverseMercatorRaw"></a>[function <span class="apidocSignatureSpan">d3.</span>geoTransverseMercatorRaw (lambda, phi)](#apidoc.element.d3.geoTransverseMercatorRaw.geoTransverseMercatorRaw)
- description and source-code
```javascript
function transverseMercatorRaw(lambda, phi) {
  return [log(tan((halfPi + phi) / 2)), -lambda];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.geoTransverseMercatorRaw.invert"></a>[function <span class="apidocSignatureSpan">d3.geoTransverseMercatorRaw.</span>invert (x, y)](#apidoc.element.d3.geoTransverseMercatorRaw.invert)
- description and source-code
```javascript
invert = function (x, y) {
  return [-y, 2 * atan(exp(x)) - halfPi];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.hcl"></a>[module d3.hcl](#apidoc.module.d3.hcl)

#### <a name="apidoc.element.d3.hcl.hcl"></a>[function <span class="apidocSignatureSpan">d3.</span>hcl (h, c, l, opacity)](#apidoc.element.d3.hcl.hcl)
- description and source-code
```javascript
function hcl(h, c, l, opacity) {
  return arguments.length === 1 ? hclConvert(h) : new Hcl(h, c, l, opacity == null ? 1 : opacity);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.hcl.prototype"></a>[module d3.hcl.prototype](#apidoc.module.d3.hcl.prototype)

#### <a name="apidoc.element.d3.hcl.prototype.brighter"></a>[function <span class="apidocSignatureSpan">d3.hcl.prototype.</span>brighter (k)](#apidoc.element.d3.hcl.prototype.brighter)
- description and source-code
```javascript
brighter = function (k) {
  return new Hcl(this.h, this.c, this.l + Kn * (k == null ? 1 : k), this.opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hcl.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.hcl.prototype.</span>constructor (h, c, l, opacity)](#apidoc.element.d3.hcl.prototype.constructor)
- description and source-code
```javascript
function Hcl(h, c, l, opacity) {
  this.h = +h;
  this.c = +c;
  this.l = +l;
  this.opacity = +opacity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hcl.prototype.darker"></a>[function <span class="apidocSignatureSpan">d3.hcl.prototype.</span>darker (k)](#apidoc.element.d3.hcl.prototype.darker)
- description and source-code
```javascript
darker = function (k) {
  return new Hcl(this.h, this.c, this.l - Kn * (k == null ? 1 : k), this.opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hcl.prototype.rgb"></a>[function <span class="apidocSignatureSpan">d3.hcl.prototype.</span>rgb ()](#apidoc.element.d3.hcl.prototype.rgb)
- description and source-code
```javascript
rgb = function () {
  return labConvert(this).rgb();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.hcl.prototype.constructor"></a>[module d3.hcl.prototype.constructor](#apidoc.module.d3.hcl.prototype.constructor)

#### <a name="apidoc.element.d3.hcl.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.hcl.prototype.</span>constructor ()](#apidoc.element.d3.hcl.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.hierarchy"></a>[module d3.hierarchy](#apidoc.module.d3.hierarchy)

#### <a name="apidoc.element.d3.hierarchy.hierarchy"></a>[function <span class="apidocSignatureSpan">d3.</span>hierarchy (data, children)](#apidoc.element.d3.hierarchy.hierarchy)
- description and source-code
```javascript
function hierarchy(data, children) {
  var root = new Node(data),
      valued = +data.value && (root.value = data.value),
      node,
      nodes = [root],
      child,
      childs,
      i,
      n;

  if (children == null) children = defaultChildren;

  while (node = nodes.pop()) {
    if (valued) node.value = +node.data.value;
    if ((childs = children(node.data)) && (n = childs.length)) {
      node.children = new Array(n);
      for (i = n - 1; i >= 0; --i) {
        nodes.push(child = node.children[i] = new Node(childs[i]));
        child.parent = node;
        child.depth = node.depth + 1;
      }
    }
  }

  return root.eachBefore(computeHeight);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.hierarchy.prototype"></a>[module d3.hierarchy.prototype](#apidoc.module.d3.hierarchy.prototype)

#### <a name="apidoc.element.d3.hierarchy.prototype.ancestors"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>ancestors ()](#apidoc.element.d3.hierarchy.prototype.ancestors)
- description and source-code
```javascript
ancestors = function () {
  var node = this, nodes = [node];
  while (node = node.parent) {
    nodes.push(node);
  }
  return nodes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>constructor (data)](#apidoc.element.d3.hierarchy.prototype.constructor)
- description and source-code
```javascript
function Node(data) {
  this.data = data;
  this.depth =
  this.height = 0;
  this.parent = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.copy"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>copy ()](#apidoc.element.d3.hierarchy.prototype.copy)
- description and source-code
```javascript
function node_copy() {
  return hierarchy(this).eachBefore(copyData);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.count"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>count ()](#apidoc.element.d3.hierarchy.prototype.count)
- description and source-code
```javascript
count = function () {
  return this.eachAfter(count);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.descendants"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>descendants ()](#apidoc.element.d3.hierarchy.prototype.descendants)
- description and source-code
```javascript
descendants = function () {
  var nodes = [];
  this.each(function(node) {
    nodes.push(node);
  });
  return nodes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.each"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>each (callback)](#apidoc.element.d3.hierarchy.prototype.each)
- description and source-code
```javascript
each = function (callback) {
  var node = this, current, next = [node], children, i, n;
  do {
    current = next.reverse(), next = [];
    while (node = current.pop()) {
      callback(node), children = node.children;
      if (children) for (i = 0, n = children.length; i < n; ++i) {
        next.push(children[i]);
      }
    }
  } while (next.length);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.eachAfter"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>eachAfter (callback)](#apidoc.element.d3.hierarchy.prototype.eachAfter)
- description and source-code
```javascript
eachAfter = function (callback) {
  var node = this, nodes = [node], next = [], children, i, n;
  while (node = nodes.pop()) {
    next.push(node), children = node.children;
    if (children) for (i = 0, n = children.length; i < n; ++i) {
      nodes.push(children[i]);
    }
  }
  while (node = next.pop()) {
    callback(node);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.eachBefore"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>eachBefore (callback)](#apidoc.element.d3.hierarchy.prototype.eachBefore)
- description and source-code
```javascript
eachBefore = function (callback) {
  var node = this, nodes = [node], children, i;
  while (node = nodes.pop()) {
    callback(node), children = node.children;
    if (children) for (i = children.length - 1; i >= 0; --i) {
      nodes.push(children[i]);
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.leaves"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>leaves ()](#apidoc.element.d3.hierarchy.prototype.leaves)
- description and source-code
```javascript
leaves = function () {
  var leaves = [];
  this.eachBefore(function(node) {
    if (!node.children) {
      leaves.push(node);
    }
  });
  return leaves;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.links"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>links ()](#apidoc.element.d3.hierarchy.prototype.links)
- description and source-code
```javascript
links = function () {
  var root = this, links = [];
  root.each(function(node) {
    if (node !== root) { // Don’t include the root’s parent, if any.
      links.push({source: node.parent, target: node});
    }
  });
  return links;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.path"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>path (end)](#apidoc.element.d3.hierarchy.prototype.path)
- description and source-code
```javascript
path = function (end) {
  var start = this,
      ancestor = leastCommonAncestor(start, end),
      nodes = [start];
  while (start !== ancestor) {
    start = start.parent;
    nodes.push(start);
  }
  var k = nodes.length;
  while (end !== ancestor) {
    nodes.splice(k, 0, end);
    end = end.parent;
  }
  return nodes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.sort"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>sort (compare)](#apidoc.element.d3.hierarchy.prototype.sort)
- description and source-code
```javascript
sort = function (compare) {
  return this.eachBefore(function(node) {
    if (node.children) {
      node.children.sort(compare);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hierarchy.prototype.sum"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>sum (value)](#apidoc.element.d3.hierarchy.prototype.sum)
- description and source-code
```javascript
sum = function (value) {
  return this.eachAfter(function(node) {
    var sum = +value(node.data) || 0,
        children = node.children,
        i = children && children.length;
    while (--i >= 0) sum += children[i].value;
    node.value = sum;
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.hierarchy.prototype.constructor"></a>[module d3.hierarchy.prototype.constructor](#apidoc.module.d3.hierarchy.prototype.constructor)

#### <a name="apidoc.element.d3.hierarchy.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.hierarchy.prototype.</span>constructor ()](#apidoc.element.d3.hierarchy.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.hsl"></a>[module d3.hsl](#apidoc.module.d3.hsl)

#### <a name="apidoc.element.d3.hsl.hsl"></a>[function <span class="apidocSignatureSpan">d3.</span>hsl (h, s, l, opacity)](#apidoc.element.d3.hsl.hsl)
- description and source-code
```javascript
function hsl(h, s, l, opacity) {
  return arguments.length === 1 ? hslConvert(h) : new Hsl(h, s, l, opacity == null ? 1 : opacity);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.hsl.prototype"></a>[module d3.hsl.prototype](#apidoc.module.d3.hsl.prototype)

#### <a name="apidoc.element.d3.hsl.prototype.brighter"></a>[function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>brighter (k)](#apidoc.element.d3.hsl.prototype.brighter)
- description and source-code
```javascript
brighter = function (k) {
  k = k == null ? brighter : Math.pow(brighter, k);
  return new Hsl(this.h, this.s, this.l * k, this.opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hsl.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>constructor (h, s, l, opacity)](#apidoc.element.d3.hsl.prototype.constructor)
- description and source-code
```javascript
function Hsl(h, s, l, opacity) {
  this.h = +h;
  this.s = +s;
  this.l = +l;
  this.opacity = +opacity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hsl.prototype.darker"></a>[function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>darker (k)](#apidoc.element.d3.hsl.prototype.darker)
- description and source-code
```javascript
darker = function (k) {
  k = k == null ? darker : Math.pow(darker, k);
  return new Hsl(this.h, this.s, this.l * k, this.opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hsl.prototype.displayable"></a>[function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>displayable ()](#apidoc.element.d3.hsl.prototype.displayable)
- description and source-code
```javascript
displayable = function () {
  return (0 <= this.s && this.s <= 1 || isNaN(this.s))
      && (0 <= this.l && this.l <= 1)
      && (0 <= this.opacity && this.opacity <= 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.hsl.prototype.rgb"></a>[function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>rgb ()](#apidoc.element.d3.hsl.prototype.rgb)
- description and source-code
```javascript
rgb = function () {
  var h = this.h % 360 + (this.h < 0) * 360,
      s = isNaN(h) || isNaN(this.s) ? 0 : this.s,
      l = this.l,
      m2 = l + (l < 0.5 ? l : 1 - l) * s,
      m1 = 2 * l - m2;
  return new Rgb(
    hsl2rgb(h >= 240 ? h - 240 : h + 120, m1, m2),
    hsl2rgb(h, m1, m2),
    hsl2rgb(h < 120 ? h + 240 : h - 120, m1, m2),
    this.opacity
  );
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.hsl.prototype.constructor"></a>[module d3.hsl.prototype.constructor](#apidoc.module.d3.hsl.prototype.constructor)

#### <a name="apidoc.element.d3.hsl.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.hsl.prototype.</span>constructor ()](#apidoc.element.d3.hsl.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.interpolateCubehelix"></a>[module d3.interpolateCubehelix](#apidoc.module.d3.interpolateCubehelix)

#### <a name="apidoc.element.d3.interpolateCubehelix.interpolateCubehelix"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateCubehelix (start, end)](#apidoc.element.d3.interpolateCubehelix.interpolateCubehelix)
- description and source-code
```javascript
function cubehelix$$1(start, end) {
  var h = hue$$1((start = d3Color.cubehelix(start)).h, (end = d3Color.cubehelix(end)).h),
      s = nogamma(start.s, end.s),
      l = nogamma(start.l, end.l),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.h = h(t);
    start.s = s(t);
    start.l = l(Math.pow(t, y));
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateCubehelix.gamma"></a>[function <span class="apidocSignatureSpan">d3.interpolateCubehelix.</span>gamma (y)](#apidoc.element.d3.interpolateCubehelix.gamma)
- description and source-code
```javascript
function cubehelixGamma(y) {
  y = +y;

  function cubehelix$$1(start, end) {
    var h = hue$$1((start = d3Color.cubehelix(start)).h, (end = d3Color.cubehelix(end)).h),
        s = nogamma(start.s, end.s),
        l = nogamma(start.l, end.l),
        opacity = nogamma(start.opacity, end.opacity);
    return function(t) {
      start.h = h(t);
      start.s = s(t);
      start.l = l(Math.pow(t, y));
      start.opacity = opacity(t);
      return start + "";
    };
  }

  cubehelix$$1.gamma = cubehelixGamma;

  return cubehelix$$1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.interpolateCubehelixLong"></a>[module d3.interpolateCubehelixLong](#apidoc.module.d3.interpolateCubehelixLong)

#### <a name="apidoc.element.d3.interpolateCubehelixLong.interpolateCubehelixLong"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateCubehelixLong (start, end)](#apidoc.element.d3.interpolateCubehelixLong.interpolateCubehelixLong)
- description and source-code
```javascript
function cubehelix$$1(start, end) {
  var h = hue$$1((start = d3Color.cubehelix(start)).h, (end = d3Color.cubehelix(end)).h),
      s = nogamma(start.s, end.s),
      l = nogamma(start.l, end.l),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.h = h(t);
    start.s = s(t);
    start.l = l(Math.pow(t, y));
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateCubehelixLong.gamma"></a>[function <span class="apidocSignatureSpan">d3.interpolateCubehelixLong.</span>gamma (y)](#apidoc.element.d3.interpolateCubehelixLong.gamma)
- description and source-code
```javascript
function cubehelixGamma(y) {
  y = +y;

  function cubehelix$$1(start, end) {
    var h = hue$$1((start = d3Color.cubehelix(start)).h, (end = d3Color.cubehelix(end)).h),
        s = nogamma(start.s, end.s),
        l = nogamma(start.l, end.l),
        opacity = nogamma(start.opacity, end.opacity);
    return function(t) {
      start.h = h(t);
      start.s = s(t);
      start.l = l(Math.pow(t, y));
      start.opacity = opacity(t);
      return start + "";
    };
  }

  cubehelix$$1.gamma = cubehelixGamma;

  return cubehelix$$1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.interpolateRgb"></a>[module d3.interpolateRgb](#apidoc.module.d3.interpolateRgb)

#### <a name="apidoc.element.d3.interpolateRgb.interpolateRgb"></a>[function <span class="apidocSignatureSpan">d3.</span>interpolateRgb (start, end)](#apidoc.element.d3.interpolateRgb.interpolateRgb)
- description and source-code
```javascript
function rgb$$1(start, end) {
  var r = color$$1((start = d3Color.rgb(start)).r, (end = d3Color.rgb(end)).r),
      g = color$$1(start.g, end.g),
      b = color$$1(start.b, end.b),
      opacity = nogamma(start.opacity, end.opacity);
  return function(t) {
    start.r = r(t);
    start.g = g(t);
    start.b = b(t);
    start.opacity = opacity(t);
    return start + "";
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.interpolateRgb.gamma"></a>[function <span class="apidocSignatureSpan">d3.interpolateRgb.</span>gamma (y)](#apidoc.element.d3.interpolateRgb.gamma)
- description and source-code
```javascript
function rgbGamma(y) {
  var color$$1 = gamma(y);

  function rgb$$1(start, end) {
    var r = color$$1((start = d3Color.rgb(start)).r, (end = d3Color.rgb(end)).r),
        g = color$$1(start.g, end.g),
        b = color$$1(start.b, end.b),
        opacity = nogamma(start.opacity, end.opacity);
    return function(t) {
      start.r = r(t);
      start.g = g(t);
      start.b = b(t);
      start.opacity = opacity(t);
      return start + "";
    };
  }

  rgb$$1.gamma = rgbGamma;

  return rgb$$1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.lab"></a>[module d3.lab](#apidoc.module.d3.lab)

#### <a name="apidoc.element.d3.lab.lab"></a>[function <span class="apidocSignatureSpan">d3.</span>lab (l, a, b, opacity)](#apidoc.element.d3.lab.lab)
- description and source-code
```javascript
function lab(l, a, b, opacity) {
  return arguments.length === 1 ? labConvert(l) : new Lab(l, a, b, opacity == null ? 1 : opacity);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.lab.prototype"></a>[module d3.lab.prototype](#apidoc.module.d3.lab.prototype)

#### <a name="apidoc.element.d3.lab.prototype.brighter"></a>[function <span class="apidocSignatureSpan">d3.lab.prototype.</span>brighter (k)](#apidoc.element.d3.lab.prototype.brighter)
- description and source-code
```javascript
brighter = function (k) {
  return new Lab(this.l + Kn * (k == null ? 1 : k), this.a, this.b, this.opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.lab.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.lab.prototype.</span>constructor (l, a, b, opacity)](#apidoc.element.d3.lab.prototype.constructor)
- description and source-code
```javascript
function Lab(l, a, b, opacity) {
  this.l = +l;
  this.a = +a;
  this.b = +b;
  this.opacity = +opacity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.lab.prototype.darker"></a>[function <span class="apidocSignatureSpan">d3.lab.prototype.</span>darker (k)](#apidoc.element.d3.lab.prototype.darker)
- description and source-code
```javascript
darker = function (k) {
  return new Lab(this.l - Kn * (k == null ? 1 : k), this.a, this.b, this.opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.lab.prototype.rgb"></a>[function <span class="apidocSignatureSpan">d3.lab.prototype.</span>rgb ()](#apidoc.element.d3.lab.prototype.rgb)
- description and source-code
```javascript
rgb = function () {
  var y = (this.l + 16) / 116,
      x = isNaN(this.a) ? y : y + this.a / 500,
      z = isNaN(this.b) ? y : y - this.b / 200;
  y = Yn * lab2xyz(y);
  x = Xn * lab2xyz(x);
  z = Zn * lab2xyz(z);
  return new Rgb(
    xyz2rgb( 3.2404542 * x - 1.5371385 * y - 0.4985314 * z), // D65 -> sRGB
    xyz2rgb(-0.9692660 * x + 1.8760108 * y + 0.0415560 * z),
    xyz2rgb( 0.0556434 * x - 0.2040259 * y + 1.0572252 * z),
    this.opacity
  );
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.lab.prototype.constructor"></a>[module d3.lab.prototype.constructor](#apidoc.module.d3.lab.prototype.constructor)

#### <a name="apidoc.element.d3.lab.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.lab.prototype.</span>constructor ()](#apidoc.element.d3.lab.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.local"></a>[module d3.local](#apidoc.module.d3.local)

#### <a name="apidoc.element.d3.local.local"></a>[function <span class="apidocSignatureSpan">d3.</span>local ()](#apidoc.element.d3.local.local)
- description and source-code
```javascript
function local() {
  return new Local;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.local.prototype"></a>[module d3.local.prototype](#apidoc.module.d3.local.prototype)

#### <a name="apidoc.element.d3.local.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.local.prototype.</span>constructor ()](#apidoc.element.d3.local.prototype.constructor)
- description and source-code
```javascript
function Local() {
  this._ = "@" + (++nextId).toString(36);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.local.prototype.get"></a>[function <span class="apidocSignatureSpan">d3.local.prototype.</span>get (node)](#apidoc.element.d3.local.prototype.get)
- description and source-code
```javascript
get = function (node) {
  var id = this._;
  while (!(id in node)) if (!(node = node.parentNode)) return;
  return node[id];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.local.prototype.remove"></a>[function <span class="apidocSignatureSpan">d3.local.prototype.</span>remove (node)](#apidoc.element.d3.local.prototype.remove)
- description and source-code
```javascript
remove = function (node) {
  return this._ in node && delete node[this._];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.local.prototype.set"></a>[function <span class="apidocSignatureSpan">d3.local.prototype.</span>set (node, value)](#apidoc.element.d3.local.prototype.set)
- description and source-code
```javascript
set = function (node, value) {
  return node[this._] = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.local.prototype.toString"></a>[function <span class="apidocSignatureSpan">d3.local.prototype.</span>toString ()](#apidoc.element.d3.local.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this._;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.local.prototype.constructor"></a>[module d3.local.prototype.constructor](#apidoc.module.d3.local.prototype.constructor)

#### <a name="apidoc.element.d3.local.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.local.prototype.</span>constructor ()](#apidoc.element.d3.local.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.map"></a>[module d3.map](#apidoc.module.d3.map)

#### <a name="apidoc.element.d3.map.map"></a>[function <span class="apidocSignatureSpan">d3.</span>map (object, f)](#apidoc.element.d3.map.map)
- description and source-code
```javascript
function map(object, f) {
  var map = new Map;

  // Copy constructor.
  if (object instanceof Map) object.each(function(value, key) { map.set(key, value); });

  // Index array by numeric index or specified key function.
  else if (Array.isArray(object)) {
    var i = -1,
        n = object.length,
        o;

    if (f == null) while (++i < n) map.set(i, object[i]);
    else while (++i < n) map.set(f(o = object[i], i, object), o);
  }

  // Convert object to map.
  else if (object) for (var key in object) map.set(key, object[key]);

  return map;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.map.prototype"></a>[module d3.map.prototype](#apidoc.module.d3.map.prototype)

#### <a name="apidoc.element.d3.map.prototype.clear"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>clear ()](#apidoc.element.d3.map.prototype.clear)
- description and source-code
```javascript
clear = function () {
  for (var property in this) if (property[0] === prefix) delete this[property];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>constructor ()](#apidoc.element.d3.map.prototype.constructor)
- description and source-code
```javascript
function Map() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.each"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>each (f)](#apidoc.element.d3.map.prototype.each)
- description and source-code
```javascript
each = function (f) {
  for (var property in this) if (property[0] === prefix) f(this[property], property.slice(1), this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.empty"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>empty ()](#apidoc.element.d3.map.prototype.empty)
- description and source-code
```javascript
empty = function () {
  for (var property in this) if (property[0] === prefix) return false;
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.entries"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>entries ()](#apidoc.element.d3.map.prototype.entries)
- description and source-code
```javascript
entries = function () {
  var entries = [];
  for (var property in this) if (property[0] === prefix) entries.push({key: property.slice(1), value: this[property]});
  return entries;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.get"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>get (key)](#apidoc.element.d3.map.prototype.get)
- description and source-code
```javascript
get = function (key) {
  return this[prefix + key];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.has"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>has (key)](#apidoc.element.d3.map.prototype.has)
- description and source-code
```javascript
has = function (key) {
  return (prefix + key) in this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.keys"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>keys ()](#apidoc.element.d3.map.prototype.keys)
- description and source-code
```javascript
keys = function () {
  var keys = [];
  for (var property in this) if (property[0] === prefix) keys.push(property.slice(1));
  return keys;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.remove"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>remove (key)](#apidoc.element.d3.map.prototype.remove)
- description and source-code
```javascript
remove = function (key) {
  var property = prefix + key;
  return property in this && delete this[property];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.set"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>set (key, value)](#apidoc.element.d3.map.prototype.set)
- description and source-code
```javascript
set = function (key, value) {
  this[prefix + key] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.size"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>size ()](#apidoc.element.d3.map.prototype.size)
- description and source-code
```javascript
size = function () {
  var size = 0;
  for (var property in this) if (property[0] === prefix) ++size;
  return size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.map.prototype.values"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>values ()](#apidoc.element.d3.map.prototype.values)
- description and source-code
```javascript
values = function () {
  var values = [];
  for (var property in this) if (property[0] === prefix) values.push(this[property]);
  return values;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.map.prototype.constructor"></a>[module d3.map.prototype.constructor](#apidoc.module.d3.map.prototype.constructor)

#### <a name="apidoc.element.d3.map.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.map.prototype.</span>constructor ()](#apidoc.element.d3.map.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.path"></a>[module d3.path](#apidoc.module.d3.path)

#### <a name="apidoc.element.d3.path.path"></a>[function <span class="apidocSignatureSpan">d3.</span>path ()](#apidoc.element.d3.path.path)
- description and source-code
```javascript
function path() {
  return new Path;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.path.prototype"></a>[module d3.path.prototype](#apidoc.module.d3.path.prototype)

#### <a name="apidoc.element.d3.path.prototype.arc"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>arc (x, y, r, a0, a1, ccw)](#apidoc.element.d3.path.prototype.arc)
- description and source-code
```javascript
arc = function (x, y, r, a0, a1, ccw) {
  x = +x, y = +y, r = +r;
  var dx = r * Math.cos(a0),
      dy = r * Math.sin(a0),
      x0 = x + dx,
      y0 = y + dy,
      cw = 1 ^ ccw,
      da = ccw ? a0 - a1 : a1 - a0;

  // Is the radius negative? Error.
  if (r < 0) throw new Error("negative radius: " + r);

  // Is this path empty? Move to (x0,y0).
  if (this._x1 === null) {
    this._ += "M" + x0 + "," + y0;
  }

  // Or, is (x0,y0) not coincident with the previous point? Line to (x0,y0).
  else if (Math.abs(this._x1 - x0) > epsilon || Math.abs(this._y1 - y0) > epsilon) {
    this._ += "L" + x0 + "," + y0;
  }

  // Is this arc empty? We’re done.
  if (!r) return;

  // Does the angle go the wrong way? Flip the direction.
  if (da < 0) da = da % tau + tau;

  // Is this a complete circle? Draw two arcs to complete the circle.
  if (da > tauEpsilon) {
    this._ += "A" + r + "," + r + ",0,1," + cw + "," + (x - dx) + "," + (y - dy) + "A" + r + "," + r + ",0,1," + cw + "," + (this
._x1 = x0) + "," + (this._y1 = y0);
  }

  // Is this arc non-empty? Draw an arc!
  else if (da > epsilon) {
    this._ += "A" + r + "," + r + ",0," + (+(da >= pi)) + "," + cw + "," + (this._x1 = x + r * Math.cos(a1)) + "," + (this._y1 =
y + r * Math.sin(a1));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path.prototype.arcTo"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>arcTo (x1, y1, x2, y2, r)](#apidoc.element.d3.path.prototype.arcTo)
- description and source-code
```javascript
arcTo = function (x1, y1, x2, y2, r) {
  x1 = +x1, y1 = +y1, x2 = +x2, y2 = +y2, r = +r;
  var x0 = this._x1,
      y0 = this._y1,
      x21 = x2 - x1,
      y21 = y2 - y1,
      x01 = x0 - x1,
      y01 = y0 - y1,
      l01_2 = x01 * x01 + y01 * y01;

  // Is the radius negative? Error.
  if (r < 0) throw new Error("negative radius: " + r);

  // Is this path empty? Move to (x1,y1).
  if (this._x1 === null) {
    this._ += "M" + (this._x1 = x1) + "," + (this._y1 = y1);
  }

  // Or, is (x1,y1) coincident with (x0,y0)? Do nothing.
  else if (!(l01_2 > epsilon)) {}

  // Or, are (x0,y0), (x1,y1) and (x2,y2) collinear?
  // Equivalently, is (x1,y1) coincident with (x2,y2)?
  // Or, is the radius zero? Line to (x1,y1).
  else if (!(Math.abs(y01 * x21 - y21 * x01) > epsilon) || !r) {
    this._ += "L" + (this._x1 = x1) + "," + (this._y1 = y1);
  }

  // Otherwise, draw an arc!
  else {
    var x20 = x2 - x0,
        y20 = y2 - y0,
        l21_2 = x21 * x21 + y21 * y21,
        l20_2 = x20 * x20 + y20 * y20,
        l21 = Math.sqrt(l21_2),
        l01 = Math.sqrt(l01_2),
        l = r * Math.tan((pi - Math.acos((l21_2 + l01_2 - l20_2) / (2 * l21 * l01))) / 2),
        t01 = l / l01,
        t21 = l / l21;

    // If the start tangent is not coincident with (x0,y0), line to.
    if (Math.abs(t01 - 1) > epsilon) {
      this._ += "L" + (x1 + t01 * x01) + "," + (y1 + t01 * y01);
    }

    this._ += "A" + r + "," + r + ",0,0," + (+(y01 * x20 > x01 * y20)) + "," + (this._x1 = x1 + t21 * x21) + "," + (this._y1 = y1
 + t21 * y21);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path.prototype.bezierCurveTo"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>bezierCurveTo (x1, y1, x2, y2, x, y)](#apidoc.element.d3.path.prototype.bezierCurveTo)
- description and source-code
```javascript
bezierCurveTo = function (x1, y1, x2, y2, x, y) {
  this._ += "C" + (+x1) + "," + (+y1) + "," + (+x2) + "," + (+y2) + "," + (this._x1 = +x) + "," + (this._y1 = +y);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path.prototype.closePath"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>closePath ()](#apidoc.element.d3.path.prototype.closePath)
- description and source-code
```javascript
closePath = function () {
  if (this._x1 !== null) {
    this._x1 = this._x0, this._y1 = this._y0;
    this._ += "Z";
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>constructor ()](#apidoc.element.d3.path.prototype.constructor)
- description and source-code
```javascript
function Path() {
  this._x0 = this._y0 = // start of current subpath
  this._x1 = this._y1 = null; // end of current subpath
  this._ = "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path.prototype.lineTo"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>lineTo (x, y)](#apidoc.element.d3.path.prototype.lineTo)
- description and source-code
```javascript
lineTo = function (x, y) {
  this._ += "L" + (this._x1 = +x) + "," + (this._y1 = +y);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path.prototype.moveTo"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>moveTo (x, y)](#apidoc.element.d3.path.prototype.moveTo)
- description and source-code
```javascript
moveTo = function (x, y) {
  this._ += "M" + (this._x0 = this._x1 = +x) + "," + (this._y0 = this._y1 = +y);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path.prototype.quadraticCurveTo"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>quadraticCurveTo (x1, y1, x, y)](#apidoc.element.d3.path.prototype.quadraticCurveTo)
- description and source-code
```javascript
quadraticCurveTo = function (x1, y1, x, y) {
  this._ += "Q" + (+x1) + "," + (+y1) + "," + (this._x1 = +x) + "," + (this._y1 = +y);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path.prototype.rect"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>rect (x, y, w, h)](#apidoc.element.d3.path.prototype.rect)
- description and source-code
```javascript
rect = function (x, y, w, h) {
  this._ += "M" + (this._x0 = this._x1 = +x) + "," + (this._y0 = this._y1 = +y) + "h" + (+w) + "v" + (+h) + "h" + (-w) + "Z";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.path.prototype.toString"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>toString ()](#apidoc.element.d3.path.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this._;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.path.prototype.constructor"></a>[module d3.path.prototype.constructor](#apidoc.module.d3.path.prototype.constructor)

#### <a name="apidoc.element.d3.path.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.path.prototype.</span>constructor ()](#apidoc.element.d3.path.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.quadtree"></a>[module d3.quadtree](#apidoc.module.d3.quadtree)

#### <a name="apidoc.element.d3.quadtree.quadtree"></a>[function <span class="apidocSignatureSpan">d3.</span>quadtree (nodes, x, y)](#apidoc.element.d3.quadtree.quadtree)
- description and source-code
```javascript
function quadtree(nodes, x, y) {
  var tree = new Quadtree(x == null ? defaultX : x, y == null ? defaultY : y, NaN, NaN, NaN, NaN);
  return nodes == null ? tree : tree.addAll(nodes);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.quadtree.prototype"></a>[module d3.quadtree.prototype](#apidoc.module.d3.quadtree.prototype)

#### <a name="apidoc.element.d3.quadtree.prototype.add"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>add (d)](#apidoc.element.d3.quadtree.prototype.add)
- description and source-code
```javascript
add = function (d) {
  var x = +this._x.call(null, d),
      y = +this._y.call(null, d);
  return add(this.cover(x, y), x, y, d);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.addAll"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>addAll (data)](#apidoc.element.d3.quadtree.prototype.addAll)
- description and source-code
```javascript
function addAll(data) {
  var d, i, n = data.length,
      x,
      y,
      xz = new Array(n),
      yz = new Array(n),
      x0 = Infinity,
      y0 = Infinity,
      x1 = -Infinity,
      y1 = -Infinity;

  // Compute the points and their extent.
  for (i = 0; i < n; ++i) {
    if (isNaN(x = +this._x.call(null, d = data[i])) || isNaN(y = +this._y.call(null, d))) continue;
    xz[i] = x;
    yz[i] = y;
    if (x < x0) x0 = x;
    if (x > x1) x1 = x;
    if (y < y0) y0 = y;
    if (y > y1) y1 = y;
  }

  // If there were no (valid) points, inherit the existing extent.
  if (x1 < x0) x0 = this._x0, x1 = this._x1;
  if (y1 < y0) y0 = this._y0, y1 = this._y1;

  // Expand the tree to cover the new points.
  this.cover(x0, y0).cover(x1, y1);

  // Add the new points.
  for (i = 0; i < n; ++i) {
    add(this, xz[i], yz[i], data[i]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.copy"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>copy ()](#apidoc.element.d3.quadtree.prototype.copy)
- description and source-code
```javascript
copy = function () {
  var copy = new Quadtree(this._x, this._y, this._x0, this._y0, this._x1, this._y1),
      node = this._root,
      nodes,
      child;

  if (!node) return copy;

  if (!node.length) return copy._root = leaf_copy(node), copy;

  nodes = [{source: node, target: copy._root = new Array(4)}];
  while (node = nodes.pop()) {
    for (var i = 0; i < 4; ++i) {
      if (child = node.source[i]) {
        if (child.length) nodes.push({source: child, target: node.target[i] = new Array(4)});
        else node.target[i] = leaf_copy(child);
      }
    }
  }

  return copy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.cover"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>cover (x, y)](#apidoc.element.d3.quadtree.prototype.cover)
- description and source-code
```javascript
cover = function (x, y) {
  if (isNaN(x = +x) || isNaN(y = +y)) return this; // ignore invalid points

  var x0 = this._x0,
      y0 = this._y0,
      x1 = this._x1,
      y1 = this._y1;

  // If the quadtree has no extent, initialize them.
  // Integer extent are necessary so that if we later double the extent,
  // the existing quadrant boundaries don’t change due to floating point error!
  if (isNaN(x0)) {
    x1 = (x0 = Math.floor(x)) + 1;
    y1 = (y0 = Math.floor(y)) + 1;
  }

  // Otherwise, double repeatedly to cover.
  else if (x0 > x || x > x1 || y0 > y || y > y1) {
    var z = x1 - x0,
        node = this._root,
        parent,
        i;

    switch (i = (y < (y0 + y1) / 2) << 1 | (x < (x0 + x1) / 2)) {
      case 0: {
        do parent = new Array(4), parent[i] = node, node = parent;
        while (z *= 2, x1 = x0 + z, y1 = y0 + z, x > x1 || y > y1);
        break;
      }
      case 1: {
        do parent = new Array(4), parent[i] = node, node = parent;
        while (z *= 2, x0 = x1 - z, y1 = y0 + z, x0 > x || y > y1);
        break;
      }
      case 2: {
        do parent = new Array(4), parent[i] = node, node = parent;
        while (z *= 2, x1 = x0 + z, y0 = y1 - z, x > x1 || y0 > y);
        break;
      }
      case 3: {
        do parent = new Array(4), parent[i] = node, node = parent;
        while (z *= 2, x0 = x1 - z, y0 = y1 - z, x0 > x || y0 > y);
        break;
      }
    }

    if (this._root && this._root.length) this._root = node;
  }

  // If the quadtree covers the point already, just return.
  else return this;

  this._x0 = x0;
  this._y0 = y0;
  this._x1 = x1;
  this._y1 = y1;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.data"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>data ()](#apidoc.element.d3.quadtree.prototype.data)
- description and source-code
```javascript
data = function () {
  var data = [];
  this.visit(function(node) {
    if (!node.length) do data.push(node.data); while (node = node.next)
  });
  return data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.extent"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>extent (_)](#apidoc.element.d3.quadtree.prototype.extent)
- description and source-code
```javascript
extent = function (_) {
  return arguments.length
      ? this.cover(+_[0][0], +_[0][1]).cover(+_[1][0], +_[1][1])
      : isNaN(this._x0) ? undefined : [[this._x0, this._y0], [this._x1, this._y1]];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.find"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>find (x, y, radius)](#apidoc.element.d3.quadtree.prototype.find)
- description and source-code
```javascript
find = function (x, y, radius) {
  var data,
      x0 = this._x0,
      y0 = this._y0,
      x1,
      y1,
      x2,
      y2,
      x3 = this._x1,
      y3 = this._y1,
      quads = [],
      node = this._root,
      q,
      i;

  if (node) quads.push(new Quad(node, x0, y0, x3, y3));
  if (radius == null) radius = Infinity;
  else {
    x0 = x - radius, y0 = y - radius;
    x3 = x + radius, y3 = y + radius;
    radius *= radius;
  }

  while (q = quads.pop()) {

    // Stop searching if this quadrant can’t contain a closer node.
    if (!(node = q.node)
        || (x1 = q.x0) > x3
        || (y1 = q.y0) > y3
        || (x2 = q.x1) < x0
        || (y2 = q.y1) < y0) continue;

    // Bisect the current quadrant.
    if (node.length) {
      var xm = (x1 + x2) / 2,
          ym = (y1 + y2) / 2;

      quads.push(
        new Quad(node[3], xm, ym, x2, y2),
        new Quad(node[2], x1, ym, xm, y2),
        new Quad(node[1], xm, y1, x2, ym),
        new Quad(node[0], x1, y1, xm, ym)
      );

      // Visit the closest quadrant first.
      if (i = (y >= ym) << 1 | (x >= xm)) {
        q = quads[quads.length - 1];
        quads[quads.length - 1] = quads[quads.length - 1 - i];
        quads[quads.length - 1 - i] = q;
      }
    }

    // Visit this point. (Visiting coincident points isn’t necessary!)
    else {
      var dx = x - +this._x.call(null, node.data),
          dy = y - +this._y.call(null, node.data),
          d2 = dx * dx + dy * dy;
      if (d2 < radius) {
        var d = Math.sqrt(radius = d2);
        x0 = x - d, y0 = y - d;
        x3 = x + d, y3 = y + d;
        data = node.data;
      }
    }
  }

  return data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.remove"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>remove (d)](#apidoc.element.d3.quadtree.prototype.remove)
- description and source-code
```javascript
remove = function (d) {
  if (isNaN(x = +this._x.call(null, d)) || isNaN(y = +this._y.call(null, d))) return this; // ignore invalid points

  var parent,
      node = this._root,
      retainer,
      previous,
      next,
      x0 = this._x0,
      y0 = this._y0,
      x1 = this._x1,
      y1 = this._y1,
      x,
      y,
      xm,
      ym,
      right,
      bottom,
      i,
      j;

  // If the tree is empty, initialize the root as a leaf.
  if (!node) return this;

  // Find the leaf node for the point.
  // While descending, also retain the deepest parent with a non-removed sibling.
  if (node.length) while (true) {
    if (right = x >= (xm = (x0 + x1) / 2)) x0 = xm; else x1 = xm;
    if (bottom = y >= (ym = (y0 + y1) / 2)) y0 = ym; else y1 = ym;
    if (!(parent = node, node = node[i = bottom << 1 | right])) return this;
    if (!node.length) break;
    if (parent[(i + 1) & 3] || parent[(i + 2) & 3] || parent[(i + 3) & 3]) retainer = parent, j = i;
  }

  // Find the point to remove.
  while (node.data !== d) if (!(previous = node, node = node.next)) return this;
  if (next = node.next) delete node.next;

  // If there are multiple coincident points, remove just the point.
  if (previous) return (next ? previous.next = next : delete previous.next), this;

  // If this is the root point, remove it.
  if (!parent) return this._root = next, this;

  // Remove this leaf.
  next ? parent[i] = next : delete parent[i];

  // If the parent now contains exactly one leaf, collapse superfluous parents.
  if ((node = parent[0] || parent[1] || parent[2] || parent[3])
      && node === (parent[3] || parent[2] || parent[1] || parent[0])
      && !node.length) {
    if (retainer) retainer[j] = node;
    else this._root = node;
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.removeAll"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>removeAll (data)](#apidoc.element.d3.quadtree.prototype.removeAll)
- description and source-code
```javascript
function removeAll(data) {
  for (var i = 0, n = data.length; i < n; ++i) this.remove(data[i]);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.root"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>root ()](#apidoc.element.d3.quadtree.prototype.root)
- description and source-code
```javascript
root = function () {
  return this._root;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.size"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>size ()](#apidoc.element.d3.quadtree.prototype.size)
- description and source-code
```javascript
size = function () {
  var size = 0;
  this.visit(function(node) {
    if (!node.length) do ++size; while (node = node.next)
  });
  return size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.visit"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>visit (callback)](#apidoc.element.d3.quadtree.prototype.visit)
- description and source-code
```javascript
visit = function (callback) {
  var quads = [], q, node = this._root, child, x0, y0, x1, y1;
  if (node) quads.push(new Quad(node, this._x0, this._y0, this._x1, this._y1));
  while (q = quads.pop()) {
    if (!callback(node = q.node, x0 = q.x0, y0 = q.y0, x1 = q.x1, y1 = q.y1) && node.length) {
      var xm = (x0 + x1) / 2, ym = (y0 + y1) / 2;
      if (child = node[3]) quads.push(new Quad(child, xm, ym, x1, y1));
      if (child = node[2]) quads.push(new Quad(child, x0, ym, xm, y1));
      if (child = node[1]) quads.push(new Quad(child, xm, y0, x1, ym));
      if (child = node[0]) quads.push(new Quad(child, x0, y0, xm, ym));
    }
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.visitAfter"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>visitAfter (callback)](#apidoc.element.d3.quadtree.prototype.visitAfter)
- description and source-code
```javascript
visitAfter = function (callback) {
  var quads = [], next = [], q;
  if (this._root) quads.push(new Quad(this._root, this._x0, this._y0, this._x1, this._y1));
  while (q = quads.pop()) {
    var node = q.node;
    if (node.length) {
      var child, x0 = q.x0, y0 = q.y0, x1 = q.x1, y1 = q.y1, xm = (x0 + x1) / 2, ym = (y0 + y1) / 2;
      if (child = node[0]) quads.push(new Quad(child, x0, y0, xm, ym));
      if (child = node[1]) quads.push(new Quad(child, xm, y0, x1, ym));
      if (child = node[2]) quads.push(new Quad(child, x0, ym, xm, y1));
      if (child = node[3]) quads.push(new Quad(child, xm, ym, x1, y1));
    }
    next.push(q);
  }
  while (q = next.pop()) {
    callback(q.node, q.x0, q.y0, q.x1, q.y1);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.x"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>x (_)](#apidoc.element.d3.quadtree.prototype.x)
- description and source-code
```javascript
x = function (_) {
  return arguments.length ? (this._x = _, this) : this._x;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.quadtree.prototype.y"></a>[function <span class="apidocSignatureSpan">d3.quadtree.prototype.</span>y (_)](#apidoc.element.d3.quadtree.prototype.y)
- description and source-code
```javascript
y = function (_) {
  return arguments.length ? (this._y = _, this) : this._y;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.queue"></a>[module d3.queue](#apidoc.module.d3.queue)

#### <a name="apidoc.element.d3.queue.queue"></a>[function <span class="apidocSignatureSpan">d3.</span>queue (concurrency)](#apidoc.element.d3.queue.queue)
- description and source-code
```javascript
function queue(concurrency) {
  return new Queue(arguments.length ? +concurrency : Infinity);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.queue.prototype"></a>[module d3.queue.prototype](#apidoc.module.d3.queue.prototype)

#### <a name="apidoc.element.d3.queue.prototype.abort"></a>[function <span class="apidocSignatureSpan">d3.queue.prototype.</span>abort ()](#apidoc.element.d3.queue.prototype.abort)
- description and source-code
```javascript
abort = function () {
  if (this._error == null) abort(this, new Error("abort"));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.queue.prototype.await"></a>[function <span class="apidocSignatureSpan">d3.queue.prototype.</span>await (callback)](#apidoc.element.d3.queue.prototype.await)
- description and source-code
```javascript
await = function (callback) {
  if (typeof callback !== "function" || this._call) throw new Error;
  this._call = function(error, results) { callback.apply(null, [error].concat(results)); };
  maybeNotify(this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.queue.prototype.awaitAll"></a>[function <span class="apidocSignatureSpan">d3.queue.prototype.</span>awaitAll (callback)](#apidoc.element.d3.queue.prototype.awaitAll)
- description and source-code
```javascript
awaitAll = function (callback) {
  if (typeof callback !== "function" || this._call) throw new Error;
  this._call = callback;
  maybeNotify(this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.queue.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.queue.prototype.</span>constructor (size)](#apidoc.element.d3.queue.prototype.constructor)
- description and source-code
```javascript
function Queue(size) {
  if (!(size >= 1)) throw new Error;
  this._size = size;
  this._call =
  this._error = null;
  this._tasks = [];
  this._data = [];
  this._waiting =
  this._active =
  this._ended =
  this._start = 0; // inside a synchronous task callback?
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.queue.prototype.defer"></a>[function <span class="apidocSignatureSpan">d3.queue.prototype.</span>defer (callback)](#apidoc.element.d3.queue.prototype.defer)
- description and source-code
```javascript
defer = function (callback) {
  if (typeof callback !== "function" || this._call) throw new Error;
  if (this._error != null) return this;
  var t = slice.call(arguments, 1);
  t.push(callback);
  ++this._waiting, this._tasks.push(t);
  poke(this);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.queue.prototype.constructor"></a>[module d3.queue.prototype.constructor](#apidoc.module.d3.queue.prototype.constructor)

#### <a name="apidoc.element.d3.queue.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.queue.prototype.</span>constructor ()](#apidoc.element.d3.queue.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.rgb"></a>[module d3.rgb](#apidoc.module.d3.rgb)

#### <a name="apidoc.element.d3.rgb.rgb"></a>[function <span class="apidocSignatureSpan">d3.</span>rgb (r, g, b, opacity)](#apidoc.element.d3.rgb.rgb)
- description and source-code
```javascript
function rgb(r, g, b, opacity) {
  return arguments.length === 1 ? rgbConvert(r) : new Rgb(r, g, b, opacity == null ? 1 : opacity);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.rgb.prototype"></a>[module d3.rgb.prototype](#apidoc.module.d3.rgb.prototype)

#### <a name="apidoc.element.d3.rgb.prototype.brighter"></a>[function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>brighter (k)](#apidoc.element.d3.rgb.prototype.brighter)
- description and source-code
```javascript
brighter = function (k) {
  k = k == null ? brighter : Math.pow(brighter, k);
  return new Rgb(this.r * k, this.g * k, this.b * k, this.opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.rgb.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>constructor (r, g, b, opacity)](#apidoc.element.d3.rgb.prototype.constructor)
- description and source-code
```javascript
function Rgb(r, g, b, opacity) {
  this.r = +r;
  this.g = +g;
  this.b = +b;
  this.opacity = +opacity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.rgb.prototype.darker"></a>[function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>darker (k)](#apidoc.element.d3.rgb.prototype.darker)
- description and source-code
```javascript
darker = function (k) {
  k = k == null ? darker : Math.pow(darker, k);
  return new Rgb(this.r * k, this.g * k, this.b * k, this.opacity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.rgb.prototype.displayable"></a>[function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>displayable ()](#apidoc.element.d3.rgb.prototype.displayable)
- description and source-code
```javascript
displayable = function () {
  return (0 <= this.r && this.r <= 255)
      && (0 <= this.g && this.g <= 255)
      && (0 <= this.b && this.b <= 255)
      && (0 <= this.opacity && this.opacity <= 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.rgb.prototype.rgb"></a>[function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>rgb ()](#apidoc.element.d3.rgb.prototype.rgb)
- description and source-code
```javascript
rgb = function () {
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.rgb.prototype.toString"></a>[function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>toString ()](#apidoc.element.d3.rgb.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var a = this.opacity; a = isNaN(a) ? 1 : Math.max(0, Math.min(1, a));
  return (a === 1 ? "rgb(" : "rgba(")
      + Math.max(0, Math.min(255, Math.round(this.r) || 0)) + ", "
      + Math.max(0, Math.min(255, Math.round(this.g) || 0)) + ", "
      + Math.max(0, Math.min(255, Math.round(this.b) || 0))
      + (a === 1 ? ")" : ", " + a + ")");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.rgb.prototype.constructor"></a>[module d3.rgb.prototype.constructor](#apidoc.module.d3.rgb.prototype.constructor)

#### <a name="apidoc.element.d3.rgb.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.rgb.prototype.</span>constructor ()](#apidoc.element.d3.rgb.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.selection"></a>[module d3.selection](#apidoc.module.d3.selection)

#### <a name="apidoc.element.d3.selection.selection"></a>[function <span class="apidocSignatureSpan">d3.</span>selection ()](#apidoc.element.d3.selection.selection)
- description and source-code
```javascript
function selection() {
  return new Selection([[document.documentElement]], root);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.selection.prototype"></a>[module d3.selection.prototype](#apidoc.module.d3.selection.prototype)

#### <a name="apidoc.element.d3.selection.prototype.append"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>append (name)](#apidoc.element.d3.selection.prototype.append)
- description and source-code
```javascript
append = function (name) {
  var create = typeof name === "function" ? name : creator(name);
  return this.select(function() {
    return this.appendChild(create.apply(this, arguments));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.attr"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>attr (name, value)](#apidoc.element.d3.selection.prototype.attr)
- description and source-code
```javascript
attr = function (name, value) {
  var fullname = namespace(name);

  if (arguments.length < 2) {
    var node = this.node();
    return fullname.local
        ? node.getAttributeNS(fullname.space, fullname.local)
        : node.getAttribute(fullname);
  }

  return this.each((value == null
      ? (fullname.local ? attrRemoveNS : attrRemove) : (typeof value === "function"
      ? (fullname.local ? attrFunctionNS : attrFunction)
      : (fullname.local ? attrConstantNS : attrConstant)))(fullname, value));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.call"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>call ()](#apidoc.element.d3.selection.prototype.call)
- description and source-code
```javascript
call = function () {
  var callback = arguments[0];
  arguments[0] = this;
  callback.apply(null, arguments);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.classed"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>classed (name, value)](#apidoc.element.d3.selection.prototype.classed)
- description and source-code
```javascript
classed = function (name, value) {
  var names = classArray(name + "");

  if (arguments.length < 2) {
    var list = classList(this.node()), i = -1, n = names.length;
    while (++i < n) if (!list.contains(names[i])) return false;
    return true;
  }

  return this.each((typeof value === "function"
      ? classedFunction : value
      ? classedTrue
      : classedFalse)(names, value));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>constructor (groups, parents)](#apidoc.element.d3.selection.prototype.constructor)
- description and source-code
```javascript
function Selection(groups, parents) {
  this._groups = groups;
  this._parents = parents;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.data"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>data (value, key)](#apidoc.element.d3.selection.prototype.data)
- description and source-code
```javascript
data = function (value, key) {
  if (!value) {
    data = new Array(this.size()), j = -1;
    this.each(function(d) { data[++j] = d; });
    return data;
  }

  var bind = key ? bindKey : bindIndex,
      parents = this._parents,
      groups = this._groups;

  if (typeof value !== "function") value = constant(value);

  for (var m = groups.length, update = new Array(m), enter = new Array(m), exit = new Array(m), j = 0; j < m; ++j) {
    var parent = parents[j],
        group = groups[j],
        groupLength = group.length,
        data = value.call(parent, parent && parent.__data__, j, parents),
        dataLength = data.length,
        enterGroup = enter[j] = new Array(dataLength),
        updateGroup = update[j] = new Array(dataLength),
        exitGroup = exit[j] = new Array(groupLength);

    bind(parent, group, enterGroup, updateGroup, exitGroup, data, key);

    // Now connect the enter nodes to their following update node, such that
    // appendChild can insert the materialized enter node before this node,
    // rather than at the end of the parent node.
    for (var i0 = 0, i1 = 0, previous, next; i0 < dataLength; ++i0) {
      if (previous = enterGroup[i0]) {
        if (i0 >= i1) i1 = i0 + 1;
        while (!(next = updateGroup[i1]) && ++i1 < dataLength);
        previous._next = next || null;
      }
    }
  }

  update = new Selection(update, parents);
  update._enter = enter;
  update._exit = exit;
  return update;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.datum"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>datum (value)](#apidoc.element.d3.selection.prototype.datum)
- description and source-code
```javascript
datum = function (value) {
  return arguments.length
      ? this.property("__data__", value)
      : this.node().__data__;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>dispatch (type, params)](#apidoc.element.d3.selection.prototype.dispatch)
- description and source-code
```javascript
dispatch = function (type, params) {
  return this.each((typeof params === "function"
      ? dispatchFunction
      : dispatchConstant)(type, params));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.each"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>each (callback)](#apidoc.element.d3.selection.prototype.each)
- description and source-code
```javascript
each = function (callback) {

  for (var groups = this._groups, j = 0, m = groups.length; j < m; ++j) {
    for (var group = groups[j], i = 0, n = group.length, node; i < n; ++i) {
      if (node = group[i]) callback.call(node, node.__data__, i, group);
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.empty"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>empty ()](#apidoc.element.d3.selection.prototype.empty)
- description and source-code
```javascript
empty = function () {
  return !this.node();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.enter"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>enter ()](#apidoc.element.d3.selection.prototype.enter)
- description and source-code
```javascript
enter = function () {
  return new Selection(this._enter || this._groups.map(sparse), this._parents);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.exit"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>exit ()](#apidoc.element.d3.selection.prototype.exit)
- description and source-code
```javascript
exit = function () {
  return new Selection(this._exit || this._groups.map(sparse), this._parents);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.filter"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>filter (match)](#apidoc.element.d3.selection.prototype.filter)
- description and source-code
```javascript
filter = function (match) {
  if (typeof match !== "function") match = matcher$1(match);

  for (var groups = this._groups, m = groups.length, subgroups = new Array(m), j = 0; j < m; ++j) {
    for (var group = groups[j], n = group.length, subgroup = subgroups[j] = [], node, i = 0; i < n; ++i) {
      if ((node = group[i]) && match.call(node, node.__data__, i, group)) {
        subgroup.push(node);
      }
    }
  }

  return new Selection(subgroups, this._parents);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.html"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>html (value)](#apidoc.element.d3.selection.prototype.html)
- description and source-code
```javascript
html = function (value) {
  return arguments.length
      ? this.each(value == null
          ? htmlRemove : (typeof value === "function"
          ? htmlFunction
          : htmlConstant)(value))
      : this.node().innerHTML;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.insert"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>insert (name, before)](#apidoc.element.d3.selection.prototype.insert)
- description and source-code
```javascript
insert = function (name, before) {
  var create = typeof name === "function" ? name : creator(name),
      select = before == null ? constantNull : typeof before === "function" ? before : selector(before);
  return this.select(function() {
    return this.insertBefore(create.apply(this, arguments), select.apply(this, arguments) || null);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.interrupt"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>interrupt (name)](#apidoc.element.d3.selection.prototype.interrupt)
- description and source-code
```javascript
interrupt = function (name) {
  return this.each(function() {
    interrupt(this, name);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.lower"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>lower ()](#apidoc.element.d3.selection.prototype.lower)
- description and source-code
```javascript
lower = function () {
  return this.each(lower);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.merge"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>merge (selection)](#apidoc.element.d3.selection.prototype.merge)
- description and source-code
```javascript
merge = function (selection) {

  for (var groups0 = this._groups, groups1 = selection._groups, m0 = groups0.length, m1 = groups1.length, m = Math.min(m0, m1),
merges = new Array(m0), j = 0; j < m; ++j) {
    for (var group0 = groups0[j], group1 = groups1[j], n = group0.length, merge = merges[j] = new Array(n), node, i = 0; i < n; ++
i) {
      if (node = group0[i] || group1[i]) {
        merge[i] = node;
      }
    }
  }

  for (; j < m0; ++j) {
    merges[j] = groups0[j];
  }

  return new Selection(merges, this._parents);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.node"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>node ()](#apidoc.element.d3.selection.prototype.node)
- description and source-code
```javascript
node = function () {

  for (var groups = this._groups, j = 0, m = groups.length; j < m; ++j) {
    for (var group = groups[j], i = 0, n = group.length; i < n; ++i) {
      var node = group[i];
      if (node) return node;
    }
  }

  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.nodes"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>nodes ()](#apidoc.element.d3.selection.prototype.nodes)
- description and source-code
```javascript
nodes = function () {
  var nodes = new Array(this.size()), i = -1;
  this.each(function() { nodes[++i] = this; });
  return nodes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.on"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>on (typename, value, capture)](#apidoc.element.d3.selection.prototype.on)
- description and source-code
```javascript
on = function (typename, value, capture) {
  var typenames = parseTypenames(typename + ""), i, n = typenames.length, t;

  if (arguments.length < 2) {
    var on = this.node().__on;
    if (on) for (var j = 0, m = on.length, o; j < m; ++j) {
      for (i = 0, o = on[j]; i < n; ++i) {
        if ((t = typenames[i]).type === o.type && t.name === o.name) {
          return o.value;
        }
      }
    }
    return;
  }

  on = value ? onAdd : onRemove;
  if (capture == null) capture = false;
  for (i = 0; i < n; ++i) this.each(on(typenames[i], value, capture));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.order"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>order ()](#apidoc.element.d3.selection.prototype.order)
- description and source-code
```javascript
order = function () {

  for (var groups = this._groups, j = -1, m = groups.length; ++j < m;) {
    for (var group = groups[j], i = group.length - 1, next = group[i], node; --i >= 0;) {
      if (node = group[i]) {
        if (next && next !== node.nextSibling) next.parentNode.insertBefore(node, next);
        next = node;
      }
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.property"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>property (name, value)](#apidoc.element.d3.selection.prototype.property)
- description and source-code
```javascript
property = function (name, value) {
  return arguments.length > 1
      ? this.each((value == null
          ? propertyRemove : typeof value === "function"
          ? propertyFunction
          : propertyConstant)(name, value))
      : this.node()[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.raise"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>raise ()](#apidoc.element.d3.selection.prototype.raise)
- description and source-code
```javascript
raise = function () {
  return this.each(raise);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.remove"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>remove ()](#apidoc.element.d3.selection.prototype.remove)
- description and source-code
```javascript
remove = function () {
  return this.each(remove);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.select"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>select (select)](#apidoc.element.d3.selection.prototype.select)
- description and source-code
```javascript
select = function (select) {
  if (typeof select !== "function") select = selector(select);

  for (var groups = this._groups, m = groups.length, subgroups = new Array(m), j = 0; j < m; ++j) {
    for (var group = groups[j], n = group.length, subgroup = subgroups[j] = new Array(n), node, subnode, i = 0; i < n; ++i) {
      if ((node = group[i]) && (subnode = select.call(node, node.__data__, i, group))) {
        if ("__data__" in node) subnode.__data__ = node.__data__;
        subgroup[i] = subnode;
      }
    }
  }

  return new Selection(subgroups, this._parents);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.selectAll"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>selectAll (select)](#apidoc.element.d3.selection.prototype.selectAll)
- description and source-code
```javascript
selectAll = function (select) {
  if (typeof select !== "function") select = selectorAll(select);

  for (var groups = this._groups, m = groups.length, subgroups = [], parents = [], j = 0; j < m; ++j) {
    for (var group = groups[j], n = group.length, node, i = 0; i < n; ++i) {
      if (node = group[i]) {
        subgroups.push(select.call(node, node.__data__, i, group));
        parents.push(node);
      }
    }
  }

  return new Selection(subgroups, parents);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.size"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>size ()](#apidoc.element.d3.selection.prototype.size)
- description and source-code
```javascript
size = function () {
  var size = 0;
  this.each(function() { ++size; });
  return size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.sort"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>sort (compare)](#apidoc.element.d3.selection.prototype.sort)
- description and source-code
```javascript
sort = function (compare) {
  if (!compare) compare = ascending;

  function compareNode(a, b) {
    return a && b ? compare(a.__data__, b.__data__) : !a - !b;
  }

  for (var groups = this._groups, m = groups.length, sortgroups = new Array(m), j = 0; j < m; ++j) {
    for (var group = groups[j], n = group.length, sortgroup = sortgroups[j] = new Array(n), node, i = 0; i < n; ++i) {
      if (node = group[i]) {
        sortgroup[i] = node;
      }
    }
    sortgroup.sort(compareNode);
  }

  return new Selection(sortgroups, this._parents).order();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.style"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>style (name, value, priority)](#apidoc.element.d3.selection.prototype.style)
- description and source-code
```javascript
style = function (name, value, priority) {
  var node;
  return arguments.length > 1
      ? this.each((value == null
            ? styleRemove : typeof value === "function"
            ? styleFunction
            : styleConstant)(name, value, priority == null ? "" : priority))
      : defaultView(node = this.node())
          .getComputedStyle(node, null)
          .getPropertyValue(name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.text"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>text (value)](#apidoc.element.d3.selection.prototype.text)
- description and source-code
```javascript
text = function (value) {
  return arguments.length
      ? this.each(value == null
          ? textRemove : (typeof value === "function"
          ? textFunction
          : textConstant)(value))
      : this.node().textContent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.selection.prototype.transition"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>transition (name)](#apidoc.element.d3.selection.prototype.transition)
- description and source-code
```javascript
transition = function (name) {
  var id,
      timing;

  if (name instanceof Transition) {
    id = name._id, name = name._name;
  } else {
    id = newId(), (timing = defaultTiming).time = d3Timer.now(), name = name == null ? null : name + "";
  }

  for (var groups = this._groups, m = groups.length, j = 0; j < m; ++j) {
    for (var group = groups[j], n = group.length, node, i = 0; i < n; ++i) {
      if (node = group[i]) {
        schedule(node, name, id, i, group, timing || inherit(node, id));
      }
    }
  }

  return new Transition(groups, this._parents, name, id);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.selection.prototype.constructor"></a>[module d3.selection.prototype.constructor](#apidoc.module.d3.selection.prototype.constructor)

#### <a name="apidoc.element.d3.selection.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.selection.prototype.</span>constructor ()](#apidoc.element.d3.selection.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.set"></a>[module d3.set](#apidoc.module.d3.set)

#### <a name="apidoc.element.d3.set.set"></a>[function <span class="apidocSignatureSpan">d3.</span>set (object, f)](#apidoc.element.d3.set.set)
- description and source-code
```javascript
function set(object, f) {
  var set = new Set;

  // Copy constructor.
  if (object instanceof Set) object.each(function(value) { set.add(value); });

  // Otherwise, assume it’s an array.
  else if (object) {
    var i = -1, n = object.length;
    if (f == null) while (++i < n) set.add(object[i]);
    else while (++i < n) set.add(f(object[i], i, object));
  }

  return set;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.set.prototype"></a>[module d3.set.prototype](#apidoc.module.d3.set.prototype)

#### <a name="apidoc.element.d3.set.prototype.add"></a>[function <span class="apidocSignatureSpan">d3.set.prototype.</span>add (value)](#apidoc.element.d3.set.prototype.add)
- description and source-code
```javascript
add = function (value) {
  value += "";
  this[prefix + value] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.set.prototype.clear"></a>[function <span class="apidocSignatureSpan">d3.set.prototype.</span>clear ()](#apidoc.element.d3.set.prototype.clear)
- description and source-code
```javascript
clear = function () {
  for (var property in this) if (property[0] === prefix) delete this[property];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.set.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.set.prototype.</span>constructor ()](#apidoc.element.d3.set.prototype.constructor)
- description and source-code
```javascript
function Set() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.set.prototype.each"></a>[function <span class="apidocSignatureSpan">d3.set.prototype.</span>each (f)](#apidoc.element.d3.set.prototype.each)
- description and source-code
```javascript
each = function (f) {
  for (var property in this) if (property[0] === prefix) f(this[property], property.slice(1), this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.set.prototype.empty"></a>[function <span class="apidocSignatureSpan">d3.set.prototype.</span>empty ()](#apidoc.element.d3.set.prototype.empty)
- description and source-code
```javascript
empty = function () {
  for (var property in this) if (property[0] === prefix) return false;
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.set.prototype.has"></a>[function <span class="apidocSignatureSpan">d3.set.prototype.</span>has (key)](#apidoc.element.d3.set.prototype.has)
- description and source-code
```javascript
has = function (key) {
  return (prefix + key) in this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.set.prototype.remove"></a>[function <span class="apidocSignatureSpan">d3.set.prototype.</span>remove (key)](#apidoc.element.d3.set.prototype.remove)
- description and source-code
```javascript
remove = function (key) {
  var property = prefix + key;
  return property in this && delete this[property];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.set.prototype.size"></a>[function <span class="apidocSignatureSpan">d3.set.prototype.</span>size ()](#apidoc.element.d3.set.prototype.size)
- description and source-code
```javascript
size = function () {
  var size = 0;
  for (var property in this) if (property[0] === prefix) ++size;
  return size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.set.prototype.values"></a>[function <span class="apidocSignatureSpan">d3.set.prototype.</span>values ()](#apidoc.element.d3.set.prototype.values)
- description and source-code
```javascript
values = function () {
  var keys = [];
  for (var property in this) if (property[0] === prefix) keys.push(property.slice(1));
  return keys;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.set.prototype.constructor"></a>[module d3.set.prototype.constructor](#apidoc.module.d3.set.prototype.constructor)

#### <a name="apidoc.element.d3.set.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.set.prototype.</span>constructor ()](#apidoc.element.d3.set.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.symbolCircle"></a>[module d3.symbolCircle](#apidoc.module.d3.symbolCircle)

#### <a name="apidoc.element.d3.symbolCircle.draw"></a>[function <span class="apidocSignatureSpan">d3.symbolCircle.</span>draw (context, size)](#apidoc.element.d3.symbolCircle.draw)
- description and source-code
```javascript
draw = function (context, size) {
  var r = Math.sqrt(size / pi);
  context.moveTo(r, 0);
  context.arc(0, 0, r, 0, tau);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.symbolCross"></a>[module d3.symbolCross](#apidoc.module.d3.symbolCross)

#### <a name="apidoc.element.d3.symbolCross.draw"></a>[function <span class="apidocSignatureSpan">d3.symbolCross.</span>draw (context, size)](#apidoc.element.d3.symbolCross.draw)
- description and source-code
```javascript
draw = function (context, size) {
  var r = Math.sqrt(size / 5) / 2;
  context.moveTo(-3 * r, -r);
  context.lineTo(-r, -r);
  context.lineTo(-r, -3 * r);
  context.lineTo(r, -3 * r);
  context.lineTo(r, -r);
  context.lineTo(3 * r, -r);
  context.lineTo(3 * r, r);
  context.lineTo(r, r);
  context.lineTo(r, 3 * r);
  context.lineTo(-r, 3 * r);
  context.lineTo(-r, r);
  context.lineTo(-3 * r, r);
  context.closePath();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.symbolDiamond"></a>[module d3.symbolDiamond](#apidoc.module.d3.symbolDiamond)

#### <a name="apidoc.element.d3.symbolDiamond.draw"></a>[function <span class="apidocSignatureSpan">d3.symbolDiamond.</span>draw (context, size)](#apidoc.element.d3.symbolDiamond.draw)
- description and source-code
```javascript
draw = function (context, size) {
  var y = Math.sqrt(size / tan30_2),
      x = y * tan30;
  context.moveTo(0, -y);
  context.lineTo(x, 0);
  context.lineTo(0, y);
  context.lineTo(-x, 0);
  context.closePath();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.symbolSquare"></a>[module d3.symbolSquare](#apidoc.module.d3.symbolSquare)

#### <a name="apidoc.element.d3.symbolSquare.draw"></a>[function <span class="apidocSignatureSpan">d3.symbolSquare.</span>draw (context, size)](#apidoc.element.d3.symbolSquare.draw)
- description and source-code
```javascript
draw = function (context, size) {
  var w = Math.sqrt(size),
      x = -w / 2;
  context.rect(x, x, w, w);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.symbolStar"></a>[module d3.symbolStar](#apidoc.module.d3.symbolStar)

#### <a name="apidoc.element.d3.symbolStar.draw"></a>[function <span class="apidocSignatureSpan">d3.symbolStar.</span>draw (context, size)](#apidoc.element.d3.symbolStar.draw)
- description and source-code
```javascript
draw = function (context, size) {
  var r = Math.sqrt(size * ka),
      x = kx * r,
      y = ky * r;
  context.moveTo(0, -r);
  context.lineTo(x, y);
  for (var i = 1; i < 5; ++i) {
    var a = tau * i / 5,
        c = Math.cos(a),
        s = Math.sin(a);
    context.lineTo(s * r, -c * r);
    context.lineTo(c * x - s * y, s * x + c * y);
  }
  context.closePath();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.symbolTriangle"></a>[module d3.symbolTriangle](#apidoc.module.d3.symbolTriangle)

#### <a name="apidoc.element.d3.symbolTriangle.draw"></a>[function <span class="apidocSignatureSpan">d3.symbolTriangle.</span>draw (context, size)](#apidoc.element.d3.symbolTriangle.draw)
- description and source-code
```javascript
draw = function (context, size) {
  var y = -Math.sqrt(size / (sqrt3 * 3));
  context.moveTo(0, y * 2);
  context.lineTo(-sqrt3 * y, -y);
  context.lineTo(sqrt3 * y, -y);
  context.closePath();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.symbolWye"></a>[module d3.symbolWye](#apidoc.module.d3.symbolWye)

#### <a name="apidoc.element.d3.symbolWye.draw"></a>[function <span class="apidocSignatureSpan">d3.symbolWye.</span>draw (context, size)](#apidoc.element.d3.symbolWye.draw)
- description and source-code
```javascript
draw = function (context, size) {
  var r = Math.sqrt(size / a),
      x0 = r / 2,
      y0 = r * k,
      x1 = x0,
      y1 = r * k + r,
      x2 = -x1,
      y2 = y1;
  context.moveTo(x0, y0);
  context.lineTo(x1, y1);
  context.lineTo(x2, y2);
  context.lineTo(c * x0 - s * y0, s * x0 + c * y0);
  context.lineTo(c * x1 - s * y1, s * x1 + c * y1);
  context.lineTo(c * x2 - s * y2, s * x2 + c * y2);
  context.lineTo(c * x0 + s * y0, c * y0 - s * x0);
  context.lineTo(c * x1 + s * y1, c * y1 - s * x1);
  context.lineTo(c * x2 + s * y2, c * y2 - s * x2);
  context.closePath();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeDay"></a>[module d3.timeDay](#apidoc.module.d3.timeDay)

#### <a name="apidoc.element.d3.timeDay.timeDay"></a>[function <span class="apidocSignatureSpan">d3.</span>timeDay (date)](#apidoc.element.d3.timeDay.timeDay)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeDay.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeDay.</span>ceil (date)](#apidoc.element.d3.timeDay.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeDay.count"></a>[function <span class="apidocSignatureSpan">d3.timeDay.</span>count (start, end)](#apidoc.element.d3.timeDay.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeDay.every"></a>[function <span class="apidocSignatureSpan">d3.timeDay.</span>every (step)](#apidoc.element.d3.timeDay.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeDay.filter"></a>[function <span class="apidocSignatureSpan">d3.timeDay.</span>filter (test)](#apidoc.element.d3.timeDay.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeDay.floor"></a>[function <span class="apidocSignatureSpan">d3.timeDay.</span>floor (date)](#apidoc.element.d3.timeDay.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeDay.offset"></a>[function <span class="apidocSignatureSpan">d3.timeDay.</span>offset (date, step)](#apidoc.element.d3.timeDay.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeDay.range"></a>[function <span class="apidocSignatureSpan">d3.timeDay.</span>range (start, stop, step)](#apidoc.element.d3.timeDay.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeDay.round"></a>[function <span class="apidocSignatureSpan">d3.timeDay.</span>round (date)](#apidoc.element.d3.timeDay.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeFriday"></a>[module d3.timeFriday](#apidoc.module.d3.timeFriday)

#### <a name="apidoc.element.d3.timeFriday.timeFriday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeFriday (date)](#apidoc.element.d3.timeFriday.timeFriday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFriday.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeFriday.</span>ceil (date)](#apidoc.element.d3.timeFriday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFriday.count"></a>[function <span class="apidocSignatureSpan">d3.timeFriday.</span>count (start, end)](#apidoc.element.d3.timeFriday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFriday.every"></a>[function <span class="apidocSignatureSpan">d3.timeFriday.</span>every (step)](#apidoc.element.d3.timeFriday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFriday.filter"></a>[function <span class="apidocSignatureSpan">d3.timeFriday.</span>filter (test)](#apidoc.element.d3.timeFriday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFriday.floor"></a>[function <span class="apidocSignatureSpan">d3.timeFriday.</span>floor (date)](#apidoc.element.d3.timeFriday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFriday.offset"></a>[function <span class="apidocSignatureSpan">d3.timeFriday.</span>offset (date, step)](#apidoc.element.d3.timeFriday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFriday.range"></a>[function <span class="apidocSignatureSpan">d3.timeFriday.</span>range (start, stop, step)](#apidoc.element.d3.timeFriday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeFriday.round"></a>[function <span class="apidocSignatureSpan">d3.timeFriday.</span>round (date)](#apidoc.element.d3.timeFriday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeHour"></a>[module d3.timeHour](#apidoc.module.d3.timeHour)

#### <a name="apidoc.element.d3.timeHour.timeHour"></a>[function <span class="apidocSignatureSpan">d3.</span>timeHour (date)](#apidoc.element.d3.timeHour.timeHour)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeHour.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeHour.</span>ceil (date)](#apidoc.element.d3.timeHour.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeHour.count"></a>[function <span class="apidocSignatureSpan">d3.timeHour.</span>count (start, end)](#apidoc.element.d3.timeHour.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeHour.every"></a>[function <span class="apidocSignatureSpan">d3.timeHour.</span>every (step)](#apidoc.element.d3.timeHour.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeHour.filter"></a>[function <span class="apidocSignatureSpan">d3.timeHour.</span>filter (test)](#apidoc.element.d3.timeHour.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeHour.floor"></a>[function <span class="apidocSignatureSpan">d3.timeHour.</span>floor (date)](#apidoc.element.d3.timeHour.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeHour.offset"></a>[function <span class="apidocSignatureSpan">d3.timeHour.</span>offset (date, step)](#apidoc.element.d3.timeHour.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeHour.range"></a>[function <span class="apidocSignatureSpan">d3.timeHour.</span>range (start, stop, step)](#apidoc.element.d3.timeHour.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeHour.round"></a>[function <span class="apidocSignatureSpan">d3.timeHour.</span>round (date)](#apidoc.element.d3.timeHour.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeMillisecond"></a>[module d3.timeMillisecond](#apidoc.module.d3.timeMillisecond)

#### <a name="apidoc.element.d3.timeMillisecond.timeMillisecond"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMillisecond (date)](#apidoc.element.d3.timeMillisecond.timeMillisecond)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMillisecond.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>ceil (date)](#apidoc.element.d3.timeMillisecond.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMillisecond.count"></a>[function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>count (start, end)](#apidoc.element.d3.timeMillisecond.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMillisecond.every"></a>[function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>every (k)](#apidoc.element.d3.timeMillisecond.every)
- description and source-code
```javascript
every = function (k) {
  k = Math.floor(k);
  if (!isFinite(k) || !(k > 0)) return null;
  if (!(k > 1)) return millisecond;
  return newInterval(function(date) {
    date.setTime(Math.floor(date / k) * k);
  }, function(date, step) {
    date.setTime(+date + step * k);
  }, function(start, end) {
    return (end - start) / k;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMillisecond.filter"></a>[function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>filter (test)](#apidoc.element.d3.timeMillisecond.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMillisecond.floor"></a>[function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>floor (date)](#apidoc.element.d3.timeMillisecond.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMillisecond.offset"></a>[function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>offset (date, step)](#apidoc.element.d3.timeMillisecond.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMillisecond.range"></a>[function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>range (start, stop, step)](#apidoc.element.d3.timeMillisecond.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMillisecond.round"></a>[function <span class="apidocSignatureSpan">d3.timeMillisecond.</span>round (date)](#apidoc.element.d3.timeMillisecond.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeMinute"></a>[module d3.timeMinute](#apidoc.module.d3.timeMinute)

#### <a name="apidoc.element.d3.timeMinute.timeMinute"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMinute (date)](#apidoc.element.d3.timeMinute.timeMinute)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMinute.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeMinute.</span>ceil (date)](#apidoc.element.d3.timeMinute.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMinute.count"></a>[function <span class="apidocSignatureSpan">d3.timeMinute.</span>count (start, end)](#apidoc.element.d3.timeMinute.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMinute.every"></a>[function <span class="apidocSignatureSpan">d3.timeMinute.</span>every (step)](#apidoc.element.d3.timeMinute.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMinute.filter"></a>[function <span class="apidocSignatureSpan">d3.timeMinute.</span>filter (test)](#apidoc.element.d3.timeMinute.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMinute.floor"></a>[function <span class="apidocSignatureSpan">d3.timeMinute.</span>floor (date)](#apidoc.element.d3.timeMinute.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMinute.offset"></a>[function <span class="apidocSignatureSpan">d3.timeMinute.</span>offset (date, step)](#apidoc.element.d3.timeMinute.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMinute.range"></a>[function <span class="apidocSignatureSpan">d3.timeMinute.</span>range (start, stop, step)](#apidoc.element.d3.timeMinute.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMinute.round"></a>[function <span class="apidocSignatureSpan">d3.timeMinute.</span>round (date)](#apidoc.element.d3.timeMinute.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeMonday"></a>[module d3.timeMonday](#apidoc.module.d3.timeMonday)

#### <a name="apidoc.element.d3.timeMonday.timeMonday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMonday (date)](#apidoc.element.d3.timeMonday.timeMonday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonday.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeMonday.</span>ceil (date)](#apidoc.element.d3.timeMonday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonday.count"></a>[function <span class="apidocSignatureSpan">d3.timeMonday.</span>count (start, end)](#apidoc.element.d3.timeMonday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonday.every"></a>[function <span class="apidocSignatureSpan">d3.timeMonday.</span>every (step)](#apidoc.element.d3.timeMonday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonday.filter"></a>[function <span class="apidocSignatureSpan">d3.timeMonday.</span>filter (test)](#apidoc.element.d3.timeMonday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonday.floor"></a>[function <span class="apidocSignatureSpan">d3.timeMonday.</span>floor (date)](#apidoc.element.d3.timeMonday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonday.offset"></a>[function <span class="apidocSignatureSpan">d3.timeMonday.</span>offset (date, step)](#apidoc.element.d3.timeMonday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonday.range"></a>[function <span class="apidocSignatureSpan">d3.timeMonday.</span>range (start, stop, step)](#apidoc.element.d3.timeMonday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonday.round"></a>[function <span class="apidocSignatureSpan">d3.timeMonday.</span>round (date)](#apidoc.element.d3.timeMonday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeMonth"></a>[module d3.timeMonth](#apidoc.module.d3.timeMonth)

#### <a name="apidoc.element.d3.timeMonth.timeMonth"></a>[function <span class="apidocSignatureSpan">d3.</span>timeMonth (date)](#apidoc.element.d3.timeMonth.timeMonth)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonth.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeMonth.</span>ceil (date)](#apidoc.element.d3.timeMonth.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonth.count"></a>[function <span class="apidocSignatureSpan">d3.timeMonth.</span>count (start, end)](#apidoc.element.d3.timeMonth.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonth.every"></a>[function <span class="apidocSignatureSpan">d3.timeMonth.</span>every (step)](#apidoc.element.d3.timeMonth.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonth.filter"></a>[function <span class="apidocSignatureSpan">d3.timeMonth.</span>filter (test)](#apidoc.element.d3.timeMonth.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonth.floor"></a>[function <span class="apidocSignatureSpan">d3.timeMonth.</span>floor (date)](#apidoc.element.d3.timeMonth.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonth.offset"></a>[function <span class="apidocSignatureSpan">d3.timeMonth.</span>offset (date, step)](#apidoc.element.d3.timeMonth.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonth.range"></a>[function <span class="apidocSignatureSpan">d3.timeMonth.</span>range (start, stop, step)](#apidoc.element.d3.timeMonth.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeMonth.round"></a>[function <span class="apidocSignatureSpan">d3.timeMonth.</span>round (date)](#apidoc.element.d3.timeMonth.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeSaturday"></a>[module d3.timeSaturday](#apidoc.module.d3.timeSaturday)

#### <a name="apidoc.element.d3.timeSaturday.timeSaturday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeSaturday (date)](#apidoc.element.d3.timeSaturday.timeSaturday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSaturday.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeSaturday.</span>ceil (date)](#apidoc.element.d3.timeSaturday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSaturday.count"></a>[function <span class="apidocSignatureSpan">d3.timeSaturday.</span>count (start, end)](#apidoc.element.d3.timeSaturday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSaturday.every"></a>[function <span class="apidocSignatureSpan">d3.timeSaturday.</span>every (step)](#apidoc.element.d3.timeSaturday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSaturday.filter"></a>[function <span class="apidocSignatureSpan">d3.timeSaturday.</span>filter (test)](#apidoc.element.d3.timeSaturday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSaturday.floor"></a>[function <span class="apidocSignatureSpan">d3.timeSaturday.</span>floor (date)](#apidoc.element.d3.timeSaturday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSaturday.offset"></a>[function <span class="apidocSignatureSpan">d3.timeSaturday.</span>offset (date, step)](#apidoc.element.d3.timeSaturday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSaturday.range"></a>[function <span class="apidocSignatureSpan">d3.timeSaturday.</span>range (start, stop, step)](#apidoc.element.d3.timeSaturday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSaturday.round"></a>[function <span class="apidocSignatureSpan">d3.timeSaturday.</span>round (date)](#apidoc.element.d3.timeSaturday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeSecond"></a>[module d3.timeSecond](#apidoc.module.d3.timeSecond)

#### <a name="apidoc.element.d3.timeSecond.timeSecond"></a>[function <span class="apidocSignatureSpan">d3.</span>timeSecond (date)](#apidoc.element.d3.timeSecond.timeSecond)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSecond.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeSecond.</span>ceil (date)](#apidoc.element.d3.timeSecond.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSecond.count"></a>[function <span class="apidocSignatureSpan">d3.timeSecond.</span>count (start, end)](#apidoc.element.d3.timeSecond.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSecond.every"></a>[function <span class="apidocSignatureSpan">d3.timeSecond.</span>every (step)](#apidoc.element.d3.timeSecond.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSecond.filter"></a>[function <span class="apidocSignatureSpan">d3.timeSecond.</span>filter (test)](#apidoc.element.d3.timeSecond.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSecond.floor"></a>[function <span class="apidocSignatureSpan">d3.timeSecond.</span>floor (date)](#apidoc.element.d3.timeSecond.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSecond.offset"></a>[function <span class="apidocSignatureSpan">d3.timeSecond.</span>offset (date, step)](#apidoc.element.d3.timeSecond.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSecond.range"></a>[function <span class="apidocSignatureSpan">d3.timeSecond.</span>range (start, stop, step)](#apidoc.element.d3.timeSecond.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeSecond.round"></a>[function <span class="apidocSignatureSpan">d3.timeSecond.</span>round (date)](#apidoc.element.d3.timeSecond.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeThursday"></a>[module d3.timeThursday](#apidoc.module.d3.timeThursday)

#### <a name="apidoc.element.d3.timeThursday.timeThursday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeThursday (date)](#apidoc.element.d3.timeThursday.timeThursday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeThursday.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeThursday.</span>ceil (date)](#apidoc.element.d3.timeThursday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeThursday.count"></a>[function <span class="apidocSignatureSpan">d3.timeThursday.</span>count (start, end)](#apidoc.element.d3.timeThursday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeThursday.every"></a>[function <span class="apidocSignatureSpan">d3.timeThursday.</span>every (step)](#apidoc.element.d3.timeThursday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeThursday.filter"></a>[function <span class="apidocSignatureSpan">d3.timeThursday.</span>filter (test)](#apidoc.element.d3.timeThursday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeThursday.floor"></a>[function <span class="apidocSignatureSpan">d3.timeThursday.</span>floor (date)](#apidoc.element.d3.timeThursday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeThursday.offset"></a>[function <span class="apidocSignatureSpan">d3.timeThursday.</span>offset (date, step)](#apidoc.element.d3.timeThursday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeThursday.range"></a>[function <span class="apidocSignatureSpan">d3.timeThursday.</span>range (start, stop, step)](#apidoc.element.d3.timeThursday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeThursday.round"></a>[function <span class="apidocSignatureSpan">d3.timeThursday.</span>round (date)](#apidoc.element.d3.timeThursday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeTuesday"></a>[module d3.timeTuesday](#apidoc.module.d3.timeTuesday)

#### <a name="apidoc.element.d3.timeTuesday.timeTuesday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeTuesday (date)](#apidoc.element.d3.timeTuesday.timeTuesday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeTuesday.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeTuesday.</span>ceil (date)](#apidoc.element.d3.timeTuesday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeTuesday.count"></a>[function <span class="apidocSignatureSpan">d3.timeTuesday.</span>count (start, end)](#apidoc.element.d3.timeTuesday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeTuesday.every"></a>[function <span class="apidocSignatureSpan">d3.timeTuesday.</span>every (step)](#apidoc.element.d3.timeTuesday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeTuesday.filter"></a>[function <span class="apidocSignatureSpan">d3.timeTuesday.</span>filter (test)](#apidoc.element.d3.timeTuesday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeTuesday.floor"></a>[function <span class="apidocSignatureSpan">d3.timeTuesday.</span>floor (date)](#apidoc.element.d3.timeTuesday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeTuesday.offset"></a>[function <span class="apidocSignatureSpan">d3.timeTuesday.</span>offset (date, step)](#apidoc.element.d3.timeTuesday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeTuesday.range"></a>[function <span class="apidocSignatureSpan">d3.timeTuesday.</span>range (start, stop, step)](#apidoc.element.d3.timeTuesday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeTuesday.round"></a>[function <span class="apidocSignatureSpan">d3.timeTuesday.</span>round (date)](#apidoc.element.d3.timeTuesday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeWednesday"></a>[module d3.timeWednesday](#apidoc.module.d3.timeWednesday)

#### <a name="apidoc.element.d3.timeWednesday.timeWednesday"></a>[function <span class="apidocSignatureSpan">d3.</span>timeWednesday (date)](#apidoc.element.d3.timeWednesday.timeWednesday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWednesday.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeWednesday.</span>ceil (date)](#apidoc.element.d3.timeWednesday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWednesday.count"></a>[function <span class="apidocSignatureSpan">d3.timeWednesday.</span>count (start, end)](#apidoc.element.d3.timeWednesday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWednesday.every"></a>[function <span class="apidocSignatureSpan">d3.timeWednesday.</span>every (step)](#apidoc.element.d3.timeWednesday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWednesday.filter"></a>[function <span class="apidocSignatureSpan">d3.timeWednesday.</span>filter (test)](#apidoc.element.d3.timeWednesday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWednesday.floor"></a>[function <span class="apidocSignatureSpan">d3.timeWednesday.</span>floor (date)](#apidoc.element.d3.timeWednesday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWednesday.offset"></a>[function <span class="apidocSignatureSpan">d3.timeWednesday.</span>offset (date, step)](#apidoc.element.d3.timeWednesday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWednesday.range"></a>[function <span class="apidocSignatureSpan">d3.timeWednesday.</span>range (start, stop, step)](#apidoc.element.d3.timeWednesday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWednesday.round"></a>[function <span class="apidocSignatureSpan">d3.timeWednesday.</span>round (date)](#apidoc.element.d3.timeWednesday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeWeek"></a>[module d3.timeWeek](#apidoc.module.d3.timeWeek)

#### <a name="apidoc.element.d3.timeWeek.timeWeek"></a>[function <span class="apidocSignatureSpan">d3.</span>timeWeek (date)](#apidoc.element.d3.timeWeek.timeWeek)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWeek.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeWeek.</span>ceil (date)](#apidoc.element.d3.timeWeek.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWeek.count"></a>[function <span class="apidocSignatureSpan">d3.timeWeek.</span>count (start, end)](#apidoc.element.d3.timeWeek.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWeek.every"></a>[function <span class="apidocSignatureSpan">d3.timeWeek.</span>every (step)](#apidoc.element.d3.timeWeek.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWeek.filter"></a>[function <span class="apidocSignatureSpan">d3.timeWeek.</span>filter (test)](#apidoc.element.d3.timeWeek.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWeek.floor"></a>[function <span class="apidocSignatureSpan">d3.timeWeek.</span>floor (date)](#apidoc.element.d3.timeWeek.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWeek.offset"></a>[function <span class="apidocSignatureSpan">d3.timeWeek.</span>offset (date, step)](#apidoc.element.d3.timeWeek.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWeek.range"></a>[function <span class="apidocSignatureSpan">d3.timeWeek.</span>range (start, stop, step)](#apidoc.element.d3.timeWeek.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeWeek.round"></a>[function <span class="apidocSignatureSpan">d3.timeWeek.</span>round (date)](#apidoc.element.d3.timeWeek.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timeYear"></a>[module d3.timeYear](#apidoc.module.d3.timeYear)

#### <a name="apidoc.element.d3.timeYear.timeYear"></a>[function <span class="apidocSignatureSpan">d3.</span>timeYear (date)](#apidoc.element.d3.timeYear.timeYear)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeYear.ceil"></a>[function <span class="apidocSignatureSpan">d3.timeYear.</span>ceil (date)](#apidoc.element.d3.timeYear.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeYear.count"></a>[function <span class="apidocSignatureSpan">d3.timeYear.</span>count (start, end)](#apidoc.element.d3.timeYear.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeYear.every"></a>[function <span class="apidocSignatureSpan">d3.timeYear.</span>every (k)](#apidoc.element.d3.timeYear.every)
- description and source-code
```javascript
every = function (k) {
  return !isFinite(k = Math.floor(k)) || !(k > 0) ? null : newInterval(function(date) {
    date.setFullYear(Math.floor(date.getFullYear() / k) * k);
    date.setMonth(0, 1);
    date.setHours(0, 0, 0, 0);
  }, function(date, step) {
    date.setFullYear(date.getFullYear() + step * k);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeYear.filter"></a>[function <span class="apidocSignatureSpan">d3.timeYear.</span>filter (test)](#apidoc.element.d3.timeYear.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeYear.floor"></a>[function <span class="apidocSignatureSpan">d3.timeYear.</span>floor (date)](#apidoc.element.d3.timeYear.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeYear.offset"></a>[function <span class="apidocSignatureSpan">d3.timeYear.</span>offset (date, step)](#apidoc.element.d3.timeYear.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeYear.range"></a>[function <span class="apidocSignatureSpan">d3.timeYear.</span>range (start, stop, step)](#apidoc.element.d3.timeYear.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timeYear.round"></a>[function <span class="apidocSignatureSpan">d3.timeYear.</span>round (date)](#apidoc.element.d3.timeYear.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timer"></a>[module d3.timer](#apidoc.module.d3.timer)

#### <a name="apidoc.element.d3.timer.timer"></a>[function <span class="apidocSignatureSpan">d3.</span>timer (callback, delay, time)](#apidoc.element.d3.timer.timer)
- description and source-code
```javascript
function timer(callback, delay, time) {
  var t = new Timer;
  t.restart(callback, delay, time);
  return t;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timer.prototype"></a>[module d3.timer.prototype](#apidoc.module.d3.timer.prototype)

#### <a name="apidoc.element.d3.timer.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.timer.prototype.</span>constructor ()](#apidoc.element.d3.timer.prototype.constructor)
- description and source-code
```javascript
function Timer() {
  this._call =
  this._time =
  this._next = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timer.prototype.restart"></a>[function <span class="apidocSignatureSpan">d3.timer.prototype.</span>restart (callback, delay, time)](#apidoc.element.d3.timer.prototype.restart)
- description and source-code
```javascript
restart = function (callback, delay, time) {
  if (typeof callback !== "function") throw new TypeError("callback is not a function");
  time = (time == null ? now() : +time) + (delay == null ? 0 : +delay);
  if (!this._next && taskTail !== this) {
    if (taskTail) taskTail._next = this;
    else taskHead = this;
    taskTail = this;
  }
  this._call = callback;
  this._time = time;
  sleep();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.timer.prototype.stop"></a>[function <span class="apidocSignatureSpan">d3.timer.prototype.</span>stop ()](#apidoc.element.d3.timer.prototype.stop)
- description and source-code
```javascript
stop = function () {
  if (this._call) {
    this._call = null;
    this._time = Infinity;
    sleep();
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.timer.prototype.constructor"></a>[module d3.timer.prototype.constructor](#apidoc.module.d3.timer.prototype.constructor)

#### <a name="apidoc.element.d3.timer.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.timer.prototype.</span>constructor ()](#apidoc.element.d3.timer.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.transition"></a>[module d3.transition](#apidoc.module.d3.transition)

#### <a name="apidoc.element.d3.transition.transition"></a>[function <span class="apidocSignatureSpan">d3.</span>transition (name)](#apidoc.element.d3.transition.transition)
- description and source-code
```javascript
function transition(name) {
  return d3Selection.selection().transition(name);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.transition.prototype"></a>[module d3.transition.prototype](#apidoc.module.d3.transition.prototype)

#### <a name="apidoc.element.d3.transition.prototype.attr"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>attr (name, value)](#apidoc.element.d3.transition.prototype.attr)
- description and source-code
```javascript
attr = function (name, value) {
  var fullname = d3Selection.namespace(name), i = fullname === "transform" ? d3Interpolate.interpolateTransformSvg : interpolate
;
  return this.attrTween(name, typeof value === "function"
      ? (fullname.local ? attrFunctionNS : attrFunction)(fullname, i, tweenValue(this, "attr." + name, value))
      : value == null ? (fullname.local ? attrRemoveNS : attrRemove)(fullname)
      : (fullname.local ? attrConstantNS : attrConstant)(fullname, i, value + ""));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.attrTween"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>attrTween (name, value)](#apidoc.element.d3.transition.prototype.attrTween)
- description and source-code
```javascript
attrTween = function (name, value) {
  var key = "attr." + name;
  if (arguments.length < 2) return (key = this.tween(key)) && key._value;
  if (value == null) return this.tween(key, null);
  if (typeof value !== "function") throw new Error;
  var fullname = d3Selection.namespace(name);
  return this.tween(key, (fullname.local ? attrTweenNS : attrTween)(fullname, value));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.call"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>call ()](#apidoc.element.d3.transition.prototype.call)
- description and source-code
```javascript
call = function () {
  var callback = arguments[0];
  arguments[0] = this;
  callback.apply(null, arguments);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>constructor (groups, parents, name, id)](#apidoc.element.d3.transition.prototype.constructor)
- description and source-code
```javascript
function Transition(groups, parents, name, id) {
  this._groups = groups;
  this._parents = parents;
  this._name = name;
  this._id = id;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.delay"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>delay (value)](#apidoc.element.d3.transition.prototype.delay)
- description and source-code
```javascript
delay = function (value) {
  var id = this._id;

  return arguments.length
      ? this.each((typeof value === "function"
          ? delayFunction
          : delayConstant)(id, value))
      : get(this.node(), id).delay;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.duration"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>duration (value)](#apidoc.element.d3.transition.prototype.duration)
- description and source-code
```javascript
duration = function (value) {
  var id = this._id;

  return arguments.length
      ? this.each((typeof value === "function"
          ? durationFunction
          : durationConstant)(id, value))
      : get(this.node(), id).duration;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.each"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>each (callback)](#apidoc.element.d3.transition.prototype.each)
- description and source-code
```javascript
each = function (callback) {

  for (var groups = this._groups, j = 0, m = groups.length; j < m; ++j) {
    for (var group = groups[j], i = 0, n = group.length, node; i < n; ++i) {
      if (node = group[i]) callback.call(node, node.__data__, i, group);
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.ease"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>ease (value)](#apidoc.element.d3.transition.prototype.ease)
- description and source-code
```javascript
ease = function (value) {
  var id = this._id;

  return arguments.length
      ? this.each(easeConstant(id, value))
      : get(this.node(), id).ease;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.empty"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>empty ()](#apidoc.element.d3.transition.prototype.empty)
- description and source-code
```javascript
empty = function () {
  return !this.node();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.filter"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>filter (match)](#apidoc.element.d3.transition.prototype.filter)
- description and source-code
```javascript
filter = function (match) {
  if (typeof match !== "function") match = d3Selection.matcher(match);

  for (var groups = this._groups, m = groups.length, subgroups = new Array(m), j = 0; j < m; ++j) {
    for (var group = groups[j], n = group.length, subgroup = subgroups[j] = [], node, i = 0; i < n; ++i) {
      if ((node = group[i]) && match.call(node, node.__data__, i, group)) {
        subgroup.push(node);
      }
    }
  }

  return new Transition(subgroups, this._parents, this._name, this._id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.merge"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>merge (transition)](#apidoc.element.d3.transition.prototype.merge)
- description and source-code
```javascript
merge = function (transition) {
  if (transition._id !== this._id) throw new Error;

  for (var groups0 = this._groups, groups1 = transition._groups, m0 = groups0.length, m1 = groups1.length, m = Math.min(m0, m1),
merges = new Array(m0), j = 0; j < m; ++j) {
    for (var group0 = groups0[j], group1 = groups1[j], n = group0.length, merge = merges[j] = new Array(n), node, i = 0; i < n; ++
i) {
      if (node = group0[i] || group1[i]) {
        merge[i] = node;
      }
    }
  }

  for (; j < m0; ++j) {
    merges[j] = groups0[j];
  }

  return new Transition(merges, this._parents, this._name, this._id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.node"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>node ()](#apidoc.element.d3.transition.prototype.node)
- description and source-code
```javascript
node = function () {

  for (var groups = this._groups, j = 0, m = groups.length; j < m; ++j) {
    for (var group = groups[j], i = 0, n = group.length; i < n; ++i) {
      var node = group[i];
      if (node) return node;
    }
  }

  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.nodes"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>nodes ()](#apidoc.element.d3.transition.prototype.nodes)
- description and source-code
```javascript
nodes = function () {
  var nodes = new Array(this.size()), i = -1;
  this.each(function() { nodes[++i] = this; });
  return nodes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.on"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>on (name, listener)](#apidoc.element.d3.transition.prototype.on)
- description and source-code
```javascript
on = function (name, listener) {
  var id = this._id;

  return arguments.length < 2
      ? get(this.node(), id).on.on(name)
      : this.each(onFunction(id, name, listener));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.remove"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>remove ()](#apidoc.element.d3.transition.prototype.remove)
- description and source-code
```javascript
remove = function () {
  return this.on("end.remove", removeFunction(this._id));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.select"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>select (select)](#apidoc.element.d3.transition.prototype.select)
- description and source-code
```javascript
select = function (select) {
  var name = this._name,
      id = this._id;

  if (typeof select !== "function") select = d3Selection.selector(select);

  for (var groups = this._groups, m = groups.length, subgroups = new Array(m), j = 0; j < m; ++j) {
    for (var group = groups[j], n = group.length, subgroup = subgroups[j] = new Array(n), node, subnode, i = 0; i < n; ++i) {
      if ((node = group[i]) && (subnode = select.call(node, node.__data__, i, group))) {
        if ("__data__" in node) subnode.__data__ = node.__data__;
        subgroup[i] = subnode;
        schedule(subgroup[i], name, id, i, subgroup, get(node, id));
      }
    }
  }

  return new Transition(subgroups, this._parents, name, id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.selectAll"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>selectAll (select)](#apidoc.element.d3.transition.prototype.selectAll)
- description and source-code
```javascript
selectAll = function (select) {
  var name = this._name,
      id = this._id;

  if (typeof select !== "function") select = d3Selection.selectorAll(select);

  for (var groups = this._groups, m = groups.length, subgroups = [], parents = [], j = 0; j < m; ++j) {
    for (var group = groups[j], n = group.length, node, i = 0; i < n; ++i) {
      if (node = group[i]) {
        for (var children = select.call(node, node.__data__, i, group), child, inherit = get(node, id), k = 0, l = children.length
; k < l; ++k) {
          if (child = children[k]) {
            schedule(child, name, id, k, children, inherit);
          }
        }
        subgroups.push(children);
        parents.push(node);
      }
    }
  }

  return new Transition(subgroups, parents, name, id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.selection"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>selection ()](#apidoc.element.d3.transition.prototype.selection)
- description and source-code
```javascript
selection = function () {
  return new Selection(this._groups, this._parents);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.size"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>size ()](#apidoc.element.d3.transition.prototype.size)
- description and source-code
```javascript
size = function () {
  var size = 0;
  this.each(function() { ++size; });
  return size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.style"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>style (name, value, priority)](#apidoc.element.d3.transition.prototype.style)
- description and source-code
```javascript
style = function (name, value, priority) {
  var i = (name += "") === "transform" ? d3Interpolate.interpolateTransformCss : interpolate;
  return value == null ? this
          .styleTween(name, styleRemove(name, i))
          .on("end.style." + name, styleRemoveEnd(name))
      : this.styleTween(name, typeof value === "function"
          ? styleFunction(name, i, tweenValue(this, "style." + name, value))
          : styleConstant(name, i, value + ""), priority);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.styleTween"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>styleTween (name, value, priority)](#apidoc.element.d3.transition.prototype.styleTween)
- description and source-code
```javascript
styleTween = function (name, value, priority) {
  var key = "style." + (name += "");
  if (arguments.length < 2) return (key = this.tween(key)) && key._value;
  if (value == null) return this.tween(key, null);
  if (typeof value !== "function") throw new Error;
  return this.tween(key, styleTween(name, value, priority == null ? "" : priority));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.text"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>text (value)](#apidoc.element.d3.transition.prototype.text)
- description and source-code
```javascript
text = function (value) {
  return this.tween("text", typeof value === "function"
      ? textFunction(tweenValue(this, "text", value))
      : textConstant(value == null ? "" : value + ""));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.transition"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>transition ()](#apidoc.element.d3.transition.prototype.transition)
- description and source-code
```javascript
transition = function () {
  var name = this._name,
      id0 = this._id,
      id1 = newId();

  for (var groups = this._groups, m = groups.length, j = 0; j < m; ++j) {
    for (var group = groups[j], n = group.length, node, i = 0; i < n; ++i) {
      if (node = group[i]) {
        var inherit = get(node, id0);
        schedule(node, name, id1, i, group, {
          time: inherit.time + inherit.delay + inherit.duration,
          delay: 0,
          duration: inherit.duration,
          ease: inherit.ease
        });
      }
    }
  }

  return new Transition(groups, this._parents, name, id1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.transition.prototype.tween"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>tween (name, value)](#apidoc.element.d3.transition.prototype.tween)
- description and source-code
```javascript
tween = function (name, value) {
  var id = this._id;

  name += "";

  if (arguments.length < 2) {
    var tween = get(this.node(), id).tween;
    for (var i = 0, n = tween.length, t; i < n; ++i) {
      if ((t = tween[i]).name === name) {
        return t.value;
      }
    }
    return null;
  }

  return this.each((value == null ? tweenRemove : tweenFunction)(id, name, value));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.transition.prototype.constructor"></a>[module d3.transition.prototype.constructor](#apidoc.module.d3.transition.prototype.constructor)

#### <a name="apidoc.element.d3.transition.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.transition.prototype.</span>constructor ()](#apidoc.element.d3.transition.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.treemapResquarify"></a>[module d3.treemapResquarify](#apidoc.module.d3.treemapResquarify)

#### <a name="apidoc.element.d3.treemapResquarify.treemapResquarify"></a>[function <span class="apidocSignatureSpan">d3.</span>treemapResquarify (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapResquarify.treemapResquarify)
- description and source-code
```javascript
function resquarify(parent, x0, y0, x1, y1) {
  if ((rows = parent._squarify) && (rows.ratio === ratio)) {
    var rows,
        row,
        nodes,
        i,
        j = -1,
        n,
        m = rows.length,
        value = parent.value;

    while (++j < m) {
      row = rows[j], nodes = row.children;
      for (i = row.value = 0, n = nodes.length; i < n; ++i) row.value += nodes[i].value;
      if (row.dice) treemapDice(row, x0, y0, x1, y0 += (y1 - y0) * row.value / value);
      else treemapSlice(row, x0, y0, x0 += (x1 - x0) * row.value / value, y1);
      value -= row.value;
    }
  } else {
    parent._squarify = rows = squarifyRatio(ratio, parent, x0, y0, x1, y1);
    rows.ratio = ratio;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.treemapResquarify.ratio"></a>[function <span class="apidocSignatureSpan">d3.treemapResquarify.</span>ratio (x)](#apidoc.element.d3.treemapResquarify.ratio)
- description and source-code
```javascript
ratio = function (x) {
  return custom((x = +x) > 1 ? x : 1);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.treemapSquarify"></a>[module d3.treemapSquarify](#apidoc.module.d3.treemapSquarify)

#### <a name="apidoc.element.d3.treemapSquarify.treemapSquarify"></a>[function <span class="apidocSignatureSpan">d3.</span>treemapSquarify (parent, x0, y0, x1, y1)](#apidoc.element.d3.treemapSquarify.treemapSquarify)
- description and source-code
```javascript
function squarify(parent, x0, y0, x1, y1) {
  squarifyRatio(ratio, parent, x0, y0, x1, y1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.treemapSquarify.ratio"></a>[function <span class="apidocSignatureSpan">d3.treemapSquarify.</span>ratio (x)](#apidoc.element.d3.treemapSquarify.ratio)
- description and source-code
```javascript
ratio = function (x) {
  return custom((x = +x) > 1 ? x : 1);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcDay"></a>[module d3.utcDay](#apidoc.module.d3.utcDay)

#### <a name="apidoc.element.d3.utcDay.utcDay"></a>[function <span class="apidocSignatureSpan">d3.</span>utcDay (date)](#apidoc.element.d3.utcDay.utcDay)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcDay.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcDay.</span>ceil (date)](#apidoc.element.d3.utcDay.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcDay.count"></a>[function <span class="apidocSignatureSpan">d3.utcDay.</span>count (start, end)](#apidoc.element.d3.utcDay.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcDay.every"></a>[function <span class="apidocSignatureSpan">d3.utcDay.</span>every (step)](#apidoc.element.d3.utcDay.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcDay.filter"></a>[function <span class="apidocSignatureSpan">d3.utcDay.</span>filter (test)](#apidoc.element.d3.utcDay.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcDay.floor"></a>[function <span class="apidocSignatureSpan">d3.utcDay.</span>floor (date)](#apidoc.element.d3.utcDay.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcDay.offset"></a>[function <span class="apidocSignatureSpan">d3.utcDay.</span>offset (date, step)](#apidoc.element.d3.utcDay.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcDay.range"></a>[function <span class="apidocSignatureSpan">d3.utcDay.</span>range (start, stop, step)](#apidoc.element.d3.utcDay.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcDay.round"></a>[function <span class="apidocSignatureSpan">d3.utcDay.</span>round (date)](#apidoc.element.d3.utcDay.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcFriday"></a>[module d3.utcFriday](#apidoc.module.d3.utcFriday)

#### <a name="apidoc.element.d3.utcFriday.utcFriday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcFriday (date)](#apidoc.element.d3.utcFriday.utcFriday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFriday.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcFriday.</span>ceil (date)](#apidoc.element.d3.utcFriday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFriday.count"></a>[function <span class="apidocSignatureSpan">d3.utcFriday.</span>count (start, end)](#apidoc.element.d3.utcFriday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFriday.every"></a>[function <span class="apidocSignatureSpan">d3.utcFriday.</span>every (step)](#apidoc.element.d3.utcFriday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFriday.filter"></a>[function <span class="apidocSignatureSpan">d3.utcFriday.</span>filter (test)](#apidoc.element.d3.utcFriday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFriday.floor"></a>[function <span class="apidocSignatureSpan">d3.utcFriday.</span>floor (date)](#apidoc.element.d3.utcFriday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFriday.offset"></a>[function <span class="apidocSignatureSpan">d3.utcFriday.</span>offset (date, step)](#apidoc.element.d3.utcFriday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFriday.range"></a>[function <span class="apidocSignatureSpan">d3.utcFriday.</span>range (start, stop, step)](#apidoc.element.d3.utcFriday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcFriday.round"></a>[function <span class="apidocSignatureSpan">d3.utcFriday.</span>round (date)](#apidoc.element.d3.utcFriday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcHour"></a>[module d3.utcHour](#apidoc.module.d3.utcHour)

#### <a name="apidoc.element.d3.utcHour.utcHour"></a>[function <span class="apidocSignatureSpan">d3.</span>utcHour (date)](#apidoc.element.d3.utcHour.utcHour)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcHour.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcHour.</span>ceil (date)](#apidoc.element.d3.utcHour.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcHour.count"></a>[function <span class="apidocSignatureSpan">d3.utcHour.</span>count (start, end)](#apidoc.element.d3.utcHour.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcHour.every"></a>[function <span class="apidocSignatureSpan">d3.utcHour.</span>every (step)](#apidoc.element.d3.utcHour.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcHour.filter"></a>[function <span class="apidocSignatureSpan">d3.utcHour.</span>filter (test)](#apidoc.element.d3.utcHour.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcHour.floor"></a>[function <span class="apidocSignatureSpan">d3.utcHour.</span>floor (date)](#apidoc.element.d3.utcHour.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcHour.offset"></a>[function <span class="apidocSignatureSpan">d3.utcHour.</span>offset (date, step)](#apidoc.element.d3.utcHour.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcHour.range"></a>[function <span class="apidocSignatureSpan">d3.utcHour.</span>range (start, stop, step)](#apidoc.element.d3.utcHour.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcHour.round"></a>[function <span class="apidocSignatureSpan">d3.utcHour.</span>round (date)](#apidoc.element.d3.utcHour.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcMinute"></a>[module d3.utcMinute](#apidoc.module.d3.utcMinute)

#### <a name="apidoc.element.d3.utcMinute.utcMinute"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMinute (date)](#apidoc.element.d3.utcMinute.utcMinute)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMinute.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcMinute.</span>ceil (date)](#apidoc.element.d3.utcMinute.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMinute.count"></a>[function <span class="apidocSignatureSpan">d3.utcMinute.</span>count (start, end)](#apidoc.element.d3.utcMinute.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMinute.every"></a>[function <span class="apidocSignatureSpan">d3.utcMinute.</span>every (step)](#apidoc.element.d3.utcMinute.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMinute.filter"></a>[function <span class="apidocSignatureSpan">d3.utcMinute.</span>filter (test)](#apidoc.element.d3.utcMinute.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMinute.floor"></a>[function <span class="apidocSignatureSpan">d3.utcMinute.</span>floor (date)](#apidoc.element.d3.utcMinute.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMinute.offset"></a>[function <span class="apidocSignatureSpan">d3.utcMinute.</span>offset (date, step)](#apidoc.element.d3.utcMinute.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMinute.range"></a>[function <span class="apidocSignatureSpan">d3.utcMinute.</span>range (start, stop, step)](#apidoc.element.d3.utcMinute.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMinute.round"></a>[function <span class="apidocSignatureSpan">d3.utcMinute.</span>round (date)](#apidoc.element.d3.utcMinute.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcMonday"></a>[module d3.utcMonday](#apidoc.module.d3.utcMonday)

#### <a name="apidoc.element.d3.utcMonday.utcMonday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMonday (date)](#apidoc.element.d3.utcMonday.utcMonday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonday.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcMonday.</span>ceil (date)](#apidoc.element.d3.utcMonday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonday.count"></a>[function <span class="apidocSignatureSpan">d3.utcMonday.</span>count (start, end)](#apidoc.element.d3.utcMonday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonday.every"></a>[function <span class="apidocSignatureSpan">d3.utcMonday.</span>every (step)](#apidoc.element.d3.utcMonday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonday.filter"></a>[function <span class="apidocSignatureSpan">d3.utcMonday.</span>filter (test)](#apidoc.element.d3.utcMonday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonday.floor"></a>[function <span class="apidocSignatureSpan">d3.utcMonday.</span>floor (date)](#apidoc.element.d3.utcMonday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonday.offset"></a>[function <span class="apidocSignatureSpan">d3.utcMonday.</span>offset (date, step)](#apidoc.element.d3.utcMonday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonday.range"></a>[function <span class="apidocSignatureSpan">d3.utcMonday.</span>range (start, stop, step)](#apidoc.element.d3.utcMonday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonday.round"></a>[function <span class="apidocSignatureSpan">d3.utcMonday.</span>round (date)](#apidoc.element.d3.utcMonday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcMonth"></a>[module d3.utcMonth](#apidoc.module.d3.utcMonth)

#### <a name="apidoc.element.d3.utcMonth.utcMonth"></a>[function <span class="apidocSignatureSpan">d3.</span>utcMonth (date)](#apidoc.element.d3.utcMonth.utcMonth)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonth.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcMonth.</span>ceil (date)](#apidoc.element.d3.utcMonth.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonth.count"></a>[function <span class="apidocSignatureSpan">d3.utcMonth.</span>count (start, end)](#apidoc.element.d3.utcMonth.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonth.every"></a>[function <span class="apidocSignatureSpan">d3.utcMonth.</span>every (step)](#apidoc.element.d3.utcMonth.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonth.filter"></a>[function <span class="apidocSignatureSpan">d3.utcMonth.</span>filter (test)](#apidoc.element.d3.utcMonth.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonth.floor"></a>[function <span class="apidocSignatureSpan">d3.utcMonth.</span>floor (date)](#apidoc.element.d3.utcMonth.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonth.offset"></a>[function <span class="apidocSignatureSpan">d3.utcMonth.</span>offset (date, step)](#apidoc.element.d3.utcMonth.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonth.range"></a>[function <span class="apidocSignatureSpan">d3.utcMonth.</span>range (start, stop, step)](#apidoc.element.d3.utcMonth.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcMonth.round"></a>[function <span class="apidocSignatureSpan">d3.utcMonth.</span>round (date)](#apidoc.element.d3.utcMonth.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcSaturday"></a>[module d3.utcSaturday](#apidoc.module.d3.utcSaturday)

#### <a name="apidoc.element.d3.utcSaturday.utcSaturday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcSaturday (date)](#apidoc.element.d3.utcSaturday.utcSaturday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSaturday.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcSaturday.</span>ceil (date)](#apidoc.element.d3.utcSaturday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSaturday.count"></a>[function <span class="apidocSignatureSpan">d3.utcSaturday.</span>count (start, end)](#apidoc.element.d3.utcSaturday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSaturday.every"></a>[function <span class="apidocSignatureSpan">d3.utcSaturday.</span>every (step)](#apidoc.element.d3.utcSaturday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSaturday.filter"></a>[function <span class="apidocSignatureSpan">d3.utcSaturday.</span>filter (test)](#apidoc.element.d3.utcSaturday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSaturday.floor"></a>[function <span class="apidocSignatureSpan">d3.utcSaturday.</span>floor (date)](#apidoc.element.d3.utcSaturday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSaturday.offset"></a>[function <span class="apidocSignatureSpan">d3.utcSaturday.</span>offset (date, step)](#apidoc.element.d3.utcSaturday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSaturday.range"></a>[function <span class="apidocSignatureSpan">d3.utcSaturday.</span>range (start, stop, step)](#apidoc.element.d3.utcSaturday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcSaturday.round"></a>[function <span class="apidocSignatureSpan">d3.utcSaturday.</span>round (date)](#apidoc.element.d3.utcSaturday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcThursday"></a>[module d3.utcThursday](#apidoc.module.d3.utcThursday)

#### <a name="apidoc.element.d3.utcThursday.utcThursday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcThursday (date)](#apidoc.element.d3.utcThursday.utcThursday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcThursday.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcThursday.</span>ceil (date)](#apidoc.element.d3.utcThursday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcThursday.count"></a>[function <span class="apidocSignatureSpan">d3.utcThursday.</span>count (start, end)](#apidoc.element.d3.utcThursday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcThursday.every"></a>[function <span class="apidocSignatureSpan">d3.utcThursday.</span>every (step)](#apidoc.element.d3.utcThursday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcThursday.filter"></a>[function <span class="apidocSignatureSpan">d3.utcThursday.</span>filter (test)](#apidoc.element.d3.utcThursday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcThursday.floor"></a>[function <span class="apidocSignatureSpan">d3.utcThursday.</span>floor (date)](#apidoc.element.d3.utcThursday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcThursday.offset"></a>[function <span class="apidocSignatureSpan">d3.utcThursday.</span>offset (date, step)](#apidoc.element.d3.utcThursday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcThursday.range"></a>[function <span class="apidocSignatureSpan">d3.utcThursday.</span>range (start, stop, step)](#apidoc.element.d3.utcThursday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcThursday.round"></a>[function <span class="apidocSignatureSpan">d3.utcThursday.</span>round (date)](#apidoc.element.d3.utcThursday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcTuesday"></a>[module d3.utcTuesday](#apidoc.module.d3.utcTuesday)

#### <a name="apidoc.element.d3.utcTuesday.utcTuesday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcTuesday (date)](#apidoc.element.d3.utcTuesday.utcTuesday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcTuesday.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcTuesday.</span>ceil (date)](#apidoc.element.d3.utcTuesday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcTuesday.count"></a>[function <span class="apidocSignatureSpan">d3.utcTuesday.</span>count (start, end)](#apidoc.element.d3.utcTuesday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcTuesday.every"></a>[function <span class="apidocSignatureSpan">d3.utcTuesday.</span>every (step)](#apidoc.element.d3.utcTuesday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcTuesday.filter"></a>[function <span class="apidocSignatureSpan">d3.utcTuesday.</span>filter (test)](#apidoc.element.d3.utcTuesday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcTuesday.floor"></a>[function <span class="apidocSignatureSpan">d3.utcTuesday.</span>floor (date)](#apidoc.element.d3.utcTuesday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcTuesday.offset"></a>[function <span class="apidocSignatureSpan">d3.utcTuesday.</span>offset (date, step)](#apidoc.element.d3.utcTuesday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcTuesday.range"></a>[function <span class="apidocSignatureSpan">d3.utcTuesday.</span>range (start, stop, step)](#apidoc.element.d3.utcTuesday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcTuesday.round"></a>[function <span class="apidocSignatureSpan">d3.utcTuesday.</span>round (date)](#apidoc.element.d3.utcTuesday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcWednesday"></a>[module d3.utcWednesday](#apidoc.module.d3.utcWednesday)

#### <a name="apidoc.element.d3.utcWednesday.utcWednesday"></a>[function <span class="apidocSignatureSpan">d3.</span>utcWednesday (date)](#apidoc.element.d3.utcWednesday.utcWednesday)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWednesday.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcWednesday.</span>ceil (date)](#apidoc.element.d3.utcWednesday.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWednesday.count"></a>[function <span class="apidocSignatureSpan">d3.utcWednesday.</span>count (start, end)](#apidoc.element.d3.utcWednesday.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWednesday.every"></a>[function <span class="apidocSignatureSpan">d3.utcWednesday.</span>every (step)](#apidoc.element.d3.utcWednesday.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWednesday.filter"></a>[function <span class="apidocSignatureSpan">d3.utcWednesday.</span>filter (test)](#apidoc.element.d3.utcWednesday.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWednesday.floor"></a>[function <span class="apidocSignatureSpan">d3.utcWednesday.</span>floor (date)](#apidoc.element.d3.utcWednesday.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWednesday.offset"></a>[function <span class="apidocSignatureSpan">d3.utcWednesday.</span>offset (date, step)](#apidoc.element.d3.utcWednesday.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWednesday.range"></a>[function <span class="apidocSignatureSpan">d3.utcWednesday.</span>range (start, stop, step)](#apidoc.element.d3.utcWednesday.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWednesday.round"></a>[function <span class="apidocSignatureSpan">d3.utcWednesday.</span>round (date)](#apidoc.element.d3.utcWednesday.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcWeek"></a>[module d3.utcWeek](#apidoc.module.d3.utcWeek)

#### <a name="apidoc.element.d3.utcWeek.utcWeek"></a>[function <span class="apidocSignatureSpan">d3.</span>utcWeek (date)](#apidoc.element.d3.utcWeek.utcWeek)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWeek.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcWeek.</span>ceil (date)](#apidoc.element.d3.utcWeek.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWeek.count"></a>[function <span class="apidocSignatureSpan">d3.utcWeek.</span>count (start, end)](#apidoc.element.d3.utcWeek.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWeek.every"></a>[function <span class="apidocSignatureSpan">d3.utcWeek.</span>every (step)](#apidoc.element.d3.utcWeek.every)
- description and source-code
```javascript
every = function (step) {
  step = Math.floor(step);
  return !isFinite(step) || !(step > 0) ? null
      : !(step > 1) ? interval
      : interval.filter(field
          ? function(d) { return field(d) % step === 0; }
          : function(d) { return interval.count(0, d) % step === 0; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWeek.filter"></a>[function <span class="apidocSignatureSpan">d3.utcWeek.</span>filter (test)](#apidoc.element.d3.utcWeek.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWeek.floor"></a>[function <span class="apidocSignatureSpan">d3.utcWeek.</span>floor (date)](#apidoc.element.d3.utcWeek.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWeek.offset"></a>[function <span class="apidocSignatureSpan">d3.utcWeek.</span>offset (date, step)](#apidoc.element.d3.utcWeek.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWeek.range"></a>[function <span class="apidocSignatureSpan">d3.utcWeek.</span>range (start, stop, step)](#apidoc.element.d3.utcWeek.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcWeek.round"></a>[function <span class="apidocSignatureSpan">d3.utcWeek.</span>round (date)](#apidoc.element.d3.utcWeek.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.utcYear"></a>[module d3.utcYear](#apidoc.module.d3.utcYear)

#### <a name="apidoc.element.d3.utcYear.utcYear"></a>[function <span class="apidocSignatureSpan">d3.</span>utcYear (date)](#apidoc.element.d3.utcYear.utcYear)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcYear.ceil"></a>[function <span class="apidocSignatureSpan">d3.utcYear.</span>ceil (date)](#apidoc.element.d3.utcYear.ceil)
- description and source-code
```javascript
ceil = function (date) {
  return floori(date = new Date(date - 1)), offseti(date, 1), floori(date), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcYear.count"></a>[function <span class="apidocSignatureSpan">d3.utcYear.</span>count (start, end)](#apidoc.element.d3.utcYear.count)
- description and source-code
```javascript
count = function (start, end) {
  t0.setTime(+start), t1.setTime(+end);
  floori(t0), floori(t1);
  return Math.floor(count(t0, t1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcYear.every"></a>[function <span class="apidocSignatureSpan">d3.utcYear.</span>every (k)](#apidoc.element.d3.utcYear.every)
- description and source-code
```javascript
every = function (k) {
  return !isFinite(k = Math.floor(k)) || !(k > 0) ? null : newInterval(function(date) {
    date.setUTCFullYear(Math.floor(date.getUTCFullYear() / k) * k);
    date.setUTCMonth(0, 1);
    date.setUTCHours(0, 0, 0, 0);
  }, function(date, step) {
    date.setUTCFullYear(date.getUTCFullYear() + step * k);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcYear.filter"></a>[function <span class="apidocSignatureSpan">d3.utcYear.</span>filter (test)](#apidoc.element.d3.utcYear.filter)
- description and source-code
```javascript
filter = function (test) {
  return newInterval(function(date) {
    if (date >= date) while (floori(date), !test(date)) date.setTime(date - 1);
  }, function(date, step) {
    if (date >= date) while (--step >= 0) while (offseti(date, 1), !test(date)) {} // eslint-disable-line no-empty
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcYear.floor"></a>[function <span class="apidocSignatureSpan">d3.utcYear.</span>floor (date)](#apidoc.element.d3.utcYear.floor)
- description and source-code
```javascript
function interval(date) {
  return floori(date = new Date(+date)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcYear.offset"></a>[function <span class="apidocSignatureSpan">d3.utcYear.</span>offset (date, step)](#apidoc.element.d3.utcYear.offset)
- description and source-code
```javascript
offset = function (date, step) {
  return offseti(date = new Date(+date), step == null ? 1 : Math.floor(step)), date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcYear.range"></a>[function <span class="apidocSignatureSpan">d3.utcYear.</span>range (start, stop, step)](#apidoc.element.d3.utcYear.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  var range = [];
  start = interval.ceil(start);
  step = step == null ? 1 : Math.floor(step);
  if (!(start < stop) || !(step > 0)) return range; // also handles Invalid Date
  do range.push(new Date(+start)); while (offseti(start, step), floori(start), start < stop)
  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.utcYear.round"></a>[function <span class="apidocSignatureSpan">d3.utcYear.</span>round (date)](#apidoc.element.d3.utcYear.round)
- description and source-code
```javascript
round = function (date) {
  var d0 = interval(date),
      d1 = interval.ceil(date);
  return date - d0 < d1 - date ? d0 : d1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.zoomTransform"></a>[module d3.zoomTransform](#apidoc.module.d3.zoomTransform)

#### <a name="apidoc.element.d3.zoomTransform.zoomTransform"></a>[function <span class="apidocSignatureSpan">d3.</span>zoomTransform (node)](#apidoc.element.d3.zoomTransform.zoomTransform)
- description and source-code
```javascript
function transform(node) {
  return node.__zoom || identity;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.zoomTransform.prototype"></a>[module d3.zoomTransform.prototype](#apidoc.module.d3.zoomTransform.prototype)

#### <a name="apidoc.element.d3.zoomTransform.prototype.apply"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>apply (point)](#apidoc.element.d3.zoomTransform.prototype.apply)
- description and source-code
```javascript
apply = function (point) {
  return [point[0] * this.k + this.x, point[1] * this.k + this.y];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.applyX"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>applyX (x)](#apidoc.element.d3.zoomTransform.prototype.applyX)
- description and source-code
```javascript
applyX = function (x) {
  return x * this.k + this.x;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.applyY"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>applyY (y)](#apidoc.element.d3.zoomTransform.prototype.applyY)
- description and source-code
```javascript
applyY = function (y) {
  return y * this.k + this.y;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.constructor"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>constructor (k, x, y)](#apidoc.element.d3.zoomTransform.prototype.constructor)
- description and source-code
```javascript
function Transform(k, x, y) {
  this.k = k;
  this.x = x;
  this.y = y;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.invert"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>invert (location)](#apidoc.element.d3.zoomTransform.prototype.invert)
- description and source-code
```javascript
invert = function (location) {
  return [(location[0] - this.x) / this.k, (location[1] - this.y) / this.k];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.invertX"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>invertX (x)](#apidoc.element.d3.zoomTransform.prototype.invertX)
- description and source-code
```javascript
invertX = function (x) {
  return (x - this.x) / this.k;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.invertY"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>invertY (y)](#apidoc.element.d3.zoomTransform.prototype.invertY)
- description and source-code
```javascript
invertY = function (y) {
  return (y - this.y) / this.k;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.rescaleX"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>rescaleX (x)](#apidoc.element.d3.zoomTransform.prototype.rescaleX)
- description and source-code
```javascript
rescaleX = function (x) {
  return x.copy().domain(x.range().map(this.invertX, this).map(x.invert, x));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.rescaleY"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>rescaleY (y)](#apidoc.element.d3.zoomTransform.prototype.rescaleY)
- description and source-code
```javascript
rescaleY = function (y) {
  return y.copy().domain(y.range().map(this.invertY, this).map(y.invert, y));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.scale"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>scale (k)](#apidoc.element.d3.zoomTransform.prototype.scale)
- description and source-code
```javascript
scale = function (k) {
  return k === 1 ? this : new Transform(this.k * k, this.x, this.y);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.toString"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>toString ()](#apidoc.element.d3.zoomTransform.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return "translate(" + this.x + "," + this.y + ") scale(" + this.k + ")";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.d3.zoomTransform.prototype.translate"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>translate (x, y)](#apidoc.element.d3.zoomTransform.prototype.translate)
- description and source-code
```javascript
translate = function (x, y) {
  return x === 0 & y === 0 ? this : new Transform(this.k, this.x + this.k * x, this.y + this.k * y);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.d3.zoomTransform.prototype.constructor"></a>[module d3.zoomTransform.prototype.constructor](#apidoc.module.d3.zoomTransform.prototype.constructor)

#### <a name="apidoc.element.d3.zoomTransform.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">d3.zoomTransform.prototype.</span>constructor ()](#apidoc.element.d3.zoomTransform.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
