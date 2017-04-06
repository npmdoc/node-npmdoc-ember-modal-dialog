# api documentation for  [ember-modal-dialog (v1.0.0)](https://github.com/yapplabs/ember-modal-dialog#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-ember-modal-dialog.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ember-modal-dialog) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ember-modal-dialog.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ember-modal-dialog)
#### An ember-cli addon for implementing modal dialogs

[![NPM](https://nodei.co/npm/ember-modal-dialog.png?downloads=true)](https://www.npmjs.com/package/ember-modal-dialog)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ember-modal-dialog/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-ember-modal-dialog_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ember-modal-dialog/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-ember-modal-dialog/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-ember-modal-dialog/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": "",
    "bugs": {
        "url": "https://github.com/yapplabs/ember-modal-dialog/issues"
    },
    "dependencies": {
        "ember-cli-babel": "^5.1.6",
        "ember-cli-htmlbars": "^1.0.8",
        "ember-cli-version-checker": "^1.2.0",
        "ember-wormhole": "~0.3.6"
    },
    "description": "An ember-cli addon for implementing modal dialogs",
    "devDependencies": {
        "broccoli-asset-rev": "^2.4.2",
        "ember-ajax": "^2.0.1",
        "ember-cli": "2.6.2",
        "ember-cli-app-version": "^1.0.0",
        "ember-cli-dependency-checker": "^1.2.0",
        "ember-cli-github-pages": "0.0.6",
        "ember-cli-htmlbars-inline-precompile": "^0.3.1",
        "ember-cli-inject-live-reload": "^1.4.0",
        "ember-cli-lorem-ipsum": "0.0.2",
        "ember-cli-qunit": "^1.4.0",
        "ember-cli-release": "^0.2.9",
        "ember-cli-sass": "3.1.1",
        "ember-cli-uglify": "^1.2.0",
        "ember-code-snippet": "1.3.0",
        "ember-disable-prototype-extensions": "^1.1.0",
        "ember-disable-proxy-controllers": "^1.0.0",
        "ember-export-application-global": "^1.0.5",
        "ember-legacy-views": "0.2.0",
        "ember-load-initializers": "^0.5.1",
        "ember-resolver": "^2.0.3",
        "ember-suave": "1.2.3",
        "ember-tether": "^0.3.1",
        "ember-truth-helpers": "1.2.0",
        "loader.js": "^4.0.1"
    },
    "directories": {
        "doc": "doc",
        "test": "tests"
    },
    "dist": {
        "shasum": "829f083cb4a4162dd2a5158e3980123b7cb69328",
        "tarball": "https://registry.npmjs.org/ember-modal-dialog/-/ember-modal-dialog-1.0.0.tgz"
    },
    "ember-addon": {
        "configPath": "tests/dummy/config",
        "demoURL": "http://yapplabs.github.io/ember-modal-dialog/",
        "versionCompatibility": {
            "ember": ">1.11.0"
        }
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "3b07c8db7ab9972796507db076c337c2a5c052fe",
    "homepage": "https://github.com/yapplabs/ember-modal-dialog#readme",
    "keywords": [
        "ember-addon"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "chrislopresto",
            "email": "chris@chrislopresto.com"
        },
        {
            "name": "lukemelia",
            "email": "luke@lukemelia.com"
        },
        {
            "name": "samselikoff",
            "email": "sam.selikoff@gmail.com"
        }
    ],
    "name": "ember-modal-dialog",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/yapplabs/ember-modal-dialog.git"
    },
    "scripts": {
        "build": "ember build",
        "deploy": "ember github-pages:commit --message \"Deploy gh-pages from commit $(git rev-parse HEAD)\"; git push; git checkout -",
        "start": "ember server",
        "test": "ember try:each"
    },
    "version": "1.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module ember-modal-dialog](#apidoc.module.ember-modal-dialog)
1.  [function <span class="apidocSignatureSpan">ember-modal-dialog.</span>init ()](#apidoc.element.ember-modal-dialog.init)
1.  [function <span class="apidocSignatureSpan">ember-modal-dialog.</span>treeForAddonTemplates (tree)](#apidoc.element.ember-modal-dialog.treeForAddonTemplates)
1.  string <span class="apidocSignatureSpan">ember-modal-dialog.</span>name



# <a name="apidoc.module.ember-modal-dialog"></a>[module ember-modal-dialog](#apidoc.module.ember-modal-dialog)

#### <a name="apidoc.element.ember-modal-dialog.init"></a>[function <span class="apidocSignatureSpan">ember-modal-dialog.</span>init ()](#apidoc.element.ember-modal-dialog.init)
- description and source-code
```javascript
init = function () {
  this._super.init && this._super.init.apply(this, arguments);
  var checker = new VersionChecker(this);

  if (!checker.forEmber().isAbove('0.2.6')) {
    console.warn("Warning: ember-modal-dialog requires ember-cli >= 0.2.6 "
      + "for support for the addon-templates tree, which allows "
      + "us to support various ember versions. Use an older "
      + "version of ember-modal-dialog if you are stuck on an "
      + "older ember-cli.");
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ember-modal-dialog.treeForAddonTemplates"></a>[function <span class="apidocSignatureSpan">ember-modal-dialog.</span>treeForAddonTemplates (tree)](#apidoc.element.ember-modal-dialog.treeForAddonTemplates)
- description and source-code
```javascript
function treeForAddonTemplates(tree) {
  var checker = new VersionChecker(this);
  var emberVersion = checker.forEmber();

  var baseTemplatesPath = path.join(this.root, 'addon/templates');

  if (emberVersion.lt('1.13.0-beta.1')) {
    return this.treeGenerator(path.join(baseTemplatesPath, 'lt-1-13'));
  } else {
    return this.treeGenerator(path.join(baseTemplatesPath, 'current'));
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
