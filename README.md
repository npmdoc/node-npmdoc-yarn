# api documentation for  [yarn (v0.21.3)](https://github.com/yarnpkg/yarn#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-yarn.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-yarn) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-yarn.svg)](https://travis-ci.org/npmdoc/node-npmdoc-yarn)
#### 📦🐈 Fast, reliable, and secure dependency management.

[![NPM](https://nodei.co/npm/yarn.png?downloads=true)](https://www.npmjs.com/package/yarn)

[![apidoc](https://npmdoc.github.io/node-npmdoc-yarn/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-yarn_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-yarn/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-yarn/build/screen-capture.npmPackageListing.svg)



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
        "camelcase": "^3.0.0",
        "chalk": "^1.1.1",
        "cmd-shim": "^2.0.1",
        "commander": "^2.9.0",
        "death": "^1.0.0",
        "debug": "^2.2.0",
        "defaults": "^1.0.3",
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
        "validate-npm-package-license": "^3.0.1"
    },
    "description": "📦🐈 Fast, reliable, and secure dependency management.",
    "devDependencies": {
        "babel-core": "^6.17.0",
        "babel-eslint": "^6.1.2",
        "babel-jest": "^14.0.0",
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
        "flow-bin": "^0.37.3",
        "gulp": "^3.9.0",
        "gulp-babel": "^6.0.0",
        "gulp-if": "^2.0.1",
        "gulp-newer": "^1.0.0",
        "gulp-plumber": "^1.0.1",
        "gulp-sourcemaps": "^2.2.0",
        "gulp-util": "^3.0.7",
        "gulp-watch": "^4.3.5",
        "jest": "^16.0.1",
        "mock-stdin": "^0.3.0",
        "temp": "^0.8.3",
        "webpack": "^2.1.0-beta.25",
        "yargs": "^6.3.0"
    },
    "directories": {},
    "dist": {
        "shasum": "8dda3a63c798b383cfa577452c2b3cb3e4aa87e0",
        "tarball": "https://registry.npmjs.org/yarn/-/yarn-0.21.3.tgz"
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
            "name": "daniel15",
            "email": "npm@dan.cx"
        }
    ],
    "name": "yarn",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
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
    "version": "0.21.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module yarn](#apidoc.module.yarn)
1.  object <span class="apidocSignatureSpan">yarn.</span>config
1.  object <span class="apidocSignatureSpan">yarn.</span>constants
1.  object <span class="apidocSignatureSpan">yarn.</span>errors
1.  object <span class="apidocSignatureSpan">yarn.</span>package_compatibility
1.  object <span class="apidocSignatureSpan">yarn.</span>package_constraint_resolver
1.  object <span class="apidocSignatureSpan">yarn.</span>package_fetcher
1.  object <span class="apidocSignatureSpan">yarn.</span>package_hoister
1.  object <span class="apidocSignatureSpan">yarn.</span>package_install_scripts
1.  object <span class="apidocSignatureSpan">yarn.</span>package_linker
1.  object <span class="apidocSignatureSpan">yarn.</span>package_reference
1.  object <span class="apidocSignatureSpan">yarn.</span>package_request
1.  object <span class="apidocSignatureSpan">yarn.</span>package_resolver

#### [module yarn.config](#apidoc.module.yarn.config)
1.  [function <span class="apidocSignatureSpan">yarn.config.</span>default (reporter)](#apidoc.element.yarn.config.default)

#### [module yarn.constants](#apidoc.module.yarn.constants)
1.  boolean <span class="apidocSignatureSpan">yarn.constants.</span>ROOT_USER
1.  [function <span class="apidocSignatureSpan">yarn.constants.</span>getPathKey (platform, env)](#apidoc.element.yarn.constants.getPathKey)
1.  [function <span class="apidocSignatureSpan">yarn.constants.</span>isRootUser (uid)](#apidoc.element.yarn.constants.isRootUser)
1.  number <span class="apidocSignatureSpan">yarn.constants.</span>CHILD_CONCURRENCY
1.  number <span class="apidocSignatureSpan">yarn.constants.</span>LOCKFILE_VERSION
1.  number <span class="apidocSignatureSpan">yarn.constants.</span>NETWORK_CONCURRENCY
1.  number <span class="apidocSignatureSpan">yarn.constants.</span>SINGLE_INSTANCE_PORT
1.  object <span class="apidocSignatureSpan">yarn.constants.</span>DEPENDENCY_TYPES
1.  object <span class="apidocSignatureSpan">yarn.constants.</span>REQUIRED_PACKAGE_KEYS
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>CACHE_FILENAME
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>CLEAN_FILENAME
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>CONFIG_DIRECTORY
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>DEFAULT_INDENT
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>ENV_PATH_KEY
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>GLOBAL_MODULE_DIRECTORY
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>INTEGRITY_FILENAME
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>LINK_REGISTRY_DIRECTORY
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>LOCKFILE_FILENAME
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>METADATA_FILENAME
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>MODULE_CACHE_DIRECTORY
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>SELF_UPDATE_DOWNLOAD_FOLDER
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>SELF_UPDATE_TARBALL_URL
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>SELF_UPDATE_VERSION_URL
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>SINGLE_INSTANCE_FILENAME
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>TARBALL_FILENAME
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>YARN_DOCS
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>YARN_INSTALLER_MSI
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>YARN_INSTALLER_SH
1.  string <span class="apidocSignatureSpan">yarn.constants.</span>YARN_REGISTRY

#### [module yarn.errors](#apidoc.module.yarn.errors)
1.  [function <span class="apidocSignatureSpan">yarn.errors.</span>MessageError (msg, code)](#apidoc.element.yarn.errors.MessageError)
1.  [function <span class="apidocSignatureSpan">yarn.errors.</span>SecurityError {{signature}}](#apidoc.element.yarn.errors.SecurityError)
1.  [function <span class="apidocSignatureSpan">yarn.errors.</span>SpawnError {{signature}}](#apidoc.element.yarn.errors.SpawnError)

#### [module yarn.package_compatibility](#apidoc.module.yarn.package_compatibility)
1.  [function <span class="apidocSignatureSpan">yarn.package_compatibility.</span>default (config, resolver, ignoreEngines)](#apidoc.element.yarn.package_compatibility.default)
1.  [function <span class="apidocSignatureSpan">yarn.package_compatibility.</span>testEngine (name, range, versions, looseSemver)](#apidoc.element.yarn.package_compatibility.testEngine)

#### [module yarn.package_constraint_resolver](#apidoc.module.yarn.package_constraint_resolver)
1.  [function <span class="apidocSignatureSpan">yarn.package_constraint_resolver.</span>default (config, reporter)](#apidoc.element.yarn.package_constraint_resolver.default)

#### [module yarn.package_fetcher](#apidoc.module.yarn.package_fetcher)
1.  [function <span class="apidocSignatureSpan">yarn.package_fetcher.</span>default (config, resolver)](#apidoc.element.yarn.package_fetcher.default)

#### [module yarn.package_hoister](#apidoc.module.yarn.package_hoister)
1.  [function <span class="apidocSignatureSpan">yarn.package_hoister.</span>HoistManifest (key, parts, pkg, loc, isIgnored, inheritIsIgnored)](#apidoc.element.yarn.package_hoister.HoistManifest)
1.  [function <span class="apidocSignatureSpan">yarn.package_hoister.</span>default (config, resolver)](#apidoc.element.yarn.package_hoister.default)

#### [module yarn.package_install_scripts](#apidoc.module.yarn.package_install_scripts)
1.  [function <span class="apidocSignatureSpan">yarn.package_install_scripts.</span>default (config, resolver, force)](#apidoc.element.yarn.package_install_scripts.default)

#### [module yarn.package_linker](#apidoc.module.yarn.package_linker)
1.  [function <span class="apidocSignatureSpan">yarn.package_linker.</span>default (config, resolver)](#apidoc.element.yarn.package_linker.default)
1.  [function <span class="apidocSignatureSpan">yarn.package_linker.</span>linkBin (_x, _x2)](#apidoc.element.yarn.package_linker.linkBin)

#### [module yarn.package_reference](#apidoc.module.yarn.package_reference)
1.  [function <span class="apidocSignatureSpan">yarn.package_reference.</span>default (request, info, remote)](#apidoc.element.yarn.package_reference.default)

#### [module yarn.package_request](#apidoc.module.yarn.package_request)
1.  [function <span class="apidocSignatureSpan">yarn.package_request.</span>default (req, resolver)](#apidoc.element.yarn.package_request.default)

#### [module yarn.package_resolver](#apidoc.module.yarn.package_resolver)
1.  [function <span class="apidocSignatureSpan">yarn.package_resolver.</span>default (config, lockfile)](#apidoc.element.yarn.package_resolver.default)



# <a name="apidoc.module.yarn"></a>[module yarn](#apidoc.module.yarn)



# <a name="apidoc.module.yarn.config"></a>[module yarn.config](#apidoc.module.yarn.config)

#### <a name="apidoc.element.yarn.config.default"></a>[function <span class="apidocSignatureSpan">yarn.config.</span>default (reporter)](#apidoc.element.yarn.config.default)
- description and source-code
```javascript
class Config {
  constructor(reporter) {
    this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
    this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
    this.reporter = reporter;
    this._init({});
  }

  //


  //


  //


  //


  //


  //


  //


  //


  //


  //


  //


  // Whether we should ignore executing lifecycle scripts


  //


  //


  //


  //


<span class="apidocCodeCommentSpan">  /**
   * Execute a promise produced by factory if it doesn't exist in our cache with
   * the associated key.
   */
</span>
  getCache(key, factory) {
    const cached = this.cache[key];
    if (cached) {
      return cached;
    }

    return this.cache[key] = factory().catch(err => {
      this.cache[key] = null;
      throw err;
    });
  }

  /**
   * Get a config option from our yarn config.
   */

  getOption(key) {
    return this.registries.yarn.getOption(key);
  }

  /**
   * Reduce a list of versions to a single one based on an input range.
   */

  resolveConstraints(versions, range) {
    return this.constraintResolver.reduce(versions, range);
  }

  /**
   * Initialise config. Fetch registry options, find package roots.
   */

  init() {
    var _this = this;

    let opts = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : {};
    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      _this._init(opts);

      yield (_fs || _load_fs()).mkdirp(_this.globalFolder);
      yield (_fs || _load_fs()).mkdirp(_this.linkFolder);

      _this.linkedModules = [];

      const linkedModules = yield (_fs || _load_fs()).readdir(_this.linkFolder);

      for (const dir of linkedModules) {
        const linkedPath = path.join(_this.linkFolder, dir);

        if (dir[0] === '@') {
          // it's a scope, not a package
          const scopedLinked = yield (_fs || _load_fs()).readdir(linkedPath);
          _this.linkedModules.push(...scopedLinked.map(function (scopedDir) {
            return path.join(dir, scopedDir);
          }));
        } else {
          _this.linkedModules.push(dir);
        }
      }

      for (const key of Object.keys((_index2 || _load_index2()).registries)) {
        const Registry = (_index2 || _load_index2()).registries[key];

        // instantiate registry
        const registry = new Registry(_this.cwd, _this.registries, _this.requestManager);
        yield registry.init();

        _this.registries[key] = registry;
        _this.registryFolders.push(registry.folder);
        const rootModuleFolder = path.join(_this.cwd, registry.folder);
        if (_this.rootModuleFolders.indexOf(rootModuleFolder) < 0) {
          _this.rootModuleFolders.push(rootModuleFolder);
        }
      }

      _this.networkConcurrency = opts.networkConcurrency || Number(_this.getOption('network-concurrency')) || (_constants || _load_constants
()).NETWORK_CONCURRENCY;

      _this.requestManager.setOptions({
        userAgent: String(_this.getOption('user-agent')),
        httpProxy: String(opts.httpProxy || _this.getOption('proxy') || ''),
        httpsProxy: String(opts.httpsProxy || _this.getOption('https-proxy') || ''),
        strictSSL: Boolean(_this.getOption('strict-ssl')),
        ca: Array.prototype.concat(opts.ca || _this.getOption('ca') || []).map(String),
        cafile: String(opts.cafile || _this.getOption('cafile') || ''),
        cert: String(opts.cert || _this.getOption('cert') || ''),
        key: String(opts.key || _this.getOption('key') || ''),
        networkConcurrency: _this.networkConcurrency
      });

      //init & create cacheFolder, tempFolder
      _this.cacheFolder = String(opts.cacheFolder || _this.getOption('cache-folder') || (_constants || _load_constants()).MODULE_CACHE_DIRECTORY
);
      _this.tempFolder = opts.tempFolder || path.join(_this.cacheFolder, '.tmp');
      yield (_fs || _load_fs()).mkdirp(_this.cacheFolder);
      yield (_fs || _load_fs()).mkdirp(_this.tempFolder);

      if (opts.production === 'false') {
        _this.production = false;
      } el ...
```
- example usage
```shell
...
  sortedObject[item] = object[item];
});
return sortedObject;
}

class Config {
constructor(reporter) {
  this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
  this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
  this.reporter = reporter;
  this._init({});
}

//
...
```



# <a name="apidoc.module.yarn.constants"></a>[module yarn.constants](#apidoc.module.yarn.constants)

#### <a name="apidoc.element.yarn.constants.getPathKey"></a>[function <span class="apidocSignatureSpan">yarn.constants.</span>getPathKey (platform, env)](#apidoc.element.yarn.constants.getPathKey)
- description and source-code
```javascript
function getPathKey(platform, env) {
  let pathKey = 'PATH';

  // windows calls its path "Path" usually, but this is not guaranteed.
  if (platform === 'win32') {
    pathKey = 'Path';

    for (const key in env) {
      if (key.toLowerCase() === 'path') {
        pathKey = key;
      }
    }
  }

  return pathKey;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yarn.constants.isRootUser"></a>[function <span class="apidocSignatureSpan">yarn.constants.</span>isRootUser (uid)](#apidoc.element.yarn.constants.isRootUser)
- description and source-code
```javascript
function isRootUser(uid) {
  return uid === 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.yarn.errors"></a>[module yarn.errors](#apidoc.module.yarn.errors)

#### <a name="apidoc.element.yarn.errors.MessageError"></a>[function <span class="apidocSignatureSpan">yarn.errors.</span>MessageError (msg, code)](#apidoc.element.yarn.errors.MessageError)
- description and source-code
```javascript
class MessageError extends Error {
  constructor(msg, code) {
    super(msg);
    this.code = code;
  }

}
```
- example usage
```shell
...
  let isRoot = arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : false;
  return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
    const manifest = yield _this3.maybeReadManifest(dir, priorityRegistry, isRoot);

    if (manifest) {
      return manifest;
    } else {
      throw new (_errors || _load_errors()).MessageError(_this3.reporter.lang('couldntFindPackagejson', dir), 'ENOENT');
    }
  })();
}

/**
* try get the manifest file by looking
* 1. mainfest file in cache
...
```

#### <a name="apidoc.element.yarn.errors.SecurityError"></a>[function <span class="apidocSignatureSpan">yarn.errors.</span>SecurityError {{signature}}](#apidoc.element.yarn.errors.SecurityError)
- description and source-code
```javascript
class SecurityError extends MessageError {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yarn.errors.SpawnError"></a>[function <span class="apidocSignatureSpan">yarn.errors.</span>SpawnError {{signature}}](#apidoc.element.yarn.errors.SpawnError)
- description and source-code
```javascript
class SpawnError extends MessageError {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.yarn.package_compatibility"></a>[module yarn.package_compatibility](#apidoc.module.yarn.package_compatibility)

#### <a name="apidoc.element.yarn.package_compatibility.default"></a>[function <span class="apidocSignatureSpan">yarn.package_compatibility.</span>default (config, resolver, ignoreEngines)](#apidoc.element.yarn.package_compatibility.default)
- description and source-code
```javascript
class PackageCompatibility {
  constructor(config, resolver, ignoreEngines) {
    this.reporter = config.reporter;
    this.resolver = resolver;
    this.config = config;
    this.ignoreEngines = ignoreEngines;
  }

  static isValidArch(archs) {
    return isValid(archs, process.arch);
  }

  static isValidPlatform(platforms) {
    return isValid(platforms, process.platform);
  }

  check(info) {
    let didIgnore = false;
    let didError = false;
    const reporter = this.reporter;
    const human = '${info.name}@${info.version}';

    const pushError = msg => {
      const ref = info._reference;
      invariant(ref, 'expected package reference');

      if (ref.optional) {
        ref.ignore = true;

        reporter.warn('${human}: ${msg}');
        if (!didIgnore) {
          reporter.info(reporter.lang('optionalCompatibilityExcluded', human));
          didIgnore = true;
        }
      } else {
        reporter.error('${human}: ${msg}');
        didError = true;
      }
    };

    const invalidPlatform = !this.config.ignorePlatform && Array.isArray(info.os) && info.os.length > 0 && !PackageCompatibility
.isValidPlatform(info.os);
    if (invalidPlatform) {
      pushError(this.reporter.lang('incompatibleOS', process.platform));
    }

    const invalidCpu = !this.config.ignorePlatform && Array.isArray(info.cpu) && info.cpu.length > 0 && !PackageCompatibility.isValidArch
(info.cpu);
    if (invalidCpu) {
      pushError(this.reporter.lang('incompatibleCPU', process.arch));
    }

    if (!this.ignoreEngines && typeof info.engines === 'object') {
      for (const entry of (0, (_misc || _load_misc()).entries)(info.engines)) {
        let name = entry[0];
        const range = entry[1];

        if (aliases[name]) {
          name = aliases[name];
        }

        if (VERSIONS[name]) {
          if (!testEngine(name, range, VERSIONS, this.config.looseSemver)) {
            pushError(this.reporter.lang('incompatibleEngine', name, range));
          }
        } else if (ignore.indexOf(name) < 0) {
          this.reporter.warn('${human}: ${this.reporter.lang('invalidEngine', name)}');
        }
      }
    }

    if (didError) {
      throw new (_errors || _load_errors()).MessageError(reporter.lang('foundIncompatible'));
    }
  }

  init() {
    const infos = this.resolver.getManifests();
    for (const info of infos) {
      this.check(info);
    }
    return Promise.resolve();
  }
}
```
- example usage
```shell
...
  sortedObject[item] = object[item];
});
return sortedObject;
}

class Config {
constructor(reporter) {
  this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
  this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
  this.reporter = reporter;
  this._init({});
}

//
...
```

#### <a name="apidoc.element.yarn.package_compatibility.testEngine"></a>[function <span class="apidocSignatureSpan">yarn.package_compatibility.</span>testEngine (name, range, versions, looseSemver)](#apidoc.element.yarn.package_compatibility.testEngine)
- description and source-code
```javascript
function testEngine(name, range, versions, looseSemver) {
  const actual = versions[name];
  if (!actual) {
    return false;
  }

  if (!semver.valid(actual, looseSemver)) {
    return false;
  }

  if (semver.satisfies(actual, range, looseSemver)) {
    return true;
  }

  if (name === 'node' && semver.gt(actual, '1.0.0', looseSemver)) {
    // WARNING: this is a massive hack and is super gross but necessary for compatibility
    // some modules have the 'engines.node' field set to a caret version below semver major v1
    // eg. ^0.12.0. this is problematic as we enforce engines checks and node is now on version >=1
    // to allow this pattern we transform the node version to fake ones in the minor range 10-13
    const major = semver.major(actual, looseSemver);
    const fakes = ['0.10.${major}', '0.11.${major}', '0.12.${major}', '0.13.${major}'];
    for (const actualFake of fakes) {
      if (semver.satisfies(actualFake, range, looseSemver)) {
        return true;
      }
    }
  }

  // incompatible version
  return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.yarn.package_constraint_resolver"></a>[module yarn.package_constraint_resolver](#apidoc.module.yarn.package_constraint_resolver)

#### <a name="apidoc.element.yarn.package_constraint_resolver.default"></a>[function <span class="apidocSignatureSpan">yarn.package_constraint_resolver.</span>default (config, reporter)](#apidoc.element.yarn.package_constraint_resolver.default)
- description and source-code
```javascript
class PackageConstraintResolver {
  constructor(config, reporter) {
    this.reporter = reporter;
    this.config = config;
  }

  reduce(versions, range) {
    if (range === 'latest') {
      // Usually versions are already ordered and the last one is the latest
      return Promise.resolve(versions[versions.length - 1]);
    } else {
      return Promise.resolve(semver.maxSatisfying(versions, range, this.config.looseSemver));
    }
  }
}
```
- example usage
```shell
...
  sortedObject[item] = object[item];
});
return sortedObject;
}

class Config {
constructor(reporter) {
  this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
  this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
  this.reporter = reporter;
  this._init({});
}

//
...
```



# <a name="apidoc.module.yarn.package_fetcher"></a>[module yarn.package_fetcher](#apidoc.module.yarn.package_fetcher)

#### <a name="apidoc.element.yarn.package_fetcher.default"></a>[function <span class="apidocSignatureSpan">yarn.package_fetcher.</span>default (config, resolver)](#apidoc.element.yarn.package_fetcher.default)
- description and source-code
```javascript
class PackageFetcher {
  constructor(config, resolver) {
    this.reporter = config.reporter;
    this.resolver = resolver;
    this.config = config;
  }

  fetchCache(dest, fetcher) {
    var _this = this;

    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      var _ref = yield _this.config.readPackageMetadata(dest);

      const hash = _ref.hash,
            pkg = _ref.package;

      return {
        package: pkg,
        resolved: yield fetcher.getResolvedFromCached(hash),
        hash,
        dest,
        cached: true
      };
    })();
  }

  fetch(ref) {
    var _this2 = this;

    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      const dest = _this2.config.generateHardModulePath(ref);

      const remote = ref.remote;
      const Fetcher = (_index || _load_index())[remote.type];
      if (!Fetcher) {
        throw new (_errors || _load_errors()).MessageError(_this2.reporter.lang('unknownFetcherFor', remote.type));
      }

      const fetcher = new Fetcher(dest, remote, _this2.config);

      if (yield _this2.config.isValidModuleDest(dest)) {
        return _this2.fetchCache(dest, fetcher);
      }

      // remove as the module may be invalid
      yield (_fs || _load_fs()).unlink(dest);

      try {
        return yield fetcher.fetch();
      } catch (err) {
        try {
          yield (_fs || _load_fs()).unlink(dest);
        } catch (err2) {
          // what do?
        }
        throw err;
      }
    })();
  }

  maybeFetch(ref) {
    var _this3 = this;

    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      try {
        return yield _this3.fetch(ref);
      } catch (err) {
        if (ref.optional) {
          _this3.reporter.error(err.message);
          return null;
        } else {
          throw err;
        }
      }
    })();
  }

  init() {
    var _this4 = this;

    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      const pkgs = _this4.resolver.getPackageReferences();
      const tick = _this4.reporter.progress(pkgs.length);

      yield (_promise || _load_promise()).queue(pkgs, (() => {
        var _ref2 = (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* (ref) {
          const res = yield _this4.maybeFetch(ref);
          let newPkg;

          if (res) {
            newPkg = res.package;

            // update with new remote
            // but only if there was a hash previously as the tarball fetcher does not provide a hash.
            if (ref.remote.hash) {
              ref.remote.hash = res.hash;
            }

            if (res.resolved) {
              ref.remote.resolved = res.resolved;
            }
          }

          if (newPkg) {
            // update with fresh manifest
            yield _this4.resolver.updateManifest(ref, newPkg);
          }

          if (tick) {
            tick(ref.name);
          }
        });

        return function (_x) {
          return _ref2.apply(this, arguments);
        };
      })(), _this4.config.networkConcurrency);
    })();
  }
}
```
- example usage
```shell
...
  sortedObject[item] = object[item];
});
return sortedObject;
}

class Config {
constructor(reporter) {
  this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
  this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
  this.reporter = reporter;
  this._init({});
}

//
...
```



# <a name="apidoc.module.yarn.package_hoister"></a>[module yarn.package_hoister](#apidoc.module.yarn.package_hoister)

#### <a name="apidoc.element.yarn.package_hoister.HoistManifest"></a>[function <span class="apidocSignatureSpan">yarn.package_hoister.</span>HoistManifest (key, parts, pkg, loc, isIgnored, inheritIsIgnored)](#apidoc.element.yarn.package_hoister.HoistManifest)
- description and source-code
```javascript
class HoistManifest {
  constructor(key, parts, pkg, loc, isIgnored, inheritIsIgnored) {
    this.isIgnored = isIgnored;
    this.inheritIsIgnored = inheritIsIgnored;
    this.loc = loc;
    this.pkg = pkg;

    this.key = key;
    this.parts = parts;
    this.originalKey = key;
    this.previousKeys = [];

    this.history = [];
    this.addHistory('Start position = ${key}');
  }

  addHistory(msg) {
    this.history.push('${++historyCounter}: ${msg}');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.yarn.package_hoister.default"></a>[function <span class="apidocSignatureSpan">yarn.package_hoister.</span>default (config, resolver)](#apidoc.element.yarn.package_hoister.default)
- description and source-code
```javascript
class PackageHoister {
  constructor(config, resolver) {
    this.resolver = resolver;
    this.config = config;

    this.taintedKeys = new Map();
    this.levelQueue = [];
    this.tree = new Map();
  }

<span class="apidocCodeCommentSpan">  /**
   * Taint this key and prevent any modules from being hoisted to it.
   */
</span>
  taintKey(key, info) {
    const existingTaint = this.taintedKeys.get(key);
    if (existingTaint && existingTaint.loc !== info.loc) {
      return false;
    } else {
      this.taintedKeys.set(key, info);
      return true;
    }
  }

  /**
   * Implode an array of ancestry parts into a key.
   */

  implodeKey(parts) {
    return parts.join('#');
  }

  /**
   * Seed the hoister with patterns taken from the included resolver.
   */

  seed(patterns) {
    this.prepass(patterns);

    for (const pattern of this.resolver.dedupePatterns(patterns)) {
      this._seed(pattern);
    }

    while (true) {
      let queue = this.levelQueue;
      if (!queue.length) {
        this._propagateNonIgnored();
        return;
      }

      this.levelQueue = [];

      // sort queue to get determinism between runs
      queue = queue.sort((_ref, _ref2) => {
        var _ref4 = (0, (_slicedToArray2 || _load_slicedToArray()).default)(_ref, 1);

        let aPattern = _ref4[0];

        var _ref3 = (0, (_slicedToArray2 || _load_slicedToArray()).default)(_ref2, 1);

        let bPattern = _ref3[0];

        return (0, (_misc || _load_misc()).sortAlpha)(aPattern, bPattern);
      });

      //
      const infos = [];
      for (const _ref5 of queue) {
        var _ref6 = (0, (_slicedToArray2 || _load_slicedToArray()).default)(_ref5, 2);

        const pattern = _ref6[0];
        const parents = _ref6[1];

        const info = this._seed(pattern, parents);
        if (info) {
          infos.push(info);
        }
      }

      //
      for (const info of infos) {
        this.hoist(info);
      }
    }
  }

  /**
   * Seed the hoister with a specific pattern.
   */

  _seed(pattern, parent) {
    //
    const pkg = this.resolver.getStrictResolvedPattern(pattern);
    const ref = pkg._reference;
    invariant(ref, 'expected reference');

    //
    let parentParts = [];
    let isIgnored = ref.ignore;
    let inheritIsIgnored = false;

    if (parent) {
      if (!this.tree.get(parent.key)) {
        return null;
      }
      // non ignored dependencies inherit parent's ignored status
      // parent may transition from ignored to non ignored when hoisted if it is used in another non ignored branch
      if (!isIgnored && parent.isIgnored) {
        isIgnored = parent.isIgnored;
        inheritIsIgnored = true;
      }
      parentParts = parent.parts;
    }

    //
    const loc = this.config.generateHardModulePath(ref);
    const parts = parentParts.concat(pkg.name);
    const key = this.implodeKey(parts);
    const info = new HoistManifest(key, parts, pkg, loc, isIgnored, inheritIsIgnored);

    //
    this.tree.set(key, info);
    this.taintKey(key, info);

    //
    for (const depPattern of ref.dependencies) {
      this.levelQueue.push([depPattern, info]);
    }

    return info;
  }

  /**
   * Propagate inherited ignore statuses from non-ignored to ignored packages
  */

  _propagateNonIgnored() {
    //
    const toVisit = [];

    // enumerate all non-ignored packages
    for (const entry of this.tree.entries()) {
      if (!entry[1].isIgnored) {
        toVisit.push(entry[1]);
      }
    }

    // visit them
    while (toVisit.length) {
      const info = toVisit.shift();
      const ref = info.pkg._reference;
      invariant(ref, 'expected reference');

      for (const depPattern of ref.dependencies) {
        const depinfo = this._lookupDependency(info, depPattern);
        if (depinfo && depinfo.isIgnored && depinfo.inheritIsIgnored) {
          depinfo.isIgnored = false;
          info.addHistory('Mark as non-ignored because of usage by ${info.key}');
          toVisit.push(depinfo);
        }
      }
    }
  }

  /**
   * Looks up the package a dependency resolves to
  */

  _lookupDependency(info, depPattern) {
    //
    const pkg = ...
```
- example usage
```shell
...
  sortedObject[item] = object[item];
});
return sortedObject;
}

class Config {
constructor(reporter) {
  this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
  this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
  this.reporter = reporter;
  this._init({});
}

//
...
```



# <a name="apidoc.module.yarn.package_install_scripts"></a>[module yarn.package_install_scripts](#apidoc.module.yarn.package_install_scripts)

#### <a name="apidoc.element.yarn.package_install_scripts.default"></a>[function <span class="apidocSignatureSpan">yarn.package_install_scripts.</span>default (config, resolver, force)](#apidoc.element.yarn.package_install_scripts.default)
- description and source-code
```javascript
class PackageInstallScripts {
  constructor(config, resolver, force) {
    this.installed = 0;
    this.resolver = resolver;
    this.reporter = config.reporter;
    this.config = config;
    this.force = force;
  }

  getInstallCommands(pkg) {
    const scripts = pkg.scripts;
    if (scripts) {
      const cmds = [];
      for (const stage of INSTALL_STAGES) {
        const cmd = scripts[stage];
        if (cmd) {
          cmds.push([stage, cmd]);
        }
      }
      return cmds;
    } else {
      return [];
    }
  }

  walk(loc) {
    var _this = this;

    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      const files = yield (_fs || _load_fs()).walk(loc, null, new Set(_this.config.registryFolders));
      const mtimes = new Map();
      for (const file of files) {
        mtimes.set(file.relative, file.mtime);
      }
      return mtimes;
    })();
  }

  saveBuildArtifacts(loc, pkg, beforeFiles, spinner) {
    var _this2 = this;

    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      const afterFiles = yield _this2.walk(loc);

      // work out what files have been created/modified
      const buildArtifacts = [];
      for (const _ref of afterFiles) {
        var _ref2 = (0, (_slicedToArray2 || _load_slicedToArray()).default)(_ref, 2);

        const file = _ref2[0];
        const mtime = _ref2[1];

        if (!beforeFiles.has(file) || beforeFiles.get(file) !== mtime) {
          buildArtifacts.push(file);
        }
      }

      if (!buildArtifacts.length) {
        // nothing else to do here since we have no build artifacts
        return;
      }

      // if the process is killed while copying over build artifacts then we'll leave
      // the cache in a bad state. remove the metadata file and add it back once we've
      // done our copies to ensure cache integrity.
      const cachedLoc = _this2.config.generateHardModulePath(pkg._reference, true);
      const metadata = yield _this2.config.readPackageMetadata(cachedLoc);
      metadata.artifacts = buildArtifacts;

      const metadataLoc = path.join(cachedLoc, (_constants || _load_constants()).METADATA_FILENAME);
      yield (_fs || _load_fs()).writeFile(metadataLoc, JSON.stringify((0, (_extends2 || _load_extends()).default)({}, metadata, {

        // config.readPackageMetadata also returns the package manifest but that's not in the original
        // metadata json
        package: undefined
      }), null, '  '));
    })();
  }

  install(cmds, pkg, spinner) {
    var _this3 = this;

    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      const ref = pkg._reference;
      invariant(ref, 'expected reference');
      const loc = _this3.config.generateHardModulePath(ref);

      try {
        for (const _ref3 of cmds) {
          var _ref4 = (0, (_slicedToArray2 || _load_slicedToArray()).default)(_ref3, 2);

          const stage = _ref4[0];
          const cmd = _ref4[1];

          yield (0, (_executeLifecycleScript || _load_executeLifecycleScript()).default)(stage, _this3.config, loc, cmd, spinner
);
        }
      } catch (err) {
        err.message = '${loc}: ${err.message}';

        invariant(ref, 'expected reference');

        if (ref.optional) {
          ref.ignore = true;
          _this3.reporter.warn(_this3.reporter.lang('optionalModuleScriptFail', err.message));
          _this3.reporter.info(_this3.reporter.lang('optionalModuleFail'));

          // Cleanup node_modules
          try {
            yield (_fs || _load_fs()).unlink(loc);
          } catch (e) {
            _this3.reporter.error(_this3.reporter.lang('optionalModuleCleanupFail', e.message));
          }
        } else {
          throw err;
        }
      }
    })();
  }

  packageCanBeInstalled(pkg) {
    const cmds = this.getInstallCommands(pkg);
    if (!cmds.length) {
      return false;
    }
    const ref = pkg._reference;
    invariant(ref, 'Missing package reference');
    if (!ref.fresh && !this.force) {
      // this package hasn't been touched ...
```
- example usage
```shell
...
  sortedObject[item] = object[item];
});
return sortedObject;
}

class Config {
constructor(reporter) {
  this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
  this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
  this.reporter = reporter;
  this._init({});
}

//
...
```



# <a name="apidoc.module.yarn.package_linker"></a>[module yarn.package_linker](#apidoc.module.yarn.package_linker)

#### <a name="apidoc.element.yarn.package_linker.default"></a>[function <span class="apidocSignatureSpan">yarn.package_linker.</span>default (config, resolver)](#apidoc.element.yarn.package_linker.default)
- description and source-code
```javascript
class PackageLinker {
  constructor(config, resolver) {
    this.resolver = resolver;
    this.reporter = config.reporter;
    this.config = config;
  }

  linkSelfDependencies(pkg, pkgLoc, targetBinLoc) {
    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      targetBinLoc = yield (_fs || _load_fs()).realpath(targetBinLoc);
      pkgLoc = yield (_fs || _load_fs()).realpath(pkgLoc);
      for (const _ref2 of (0, (_misc || _load_misc()).entries)(pkg.bin)) {
        var _ref3 = (0, (_slicedToArray2 || _load_slicedToArray()).default)(_ref2, 2);

        const scriptName = _ref3[0];
        const scriptCmd = _ref3[1];

        const dest = path.join(targetBinLoc, scriptName);
        const src = path.join(pkgLoc, scriptCmd);
        if (!(yield (_fs || _load_fs()).exists(src))) {
          // TODO maybe throw an error
          continue;
        }
        yield linkBin(src, dest);
      }
    })();
  }

  linkBinDependencies(pkg, dir) {
    var _this = this;

    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      const deps = [];

      const ref = pkg._reference;
      invariant(ref, 'Package reference is missing');

      const remote = pkg._remote;
      invariant(remote, 'Package remote is missing');

      // link up 'bin scripts' in 'dependencies'
      for (const pattern of ref.dependencies) {
        const dep = _this.resolver.getStrictResolvedPattern(pattern);
        if (dep.bin && Object.keys(dep.bin).length) {
          deps.push({ dep, loc: _this.config.generateHardModulePath(dep._reference) });
        }
      }

      // link up the 'bin' scripts in bundled dependencies
      if (pkg.bundleDependencies) {
        for (const depName of pkg.bundleDependencies) {
          const loc = path.join(_this.config.generateHardModulePath(ref), _this.config.getFolder(pkg), depName);

          const dep = yield _this.config.readManifest(loc, remote.registry);

          if (dep.bin && Object.keys(dep.bin).length) {
            deps.push({ dep, loc });
          }
        }
      }

      // no deps to link
      if (!deps.length) {
        return;
      }

      // ensure our .bin file we're writing these to exists
      const binLoc = path.join(dir, '.bin');
      yield (_fs || _load_fs()).mkdirp(binLoc);

      // write the executables
      for (const _ref4 of deps) {
        const dep = _ref4.dep,
              loc = _ref4.loc;

        yield _this.linkSelfDependencies(dep, loc, binLoc);
      }
    })();
  }

  getFlatHoistedTree(patterns) {
    const hoister = new (_packageHoister || _load_packageHoister()).default(this.config, this.resolver);
    hoister.seed(patterns);
    return Promise.resolve(hoister.init());
  }

  copyModules(patterns, linkDuplicates) {
    var _this2 = this;

    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      let flatTree = yield _this2.getFlatHoistedTree(patterns);

      // sorted tree makes file creation and copying not to interfere with each other
      flatTree = flatTree.sort(function (dep1, dep2) {
        return dep1[0].localeCompare(dep2[0]);
      });

      // list of artifacts in modules to remove from extraneous removal
      const artifactFiles = [];

      const copyQueue = new Map();
      const hardlinkQueue = new Map();
      const hardlinksEnabled = linkDuplicates && (yield (_fs || _load_fs()).hardlinksWork(_this2.config.cwd));

      const copiedSrcs = new Map();
      for (const _ref5 of flatTree) {
        var _ref6 = (0, (_slicedToArray2 || _load_slicedToArray()).default)(_ref5, 2);

        const dest = _ref6[0];
        var _ref6$ = _ref6[1];
        const pkg = _ref6$.pkg;
        const src = _ref6$.loc;

        const ref = pkg._reference;
        invariant(ref, 'expected package reference');
        ref.setLocation(dest);

        // get a list of build artifacts contained in this module so we can prevent them from being marked as
        // extraneous
        const metadata = yield _this2.config.readPackageMetadata(src);
        for (const file ...
```
- example usage
```shell
...
  sortedObject[item] = object[item];
});
return sortedObject;
}

class Config {
constructor(reporter) {
  this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
  this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
  this.reporter = reporter;
  this._init({});
}

//
...
```

#### <a name="apidoc.element.yarn.package_linker.linkBin"></a>[function <span class="apidocSignatureSpan">yarn.package_linker.</span>linkBin (_x, _x2)](#apidoc.element.yarn.package_linker.linkBin)
- description and source-code
```javascript
function linkBin(_x, _x2) {
  return _ref.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.yarn.package_reference"></a>[module yarn.package_reference](#apidoc.module.yarn.package_reference)

#### <a name="apidoc.element.yarn.package_reference.default"></a>[function <span class="apidocSignatureSpan">yarn.package_reference.</span>default (request, info, remote)](#apidoc.element.yarn.package_reference.default)
- description and source-code
```javascript
class PackageReference {
  constructor(request, info, remote) {
    this.resolver = request.resolver;
    this.lockfile = request.lockfile;
    this.requests = [];
    this.config = request.config;

    this.registry = remote.registry;
    this.version = info.version;
    this.name = info.name;
    this.uid = info._uid;

    this.remote = remote;

    this.dependencies = [];

    this.permissions = {};
    this.patterns = [];
    this.optional = null;
    this.root = false;
    this.ignore = false;
    this.fresh = false;
    this.location = null;
    this.addRequest(request);
  }

  setFresh(fresh) {
    this.fresh = fresh;
  }

  setLocation(loc) {
    return this.location = loc;
  }

  addRequest(request) {
    this.requests.push(request);

    if (!request.parentRequest) {
      this.root = true;
    }
  }

  prune() {
    for (const selfPattern of this.patterns) {
      // remove ourselves from the resolver
      this.resolver.removePattern(selfPattern);
    }
  }

  addDependencies(deps) {
    this.dependencies = this.dependencies.concat(deps);
  }

  setPermission(key, val) {
    this.permissions[key] = val;
  }

  hasPermission(key) {
    if (key in this.permissions) {
      return this.permissions[key];
    } else {
      return false;
    }
  }

  addPattern(pattern, manifest) {
    this.resolver.addPattern(pattern, manifest);

    this.patterns.push(pattern);

    const shrunk = this.lockfile.getLocked(pattern);
    if (shrunk && shrunk.permissions) {
      for (const _ref of (0, (_misc || _load_misc()).entries)(shrunk.permissions)) {
        var _ref2 = (0, (_slicedToArray2 || _load_slicedToArray()).default)(_ref, 2);

        const key = _ref2[0];
        const perm = _ref2[1];

        this.setPermission(key, perm);
      }
    }
  }

  addOptional(optional) {
    if (this.optional == null) {
      // optional is uninitialised
      this.optional = optional;
    } else if (!optional) {
      // otherwise, ignore all subsequent optional assignments and only accept ones making
      // this not optional
      this.optional = false;
    }
  }
}
```
- example usage
```shell
...
  sortedObject[item] = object[item];
});
return sortedObject;
}

class Config {
constructor(reporter) {
  this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
  this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
  this.reporter = reporter;
  this._init({});
}

//
...
```



# <a name="apidoc.module.yarn.package_request"></a>[module yarn.package_request](#apidoc.module.yarn.package_request)

#### <a name="apidoc.element.yarn.package_request.default"></a>[function <span class="apidocSignatureSpan">yarn.package_request.</span>default (req, resolver)](#apidoc.element.yarn.package_request.default)
- description and source-code
```javascript
class PackageRequest {
  constructor(req, resolver) {
    this.parentRequest = req.parentRequest;
    this.lockfile = resolver.lockfile;
    this.registry = req.registry;
    this.reporter = resolver.reporter;
    this.resolver = resolver;
    this.optional = req.optional;
    this.pattern = req.pattern;
    this.config = resolver.config;

    resolver.usedRegistries.add(req.registry);
  }

  static getExoticResolver(pattern) {
    // TODO make this type more refined
    for (const _ref of (0, (_misc || _load_misc()).entries)((_index || _load_index()).exotics)) {
      var _ref2 = (0, (_slicedToArray2 || _load_slicedToArray()).default)(_ref, 2);

      const Resolver = _ref2[1];

      if (Resolver.isVersion(pattern)) {
        return Resolver;
      }
    }
    return null;
  }

  getParentNames() {
    const chain = [];

    let request = this.parentRequest;
    while (request) {
      const info = this.resolver.getStrictResolvedPattern(request.pattern);
      chain.unshift(info.name);

      request = request.parentRequest;
    }

    return chain;
  }

  getLocked(remoteType) {
    // always prioritise root lockfile
    const shrunk = this.lockfile.getLocked(this.pattern);

    if (shrunk && shrunk.resolved) {
      const resolvedParts = (_version || _load_version()).explodeHashedUrl(shrunk.resolved);

      return {
        name: shrunk.name,
        version: shrunk.version,
        _uid: shrunk.uid,
        _remote: {
          resolved: shrunk.resolved,
          type: remoteType,
          reference: resolvedParts.url,
          hash: resolvedParts.hash,
          registry: shrunk.registry
        },
        optionalDependencies: shrunk.optionalDependencies,
        dependencies: shrunk.dependencies
      };
    } else {
      return null;
    }
  }

<span class="apidocCodeCommentSpan">  /**
   * If the input pattern matches a registry one then attempt to find it on the registry.
   * Otherwise fork off to an exotic resolver if one matches.
   */
</span>
  findVersionOnRegistry(pattern) {
    var _this = this;

    return (0, (_asyncToGenerator2 || _load_asyncToGenerator()).default)(function* () {
      var _PackageRequest$norma = PackageRequest.normalizePattern(pattern);

      const range = _PackageRequest$norma.range,
            name = _PackageRequest$norma.name;


      const exoticResolver = PackageRequest.getExoticResolver(range);
      if (exoticResolver) {
        let data = yield _this.findExoticVersionInfo(exoticResolver, range);

        // clone data as we're manipulating it in place and this could be resolved multiple
        // times
        data = Object.assign({}, data);

        // this is so the returned package response uses the overridden name. ie. if the
        // package's actual name is 'bar', but it's been specified in the manifest like:
        //   "foo": "http://foo.com/bar.tar.gz"
        // then we use the foo name
        data.name = name;

        return data;
      }

      const Resolver = _this.getRegistryResolver();
      const resolver = new Resolver(_this, name, range);
      return resolver.resolve();
    })();
  }

  /**
   * Get the registry resolver associated with this package request.
   */

  getRegistryResolver() {
    const Resolver = (_index2 || _load_index2()).registries[this.registry];
    if (Resolver) {
      return Resolver;
    } else {
      throw new (_errors || _load_errors()).MessageError(this.reporter.lang('unknownRegistryResolver', this.registry));
    }
  }

  /**
   * Explode and normalize a pattern into it's name and range.
   */

  static normalizePattern(pattern) {
    let hasVersion = false;
    let range = 'latest';
    let name = pattern;

    // if we're a scope then remove the @ and add it back later
    let isScoped = false;
    if (name[0] === '@') {
      isScoped = true;
      name = name.slice(1);
    }

    // take first part as the name
    const parts = name.split('@');
    if (parts.length > 1) {
      name = parts.shift();
      range = parts.join('@');

      if (range) {
        hasVersion = true;
      } else {
        range = '*';
      }
    }

    // add back @ scope su ...
```
- example usage
```shell
...
  sortedObject[item] = object[item];
});
return sortedObject;
}

class Config {
constructor(reporter) {
  this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
  this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
  this.reporter = reporter;
  this._init({});
}

//
...
```



# <a name="apidoc.module.yarn.package_resolver"></a>[module yarn.package_resolver](#apidoc.module.yarn.package_resolver)

#### <a name="apidoc.element.yarn.package_resolver.default"></a>[function <span class="apidocSignatureSpan">yarn.package_resolver.</span>default (config, lockfile)](#apidoc.element.yarn.package_resolver.default)
- description and source-code
```javascript
class PackageResolver {
  constructor(config, lockfile) {
    this.patternsByPackage = (0, (_map || _load_map()).default)();
    this.fetchingPatterns = (0, (_map || _load_map()).default)();
    this.fetchingQueue = new (_blockingQueue || _load_blockingQueue()).default('resolver fetching');
    this.newPatterns = [];
    this.patterns = (0, (_map || _load_map()).default)();
    this.usedRegistries = new Set();
    this.flat = false;

    this.reporter = config.reporter;
    this.lockfile = lockfile;
    this.config = config;
  }

  // whether the dependency graph will be flattened


  // list of registries that have been used in this resolution


  // activity monitor


  // patterns we've already resolved or are in the process of resolving


  // new patterns that didn't exist in the lockfile


  // TODO


  // these are patterns that the package resolver was seeded with. these are required in
  // order to resolve top level peerDependencies


  // manages and throttles json api http requests


  // list of patterns associated with a package


  // lockfile instance which we can use to retrieve version info


  // a map of dependency patterns to packages


  // reporter instance, abstracts out display logic


  // environment specific config methods and options


<span class="apidocCodeCommentSpan">  /**
   * TODO description
   */
</span>
  isNewPattern(pattern) {
    return this.newPatterns.indexOf(pattern) >= 0;
  }

  /**
   * TODO description
   */

  updateManifest(ref, newPkg) {
    // inherit fields
    const oldPkg = this.patterns[ref.patterns[0]];
    newPkg._reference = ref;
    newPkg._remote = ref.remote;
    newPkg.name = oldPkg.name;

    // update patterns
    for (const pattern of ref.patterns) {
      this.patterns[pattern] = newPkg;
    }

    return Promise.resolve();
  }

  /**
   * Given a list of patterns, dedupe them to a list of unique patterns.
   */

  dedupePatterns(patterns) {
    const deduped = [];
    const seen = new Set();

    for (const pattern of patterns) {
      const info = this.getResolvedPattern(pattern);
      if (seen.has(info)) {
        continue;
      }

      seen.add(info);
      deduped.push(pattern);
    }

    return deduped;
  }

  /**
   * Get a list of all manifests by topological order.
   */

  getTopologicalManifests(seedPatterns) {
    const pkgs = new Set();
    const skip = new Set();

    const add = seedPatterns => {
      for (const pattern of seedPatterns) {
        const pkg = this.getStrictResolvedPattern(pattern);
        if (skip.has(pkg)) {
          continue;
        }

        const ref = pkg._reference;
        invariant(ref, 'expected reference');
        skip.add(pkg);
        add(ref.dependencies);
        pkgs.add(pkg);
      }
    };

    add(seedPatterns);

    return pkgs;
  }

  /**
   * Get a list of all manifests by level sort order.
   */

  getLevelOrderManifests(seedPatterns) {
    const pkgs = new Set();
    const skip = new Set();

    const add = seedPatterns => {
      const refs = [];

      for (const pattern of seedPatterns) {
        const pkg = this.getStrictResolvedPattern(pattern);
        if (skip.has(pkg)) {
          continue;
        }

        const ref = pkg._reference;
        invariant(ref, 'expected reference');

        refs.push(ref);
        skip.add(pkg);
        pkgs.add(pkg);
      }

      for (const ref of refs) {
        add(ref.dependencies);
      }
    };

    add(seedPatterns);

    return pkgs;
  }

  /**
   * Get a list of all package names in the depenency graph.
   */

  getAllDependencyNamesByLevelOrder(seedPatterns) {
    const names = new Set();
    for (const _ref of this.getLevelOrderManifests(seedPatterns)) {
      const name = _ref.name;

      names.add(name);
    }
    return names;
  }

  /**
   * Retrieve all the package info stored for this package name.
   */

  getAllInfoForPackageName(name) {
    const infos = [];
    const seen = new Set();

    for (const pattern of this.patternsByPackage[name]) {
      const info = this.patterns[pattern];
      if (seen.has(info)) {
        continue;
      }

      seen.add(info);
      inf ...
```
- example usage
```shell
...
  sortedObject[item] = object[item];
});
return sortedObject;
}

class Config {
constructor(reporter) {
  this.constraintResolver = new (_packageConstraintResolver || _load_packageConstraintResolver()).default(this, reporter);
  this.requestManager = new (_requestManager || _load_requestManager()).default(reporter);
  this.reporter = reporter;
  this._init({});
}

//
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
