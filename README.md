# npmdoc-yarn

#### basic api documentation for  [yarn (v0.22.0)](https://github.com/yarnpkg/yarn#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-yarn.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-yarn) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-yarn.svg)](https://travis-ci.org/npmdoc/node-npmdoc-yarn)

#### 📦🐈 Fast, reliable, and secure dependency management.

[![NPM](https://nodei.co/npm/yarn.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/yarn)

- [https://npmdoc.github.io/node-npmdoc-yarn/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-yarn/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-yarn/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-yarn/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-yarn/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-yarn/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bin": {
        "yarn": "./bin/yarn.js",
        "yarnpkg": "./bin/yarn.js"
    },
    "bugs": {
        "url": "https://github.com/yarnpkg/yarn/issues"
    },
    "dependencies": {
        "babel-runtime": "^6.0.0",
        "bytes": "^2.4.0",
        "camelcase": "^4.0.0",
        "chalk": "^1.1.1",
        "cmd-shim": "^2.0.1",
        "commander": "^2.9.0",
        "death": "^1.0.0",
        "debug": "^2.2.0",
        "detect-indent": "^5.0.0",
        "ini": "^1.3.4",
        "inquirer": "^3.0.1",
        "invariant": "^2.2.0",
        "is-builtin-module": "^1.0.0",
        "is-ci": "^1.0.10",
        "leven": "^2.0.0",
        "loud-rejection": "^1.2.0",
        "minimatch": "^3.0.3",
        "mkdirp": "^0.5.1",
        "node-emoji": "^1.0.4",
        "node-gyp": "^3.2.1",
        "object-path": "^0.11.2",
        "proper-lockfile": "^2.0.0",
        "read": "^1.0.7",
        "request": "^2.75.0",
        "request-capture-har": "^1.1.4",
        "rimraf": "^2.5.0",
        "roadrunner": "^1.1.0",
        "semver": "^5.1.0",
        "strip-bom": "^3.0.0",
        "tar": "^2.2.1",
        "tar-stream": "^1.5.2",
        "v8-compile-cache": "^1.0.0",
        "validate-npm-package-license": "^3.0.1"
    },
    "deprecated": "It is recommended to install Yarn using the native installation method for your environment. See https://yarnpkg.com/en/docs/install",
    "description": "📦🐈 Fast, reliable, and secure dependency management.",
    "devDependencies": {
        "babel-core": "^6.17.0",
        "babel-eslint": "^6.1.2",
        "babel-jest": "^19.0.0",
        "babel-loader": "^6.2.5",
        "babel-plugin-transform-es2015-typeof-symbol": "^6.8.0",
        "babel-plugin-transform-inline-imports-commonjs": "^1.0.0",
        "babel-plugin-transform-runtime": "^6.4.3",
        "babel-preset-es2015-node4": "^2.1.0",
        "babel-preset-node5": "^10.2.0",
        "babel-preset-stage-0": "^6.0.0",
        "babylon": "^6.5.0",
        "eslint": "^3.3.1",
        "eslint-config-fb-strict": "^14.1.3",
        "eslint-config-fbjs": "^1.0.0",
        "eslint-plugin-babel": "^3.3.0",
        "eslint-plugin-flowtype": "^2.15.0",
        "eslint-plugin-no-async-without-await": "^1.0.0",
        "eslint-plugin-react": "5.2.2",
        "eslint-plugin-yarn-internal": "file:scripts/eslint-rules",
        "flow-bin": "^0.40.0",
        "gulp": "^3.9.0",
        "gulp-babel": "^6.0.0",
        "gulp-if": "^2.0.1",
        "gulp-newer": "^1.0.0",
        "gulp-plumber": "^1.0.1",
        "gulp-sourcemaps": "^2.2.0",
        "gulp-util": "^3.0.7",
        "gulp-watch": "^4.3.5",
        "jest": "^19.0.2",
        "mock-stdin": "^0.3.0",
        "temp": "^0.8.3",
        "webpack": "^2.1.0-beta.25",
        "yargs": "^6.3.0"
    },
    "directories": {},
    "dist": {
        "shasum": "fd8511dc29225b925be967dc185772cc59de5888",
        "tarball": "https://registry.npmjs.org/yarn/-/yarn-0.22.0.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "homepage": "https://github.com/yarnpkg/yarn#readme",
    "installationMethod": "npm",
    "jest": {
        "timers": "fake",
        "testEnvironment": "node",
        "modulePathIgnorePatterns": [
            "__tests__/fixtures/"
        ],
        "testPathIgnorePatterns": [
            "__tests__/(fixtures|__mocks__)/",
            "updates/",
            "/_(temp|mock|install|init|helpers).js$"
        ]
    },
    "license": "BSD-2-Clause",
    "maintainers": [
        {
            "name": "daniel15"
        }
    ],
    "name": "yarn",
    "optionalDependencies": {},
    "preferGlobal": true,
    "repository": {
        "type": "git",
        "url": "git+https://github.com/yarnpkg/yarn.git"
    },
    "scripts": {
        "build": "gulp build",
        "build-chocolatey": "powershell ./scripts/build-chocolatey.ps1",
        "build-dist": "./scripts/build-dist.sh",
        "build-win-installer": "scripts\\build-windows-installer.bat",
        "check-lockfile": "./scripts/check-lockfile.sh",
        "lint": "eslint . && flow check",
        "release-branch": "./scripts/release-branch.sh",
        "test": "npm run lint && npm run test-only",
        "test-ci": "npm run build && npm run test-only",
        "test-only": "jest --coverage --verbose",
        "watch": "gulp watch"
    },
    "version": "0.22.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
