# api documentation for  [hpm-cli (v2.0.1)](https://github.com/zeit/hpm#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-hpm-cli.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-hpm-cli) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-hpm-cli.svg)](https://travis-ci.org/npmdoc/node-npmdoc-hpm-cli)
#### A plugin manager for Hyper.app

[![NPM](https://nodei.co/npm/hpm-cli.png?downloads=true)](https://www.npmjs.com/package/hpm-cli)

[![apidoc](https://npmdoc.github.io/node-npmdoc-hpm-cli/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-hpm-cli%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-hpm-cli/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-hpm-cli/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-hpm-cli/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matheus Fernandes",
        "email": "npm@matheus.top",
        "url": "http://matheus.top"
    },
    "bin": {
        "hpm": "./index.js"
    },
    "bugs": {
        "url": "https://github.com/zeit/hpm/issues"
    },
    "dependencies": {
        "args": "^2.0.0",
        "chalk": "^1.1.3",
        "columnify": "^1.5.4",
        "execa": "^0.5.0",
        "file-exists": "^2.0.0",
        "got": "^6.3.0",
        "npm-name": "^3.0.0",
        "opn": "^4.0.2",
        "ora": "^0.3.0",
        "pify": "^2.3.0",
        "recast": "^0.11.10",
        "update-notifier": "^1.0.2"
    },
    "description": "A plugin manager for Hyper.app",
    "devDependencies": {
        "ava": "^0.16.0",
        "coveralls": "^2.11.11",
        "is-ci": "^1.0.9",
        "mock-fs": "^3.11.0",
        "nyc": "^8.3.0",
        "xo": "^0.17.0"
    },
    "directories": {},
    "dist": {
        "shasum": "32073c17208dea80f19be811020bba63f3883053",
        "tarball": "https://registry.npmjs.org/hpm-cli/-/hpm-cli-2.0.1.tgz"
    },
    "engines": {
        "node": ">=6"
    },
    "files": [
        "api.js",
        "index.js"
    ],
    "gitHead": "1610fada94e68a1b1c103741743a31defa60e058",
    "homepage": "https://github.com/zeit/hpm#readme",
    "keywords": [
        "hyper.app",
        "hyperapp",
        "hyperterm",
        "package",
        "manager",
        "terminal",
        "cli",
        "🦁"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "leo",
            "email": "mindrun@icloud.com"
        },
        {
            "name": "matheuss",
            "email": "me@matheus.top"
        }
    ],
    "name": "hpm-cli",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/zeit/hpm.git"
    },
    "scripts": {
        "coverage": "nyc report --reporter=text-lcov | coveralls",
        "test": "xo && nyc ava"
    },
    "version": "2.0.1",
    "xo": {
        "space": 2,
        "semicolon": false,
        "esnext": true
    }
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module hpm-cli](#apidoc.module.hpm-cli)
1.  boolean <span class="apidocSignatureSpan">hpm-cli.</span>_inCache
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>_args
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>_npmOperationalInternal
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>_npmUser
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>_phantomChildren
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>_requested
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>_requiredBy
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>_shrinkwrap
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>api
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>author
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>bin
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>bugs
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>dependencies
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>devDependencies
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>directories
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>dist
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>engines
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>files
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>keywords
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>maintainers
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>optionalDependencies
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>repository
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>scripts
1.  object <span class="apidocSignatureSpan">hpm-cli.</span>xo
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>_from
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>_id
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>_location
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>_nodeVersion
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>_npmVersion
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>_resolved
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>_shasum
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>_spec
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>_where
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>description
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>gitHead
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>homepage
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>license
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>main
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>name
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>readme
1.  string <span class="apidocSignatureSpan">hpm-cli.</span>version

#### [module hpm-cli.api](#apidoc.module.hpm-cli.api)
1.  [function <span class="apidocSignatureSpan">hpm-cli.api.</span>exists ()](#apidoc.element.hpm-cli.api.exists)
1.  [function <span class="apidocSignatureSpan">hpm-cli.api.</span>existsOnNpm (plugin)](#apidoc.element.hpm-cli.api.existsOnNpm)
1.  [function <span class="apidocSignatureSpan">hpm-cli.api.</span>install (plugin, locally)](#apidoc.element.hpm-cli.api.install)
1.  [function <span class="apidocSignatureSpan">hpm-cli.api.</span>isInstalled (plugin, locally)](#apidoc.element.hpm-cli.api.isInstalled)
1.  [function <span class="apidocSignatureSpan">hpm-cli.api.</span>list ()](#apidoc.element.hpm-cli.api.list)
1.  [function <span class="apidocSignatureSpan">hpm-cli.api.</span>uninstall (plugin)](#apidoc.element.hpm-cli.api.uninstall)



# <a name="apidoc.module.hpm-cli"></a>[module hpm-cli](#apidoc.module.hpm-cli)



# <a name="apidoc.module.hpm-cli.api"></a>[module hpm-cli.api](#apidoc.module.hpm-cli.api)

#### <a name="apidoc.element.hpm-cli.api.exists"></a>[function <span class="apidocSignatureSpan">hpm-cli.api.</span>exists ()](#apidoc.element.hpm-cli.api.exists)
- description and source-code
```javascript
function exists() {
  if (fs.existsSync(oldConf)) {
    console.log(chalk.yellow('Warning: ${oldConf} should be ${fileName}'))
  }
  return fileContents !== undefined
}
```
- example usage
```shell
...
const updateNotifier = require('update-notifier')

const api = require('./api')
const pkg = require('./package')

updateNotifier({pkg}).notify()

if (!api.exists()) {
  let msg = chalk.red('You don\'t have Hyper.app installed! :(\n')
  msg += '${chalk.red('You are missing')} ${chalk.green('awesomeness')}'
  msg += chalk.red('.\n')
  msg += chalk.green('Check it out: https://hyper.is/')
  console.error(msg)
  process.exit(1)
}
...
```

#### <a name="apidoc.element.hpm-cli.api.existsOnNpm"></a>[function <span class="apidocSignatureSpan">hpm-cli.api.</span>existsOnNpm (plugin)](#apidoc.element.hpm-cli.api.existsOnNpm)
- description and source-code
```javascript
function existsOnNpm(plugin) {
  plugin = plugin.split('#')[0]
  return npmName(plugin).then(available => {
    if (available) {
      const err = new Error('${plugin} not found on npm')
      err.code = 'NOT_FOUND_ON_NPM'
      throw err
    }
  })
}
```
- example usage
```shell
...
args.command(['d', 'docs', 'h', 'home'], 'Open the npm page of a plugin', (name, args) => {
  return opn('http://ghub.io/${args[0]}', {wait: false})
})

args.command(['f', 'fork'], 'Fork a plugin from npm into your ~/.hyper_plugins/local', (name, args) => {
  const spinner = ora('Installing').start()
  const plugin = args[0]
  return api.existsOnNpm(plugin).then(() => {
if (api.isInstalled(plugin, true)) {
  spinner.fail()
  console.error(chalk.red('${plugin} is already installed locally'))
  process.exit(1)
}

const folderName = '${os.homedir()}/.hyper_plugins/local'
...
```

#### <a name="apidoc.element.hpm-cli.api.install"></a>[function <span class="apidocSignatureSpan">hpm-cli.api.</span>install (plugin, locally)](#apidoc.element.hpm-cli.api.install)
- description and source-code
```javascript
function install(plugin, locally) {
  const array = locally ? localPlugins : plugins
  return new Promise((resolve, reject) => {
    existsOnNpm(plugin).then(() => {
      if (isInstalled(plugin, locally)) {
        return reject('${plugin} is already installed')
      }

      array.push(recast.types.builders.literal(plugin))
      save().then(resolve).catch(err => reject(err))
    }).catch(err => {
      if (err.code === 'NOT_FOUND_ON_NPM') {
        reject(err.message)
      } else {
        reject(err)
      }
    })
  })
}
```
- example usage
```shell
...
msg += chalk.green('Check it out: https://hyper.is/')
console.error(msg)
process.exit(1)
}

args.command(['i', 'install'], 'Install a plugin', (name, args) => {
const plugin = args[0]
return api.install(plugin)
		.then(() => console.log(chalk.green('${plugin} installed successfully!')))
		.catch(err => console.error(chalk.red(err)))
})

args.command(['u', 'uni', 'uninstall', 'rm', 'remove'], 'Uninstall a plugin', (name, args) => {
const plugin = args[0]
return api.uninstall(plugin)
...
```

#### <a name="apidoc.element.hpm-cli.api.isInstalled"></a>[function <span class="apidocSignatureSpan">hpm-cli.api.</span>isInstalled (plugin, locally)](#apidoc.element.hpm-cli.api.isInstalled)
- description and source-code
```javascript
function isInstalled(plugin, locally) {
  const array = locally ? localPlugins : plugins
  if (array && Array.isArray(array)) {
    return array.find(entry => getPluginName(entry) === plugin) !== undefined
  }
  return false
}
```
- example usage
```shell
...
  return opn('http://ghub.io/${args[0]}', {wait: false})
})

args.command(['f', 'fork'], 'Fork a plugin from npm into your ~/.hyper_plugins/local', (name, args) => {
  const spinner = ora('Installing').start()
  const plugin = args[0]
  return api.existsOnNpm(plugin).then(() => {
if (api.isInstalled(plugin, true)) {
  spinner.fail()
  console.error(chalk.red('${plugin} is already installed locally'))
  process.exit(1)
}

const folderName = '${os.homedir()}/.hyper_plugins/local'
const fileName = '${folderName}/package.json'
...
```

#### <a name="apidoc.element.hpm-cli.api.list"></a>[function <span class="apidocSignatureSpan">hpm-cli.api.</span>list ()](#apidoc.element.hpm-cli.api.list)
- description and source-code
```javascript
function list() {
  if (Array.isArray(plugins)) {
    return plugins.map(plugin => getPluginName(plugin)).join('\n')
  }
  return false
}
```
- example usage
```shell
...
const plugin = args[0]
return api.uninstall(plugin)
		.then(() => console.log(chalk.green('${plugin} uninstalled successfully!')))
		.catch(err => console.log(chalk.red(err)))
})

args.command(['ls', 'list'], 'List installed plugins', () => {
const plugins = api.list()

if (plugins) {
  console.log(plugins)
} else {
  console.log(chalk.red('No plugins installed yet.'))
}
process.exit(1)
...
```

#### <a name="apidoc.element.hpm-cli.api.uninstall"></a>[function <span class="apidocSignatureSpan">hpm-cli.api.</span>uninstall (plugin)](#apidoc.element.hpm-cli.api.uninstall)
- description and source-code
```javascript
function uninstall(plugin) {
  return new Promise((resolve, reject) => {
    if (!isInstalled(plugin)) {
      return reject('${plugin} is not installed')
    }

    const index = plugins.findIndex(entry => getPluginName(entry) === plugin)
    plugins.splice(index, 1)
    save().then(resolve).catch(err => reject(err))
  })
}
```
- example usage
```shell
...
return api.install(plugin)
		.then(() => console.log(chalk.green('${plugin} installed successfully!')))
		.catch(err => console.error(chalk.red(err)))
})

args.command(['u', 'uni', 'uninstall', 'rm', 'remove'], 'Uninstall a plugin', (name, args) => {
const plugin = args[0]
return api.uninstall(plugin)
		.then(() => console.log(chalk.green('${plugin} uninstalled successfully!')))
		.catch(err => console.log(chalk.red(err)))
})

args.command(['ls', 'list'], 'List installed plugins', () => {
const plugins = api.list()
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
