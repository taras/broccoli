# master

* In addition to `Brocfile.js`, accept lowercase `brocfile.js`

# 0.2.0

* Rename `Broccolifile.js` to `Brocfile.js`
* Change default port from 8000 to 4200

# 0.1.1

* Make `tree.cleanup` non-optional
* Rename `broccoli.read` to `broccoli.makeTree`

# 0.1.0

* Bump to indicate beta status
* Remove unused `helpers.walkSync` (now in node-walk-sync)

# 0.0.13

* Extract `Transformer` into `broccoli-transform` package (now "`Transform`")
* Extract `Filter` into `broccoli-filter` package

# 0.0.12

* In plugin (tree) API, replace `.afterBuild` with `.cleanup`
* Move temporary directories out of the way

# 0.0.11

* Extract `factory.env` into broccoli-env package
* Eliminate `factory` argument to Broccolifile

# 0.0.10

* Change to a `.read`-based everything-is-a-tree architecture
* Various performance improvements
* Various plugin API changes
* Add `MergedTree`
* Broccolifile may now return an array of trees, which will be merged
* Expose `broccoli.bowerTrees()`, which will hopefully be redesigned and go
  away again
* Remove `Component` base class
* Remove `CompilerCollection` and `Compiler` base class; use a `Transformer`
* Remove `Tree::addTransform`, `Tree::addTrees`, and `Tree::addBower`
* `Builder::build` now has a promise interface as well

# 0.0.9

* Expect a `Tree`, not a `Builder`, returned from Broccolifile.js

# 0.0.8

* Fold `Reader` into `Tree`
* Replace `PreprocessorPipeline` and `Preprocessor` with `Filter`; each
  `Filter` is added directly on the tree or builder with `addTransform`

# 0.0.7

* Bind to `0.0.0.0` instead of `localhost`
* Add `factory.env` based on `$BROCCOLI_ENV`
* Do not fail on invalid Cookie header
* Use promises instead of callbacks in all external APIs

# 0.0.6

* Here be dragons
