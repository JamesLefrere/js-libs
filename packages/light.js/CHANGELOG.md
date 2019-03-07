# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [5.0.1](https://github.com/paritytech/js-libs/tree/master/packages/light.js/compare/v5.0.0...v5.0.1) (2019-03-07)

**Note:** Version bump only for package @parity/light.js





# [5.0.0](https://github.com/paritytech/js-libs/tree/master/packages/light.js/compare/v4.1.1...v5.0.0) (2019-03-05)


### Code Refactoring

* Remove RPC_LOADING/withoutLoading ([#200](https://github.com/paritytech/js-libs/tree/master/packages/light.js/issues/200)) ([ae9ea03](https://github.com/paritytech/js-libs/tree/master/packages/light.js/commit/ae9ea03))


### BREAKING CHANGES

* Observables do not emit the symbol RPC_LOADING anymore. They will
only emit once a value is available. The operator withoutLoading
has been removed as this is now the default behaviour.

* refactor: Remove RPC_LOADING/withoutLoading

* Fix error

switchMapPromise source and output can differ (number => BigNumber)





## [4.1.1](https://github.com/paritytech/js-libs/tree/master/packages/light.js/compare/v4.1.0...v4.1.1) (2019-03-05)

**Note:** Version bump only for package @parity/light.js





# [4.1.0](https://github.com/paritytech/js-libs/tree/master/packages/light.js/compare/v4.0.3...v4.1.0) (2019-03-05)


### Features

* createRpc & createPubSub: defer getApi & delay unsubscription ([#197](https://github.com/paritytech/js-libs/tree/master/packages/light.js/issues/197)) ([191f1d2](https://github.com/paritytech/js-libs/tree/master/packages/light.js/commit/191f1d2))
* fix build errored in [#197](https://github.com/paritytech/js-libs/tree/master/packages/light.js/issues/197) ([#201](https://github.com/paritytech/js-libs/tree/master/packages/light.js/issues/201)) ([1e0790d](https://github.com/paritytech/js-libs/tree/master/packages/light.js/commit/1e0790d))





## [4.0.3](https://github.com/paritytech/js-libs/tree/master/packages/light.js/compare/v4.0.2...v4.0.3) (2019-02-04)

**Note:** Version bump only for package @parity/light.js





## [4.0.2](https://github.com/paritytech/js-libs/tree/master/packages/light.js/compare/v4.0.1...v4.0.2) (2019-01-22)

**Note:** Version bump only for package @parity/light.js





## [4.0.1](https://github.com/paritytech/js-libs/tree/master/packages/light.js/compare/v4.0.0...v4.0.1) (2019-01-22)

**Note:** Version bump only for package @parity/light.js





# [4.0.0](https://github.com/paritytech/js-libs/tree/master/packages/light.js/compare/v3.0.31...v4.0.0) (2019-01-22)


### Code Refactoring

* Rewrite post$ to take a password and not use signer ([689ae52](https://github.com/paritytech/js-libs/tree/master/packages/light.js/commit/689ae52))


### BREAKING CHANGES

* `post$` now requires `passphrase` in its options.

Non-constant contract method calls from `makeContract` now require `passphrase` in their options.

`post$` now returns `{estimated}?` `{signed}` `{sent}` `{confirmed}` and postRaw$ now returns `{sent}` `{confirmed}`