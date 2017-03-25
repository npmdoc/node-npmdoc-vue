# api documentation for  [vue (v2.2.5)](https://github.com/vuejs/vue#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-vue.svg)](https://travis-ci.org/npmdoc/node-npmdoc-vue)
#### Reactive, component-oriented view layer for modern web interfaces.

[![NPM](https://nodei.co/npm/vue.png?downloads=true)](https://www.npmjs.com/package/vue)

[![apidoc](https://npmdoc.github.io/node-npmdoc-vue/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-vue_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-vue/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-vue/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Evan You"
    },
    "bugs": {
        "url": "https://github.com/vuejs/vue/issues"
    },
    "dependencies": {},
    "description": "Reactive, component-oriented view layer for modern web interfaces.",
    "devDependencies": {
        "babel-core": "^6.9.0",
        "babel-eslint": "^7.1.0",
        "babel-helper-vue-jsx-merge-props": "^2.0.2",
        "babel-loader": "^6.2.4",
        "babel-plugin-istanbul": "^4.0.0",
        "babel-plugin-syntax-dynamic-import": "^6.18.0",
        "babel-plugin-syntax-jsx": "^6.18.0",
        "babel-plugin-transform-vue-jsx": "^3.2.0",
        "babel-preset-es2015": "^6.9.0",
        "babel-preset-flow-vue": "^1.0.0",
        "buble": "^0.15.2",
        "chromedriver": "^2.21.2",
        "codecov.io": "^0.1.6",
        "cross-spawn": "^5.0.1",
        "de-indent": "^1.0.2",
        "es6-promise": "^4.0.5",
        "eslint": "^3.10.1",
        "eslint-config-vue": "^2.0.1",
        "eslint-loader": "^1.3.0",
        "eslint-plugin-flowtype": "^2.16.0",
        "eslint-plugin-jasmine": "^2.1.0",
        "eslint-plugin-vue": "^2.0.0",
        "flow-bin": "^0.39.0",
        "he": "^1.1.0",
        "http-server": "^0.9.0",
        "jasmine": "^2.5.2",
        "jasmine-core": "^2.5.2",
        "karma": "^1.1.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-coverage": "^1.0.0",
        "karma-firefox-launcher": "^1.0.0",
        "karma-jasmine": "^1.0.2",
        "karma-mocha-reporter": "^2.0.4",
        "karma-phantomjs-launcher": "^1.0.0",
        "karma-safari-launcher": "^1.0.0",
        "karma-sauce-launcher": "^1.0.0",
        "karma-sourcemap-loader": "^0.3.0",
        "karma-webpack": "^2.0.1",
        "lodash": "^4.17.1",
        "nightwatch": "^0.9.9",
        "nightwatch-helpers": "^1.2.0",
        "phantomjs-prebuilt": "^2.1.1",
        "resolve": "^1.2.0",
        "rollup": "^0.41.4",
        "rollup-plugin-alias": "^1.2.0",
        "rollup-plugin-babel": "^2.4.0",
        "rollup-plugin-buble": "^0.15.0",
        "rollup-plugin-flow-no-whitespace": "^1.0.0",
        "rollup-plugin-replace": "^1.1.0",
        "rollup-watch": "^3.2.2",
        "selenium-server": "^2.53.1",
        "typescript": "^2.1.6",
        "uglify-js": "^2.6.2",
        "vue-ssr-html-stream": "^2.1.0",
        "vue-ssr-webpack-plugin": "^1.0.0",
        "webpack": "^2.2.0",
        "weex-js-runtime": "^0.17.0-alpha4",
        "weex-vdom-tester": "^0.1.4"
    },
    "directories": {},
    "dist": {
        "shasum": "528eba68447d7eff99f86767b31176aa656c6963",
        "tarball": "https://registry.npmjs.org/vue/-/vue-2.2.5.tgz"
    },
    "files": [
        "src",
        "dist/*.js",
        "types/*.d.ts"
    ],
    "gitHead": "c0ad75beeb5bf5e7679221b679fbdd13e0d945bb",
    "homepage": "https://github.com/vuejs/vue#readme",
    "keywords": [
        "vue"
    ],
    "license": "MIT",
    "main": "dist/vue.runtime.common.js",
    "maintainers": [
        {
            "name": "yyx990803",
            "email": "yyx990803@gmail.com"
        }
    ],
    "module": "dist/vue.runtime.esm.js",
    "name": "vue",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/vuejs/vue.git"
    },
    "scripts": {
        "bench:ssr": "npm run build:ssr && node benchmarks/ssr/renderToString.js && node benchmarks/ssr/renderToStream.js",
        "build": "node build/build.js",
        "build:ssr": "npm run build -- vue.runtime.common.js,vue-server-renderer",
        "build:weex": "npm run build -- weex-vue-framework,weex-template-compiler",
        "dev": "rollup -w -c build/config.js --environment TARGET:web-full-dev",
        "dev:cjs": "rollup -w -c build/config.js --environment TARGET:web-runtime-cjs",
        "dev:compiler": "rollup -w -c build/config.js --environment TARGET:web-compiler ",
        "dev:ssr": "rollup -w -c build/config.js --environment TARGET:web-server-renderer",
        "dev:test": "karma start build/karma.dev.config.js",
        "dev:weex": "rollup -w -c build/config.js --environment TARGET:weex-framework ",
        "dev:weex:compiler": "rollup -w -c build/config.js --environment TARGET:weex-compiler ",
        "flow": "flow check",
        "install:hooks": "ln -fs ../../build/git-hooks/pre-commit .git/hooks/pre-commit",
        "lint": "eslint src build test",
        "release": "bash build/release.sh",
        "release:weex": "bash build/release-weex.sh",
        "sauce": "karma start build/karma.sauce.config.js",
        "test": "npm run lint && flow check && npm run test:types && npm run test:cover && npm run test:e2e -- --env phantomjs && npm run test:ssr && npm run test:weex",
        "test:cover": "karma start build/karma.cover.config.js",
        "test:e2e": "npm run build -- vue.min.js && node test/e2e/runner.js",
        "test:sauce": "npm run sauce -- 0 && npm run sauce -- 1 && npm run sauce -- 2",
        "test:ssr": "npm run build:ssr && jasmine JASMINE_CONFIG_PATH=test/ssr/jasmine.json",
        "test:types": "tsc -p ./types/test/tsconfig.json",
        "test:unit": "karma start build/karma.unit.config.js",
        "test:weex": "npm run build:weex && jasmine JASMINE_CONFIG_PATH=test/weex/jasmine.json"
    },
    "typings": "types/index.d.ts",
    "unpkg": "dist/vue.js",
    "version": "2.2.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module vue](#apidoc.module.vue)
1.  [function <span class="apidocSignatureSpan">vue.</span>component ( id, definition )](#apidoc.element.vue.component)
1.  [function <span class="apidocSignatureSpan">vue.</span>delete (target, key)](#apidoc.element.vue.delete)
1.  [function <span class="apidocSignatureSpan">vue.</span>directive ( id, definition )](#apidoc.element.vue.directive)
1.  [function <span class="apidocSignatureSpan">vue.</span>extend (extendOptions)](#apidoc.element.vue.extend)
1.  [function <span class="apidocSignatureSpan">vue.</span>filter ( id, definition )](#apidoc.element.vue.filter)
1.  [function <span class="apidocSignatureSpan">vue.</span>mixin (mixin)](#apidoc.element.vue.mixin)
1.  [function <span class="apidocSignatureSpan">vue.</span>nextTick (cb, ctx)](#apidoc.element.vue.nextTick)
1.  [function <span class="apidocSignatureSpan">vue.</span>set (target, key, val)](#apidoc.element.vue.set)
1.  [function <span class="apidocSignatureSpan">vue.</span>use (plugin)](#apidoc.element.vue.use)
1.  number <span class="apidocSignatureSpan">vue.</span>cid
1.  object <span class="apidocSignatureSpan">vue.</span>options
1.  object <span class="apidocSignatureSpan">vue.</span>util
1.  string <span class="apidocSignatureSpan">vue.</span>version

#### [module vue.options](#apidoc.module.vue.options)
1.  [function <span class="apidocSignatureSpan">vue.options.</span>_base (options)](#apidoc.element.vue.options._base)
1.  object <span class="apidocSignatureSpan">vue.options.</span>components
1.  object <span class="apidocSignatureSpan">vue.options.</span>directives
1.  object <span class="apidocSignatureSpan">vue.options.</span>filters

#### [module vue.util](#apidoc.module.vue.util)
1.  [function <span class="apidocSignatureSpan">vue.util.</span>defineReactive ( obj, key, val, customSetter )](#apidoc.element.vue.util.defineReactive)
1.  [function <span class="apidocSignatureSpan">vue.util.</span>extend (to, _from)](#apidoc.element.vue.util.extend)
1.  [function <span class="apidocSignatureSpan">vue.util.</span>mergeOptions ( parent, child, vm )](#apidoc.element.vue.util.mergeOptions)
1.  [function <span class="apidocSignatureSpan">vue.util.</span>warn (msg, vm)](#apidoc.element.vue.util.warn)



# <a name="apidoc.module.vue"></a>[module vue](#apidoc.module.vue)

#### <a name="apidoc.element.vue.component"></a>[function <span class="apidocSignatureSpan">vue.</span>component ( id, definition )](#apidoc.element.vue.component)
- description and source-code
```javascript
component = function ( id, definition ) {
  if (!definition) {
    return this.options[type + 's'][id]
  } else {
<span class="apidocCodeCommentSpan">    /* istanbul ignore if */
</span>    if (process.env.NODE_ENV !== 'production') {
      if (type === 'component' && config.isReservedTag(id)) {
        warn(
          'Do not use built-in or reserved HTML elements as component ' +
          'id: ' + id
        );
      }
    }
    if (type === 'component' && isPlainObject(definition)) {
      definition.name = definition.name || id;
      definition = this.options._base.extend(definition);
    }
    if (type === 'directive' && typeof definition === 'function') {
      definition = { bind: definition, update: definition };
    }
    this.options[type + 's'][id] = definition;
    return definition
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.delete"></a>[function <span class="apidocSignatureSpan">vue.</span>delete (target, key)](#apidoc.element.vue.delete)
- description and source-code
```javascript
function del(target, key) {
  if (Array.isArray(target) && typeof key === 'number') {
    target.splice(key, 1);
    return
  }
  var ob = (target ).__ob__;
  if (target._isVue || (ob && ob.vmCount)) {
    process.env.NODE_ENV !== 'production' && warn(
      'Avoid deleting properties on a Vue instance or its root $data ' +
      '- just set it to null.'
    );
    return
  }
  if (!hasOwn(target, key)) {
    return
  }
  delete target[key];
  if (!ob) {
    return
  }
  ob.dep.notify();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.directive"></a>[function <span class="apidocSignatureSpan">vue.</span>directive ( id, definition )](#apidoc.element.vue.directive)
- description and source-code
```javascript
directive = function ( id, definition ) {
  if (!definition) {
    return this.options[type + 's'][id]
  } else {
<span class="apidocCodeCommentSpan">    /* istanbul ignore if */
</span>    if (process.env.NODE_ENV !== 'production') {
      if (type === 'component' && config.isReservedTag(id)) {
        warn(
          'Do not use built-in or reserved HTML elements as component ' +
          'id: ' + id
        );
      }
    }
    if (type === 'component' && isPlainObject(definition)) {
      definition.name = definition.name || id;
      definition = this.options._base.extend(definition);
    }
    if (type === 'directive' && typeof definition === 'function') {
      definition = { bind: definition, update: definition };
    }
    this.options[type + 's'][id] = definition;
    return definition
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.extend"></a>[function <span class="apidocSignatureSpan">vue.</span>extend (extendOptions)](#apidoc.element.vue.extend)
- description and source-code
```javascript
extend = function (extendOptions) {
  extendOptions = extendOptions || {};
  var Super = this;
  var SuperId = Super.cid;
  var cachedCtors = extendOptions._Ctor || (extendOptions._Ctor = {});
  if (cachedCtors[SuperId]) {
    return cachedCtors[SuperId]
  }

  var name = extendOptions.name || Super.options.name;
  if (process.env.NODE_ENV !== 'production') {
    if (!/^[a-zA-Z][\w-]*$/.test(name)) {
      warn(
        'Invalid component name: "' + name + '". Component names ' +
        'can only contain alphanumeric characters and the hyphen, ' +
        'and must start with a letter.'
      );
    }
  }

  var Sub = function VueComponent (options) {
    this._init(options);
  };
  Sub.prototype = Object.create(Super.prototype);
  Sub.prototype.constructor = Sub;
  Sub.cid = cid++;
  Sub.options = mergeOptions(
    Super.options,
    extendOptions
  );
  Sub['super'] = Super;

  // For props and computed properties, we define the proxy getters on
  // the Vue instances at extension time, on the extended prototype. This
  // avoids Object.defineProperty calls for each instance created.
  if (Sub.options.props) {
    initProps$1(Sub);
  }
  if (Sub.options.computed) {
    initComputed$1(Sub);
  }

  // allow further extension/mixin/plugin usage
  Sub.extend = Super.extend;
  Sub.mixin = Super.mixin;
  Sub.use = Super.use;

  // create asset registers, so extended classes
  // can have their private assets too.
  config._assetTypes.forEach(function (type) {
    Sub[type] = Super[type];
  });
  // enable recursive self-lookup
  if (name) {
    Sub.options.components[name] = Sub;
  }

  // keep a reference to the super options at extension time.
  // later at instantiation we can check if Super's options have
  // been updated.
  Sub.superOptions = Super.options;
  Sub.extendOptions = extendOptions;
  Sub.sealedOptions = extend({}, Sub.options);

  // cache constructor
  cachedCtors[SuperId] = Sub;
  return Sub
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.filter"></a>[function <span class="apidocSignatureSpan">vue.</span>filter ( id, definition )](#apidoc.element.vue.filter)
- description and source-code
```javascript
filter = function ( id, definition ) {
  if (!definition) {
    return this.options[type + 's'][id]
  } else {
<span class="apidocCodeCommentSpan">    /* istanbul ignore if */
</span>    if (process.env.NODE_ENV !== 'production') {
      if (type === 'component' && config.isReservedTag(id)) {
        warn(
          'Do not use built-in or reserved HTML elements as component ' +
          'id: ' + id
        );
      }
    }
    if (type === 'component' && isPlainObject(definition)) {
      definition.name = definition.name || id;
      definition = this.options._base.extend(definition);
    }
    if (type === 'directive' && typeof definition === 'function') {
      definition = { bind: definition, update: definition };
    }
    this.options[type + 's'][id] = definition;
    return definition
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.mixin"></a>[function <span class="apidocSignatureSpan">vue.</span>mixin (mixin)](#apidoc.element.vue.mixin)
- description and source-code
```javascript
mixin = function (mixin) {
  this.options = mergeOptions(this.options, mixin);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.nextTick"></a>[function <span class="apidocSignatureSpan">vue.</span>nextTick (cb, ctx)](#apidoc.element.vue.nextTick)
- description and source-code
```javascript
function queueNextTick(cb, ctx) {
  var _resolve;
  callbacks.push(function () {
    if (cb) { cb.call(ctx); }
    if (_resolve) { _resolve(ctx); }
  });
  if (!pending) {
    pending = true;
    timerFunc();
  }
  if (!cb && typeof Promise !== 'undefined') {
    return new Promise(function (resolve) {
      _resolve = resolve;
    })
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.set"></a>[function <span class="apidocSignatureSpan">vue.</span>set (target, key, val)](#apidoc.element.vue.set)
- description and source-code
```javascript
function set(target, key, val) {
  if (Array.isArray(target) && typeof key === 'number') {
    target.length = Math.max(target.length, key);
    target.splice(key, 1, val);
    return val
  }
  if (hasOwn(target, key)) {
    target[key] = val;
    return val
  }
  var ob = (target ).__ob__;
  if (target._isVue || (ob && ob.vmCount)) {
    process.env.NODE_ENV !== 'production' && warn(
      'Avoid adding reactive properties to a Vue instance or its root $data ' +
      'at runtime - declare it upfront in the data option.'
    );
    return val
  }
  if (!ob) {
    target[key] = val;
    return val
  }
  defineReactive$$1(ob.value, key, val);
  ob.dep.notify();
  return val
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.use"></a>[function <span class="apidocSignatureSpan">vue.</span>use (plugin)](#apidoc.element.vue.use)
- description and source-code
```javascript
use = function (plugin) {
<span class="apidocCodeCommentSpan">  /* istanbul ignore if */
</span>  if (plugin.installed) {
    return
  }
  // additional parameters
  var args = toArray(arguments, 1);
  args.unshift(this);
  if (typeof plugin.install === 'function') {
    plugin.install.apply(plugin, args);
  } else if (typeof plugin === 'function') {
    plugin.apply(null, args);
  }
  plugin.installed = true;
  return this
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vue.options"></a>[module vue.options](#apidoc.module.vue.options)

#### <a name="apidoc.element.vue.options._base"></a>[function <span class="apidocSignatureSpan">vue.options.</span>_base (options)](#apidoc.element.vue.options._base)
- description and source-code
```javascript
function Vue$2(options) {
  if (process.env.NODE_ENV !== 'production' &&
    !(this instanceof Vue$2)) {
    warn('Vue is a constructor and should be called with the 'new' keyword');
  }
  this._init(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vue.util"></a>[module vue.util](#apidoc.module.vue.util)

#### <a name="apidoc.element.vue.util.defineReactive"></a>[function <span class="apidocSignatureSpan">vue.util.</span>defineReactive ( obj, key, val, customSetter )](#apidoc.element.vue.util.defineReactive)
- description and source-code
```javascript
function defineReactive$$1( obj, key, val, customSetter ) {
  var dep = new Dep();

  var property = Object.getOwnPropertyDescriptor(obj, key);
  if (property && property.configurable === false) {
    return
  }

  // cater for pre-defined getter/setters
  var getter = property && property.get;
  var setter = property && property.set;

  var childOb = observe(val);
  Object.defineProperty(obj, key, {
    enumerable: true,
    configurable: true,
    get: function reactiveGetter () {
      var value = getter ? getter.call(obj) : val;
      if (Dep.target) {
        dep.depend();
        if (childOb) {
          childOb.dep.depend();
        }
        if (Array.isArray(value)) {
          dependArray(value);
        }
      }
      return value
    },
    set: function reactiveSetter (newVal) {
      var value = getter ? getter.call(obj) : val;
<span class="apidocCodeCommentSpan">      /* eslint-disable no-self-compare */
</span>      if (newVal === value || (newVal !== newVal && value !== value)) {
        return
      }
      /* eslint-enable no-self-compare */
      if (process.env.NODE_ENV !== 'production' && customSetter) {
        customSetter();
      }
      if (setter) {
        setter.call(obj, newVal);
      } else {
        val = newVal;
      }
      childOb = observe(newVal);
      dep.notify();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.util.extend"></a>[function <span class="apidocSignatureSpan">vue.util.</span>extend (to, _from)](#apidoc.element.vue.util.extend)
- description and source-code
```javascript
function extend(to, _from) {
  for (var key in _from) {
    to[key] = _from[key];
  }
  return to
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.util.mergeOptions"></a>[function <span class="apidocSignatureSpan">vue.util.</span>mergeOptions ( parent, child, vm )](#apidoc.element.vue.util.mergeOptions)
- description and source-code
```javascript
function mergeOptions( parent, child, vm ) {
  if (process.env.NODE_ENV !== 'production') {
    checkComponents(child);
  }
  normalizeProps(child);
  normalizeDirectives(child);
  var extendsFrom = child.extends;
  if (extendsFrom) {
    parent = typeof extendsFrom === 'function'
      ? mergeOptions(parent, extendsFrom.options, vm)
      : mergeOptions(parent, extendsFrom, vm);
  }
  if (child.mixins) {
    for (var i = 0, l = child.mixins.length; i < l; i++) {
      var mixin = child.mixins[i];
      if (mixin.prototype instanceof Vue$2) {
        mixin = mixin.options;
      }
      parent = mergeOptions(parent, mixin, vm);
    }
  }
  var options = {};
  var key;
  for (key in parent) {
    mergeField(key);
  }
  for (key in child) {
    if (!hasOwn(parent, key)) {
      mergeField(key);
    }
  }
  function mergeField (key) {
    var strat = strats[key] || defaultStrat;
    options[key] = strat(parent[key], child[key], vm, key);
  }
  return options
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue.util.warn"></a>[function <span class="apidocSignatureSpan">vue.util.</span>warn (msg, vm)](#apidoc.element.vue.util.warn)
- description and source-code
```javascript
warn = function (msg, vm) {
  if (hasConsole && (!config.silent)) {
    console.error("[Vue warn]: " + msg + " " + (
      vm ? formatLocation(formatComponentName(vm)) : ''
    ));
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
