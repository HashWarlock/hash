oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![GitHub license](https://img.shields.io/github/license/oclif/hello-world)](https://github.com/oclif/hello-world/blob/main/LICENSE)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g hash
$ hash COMMAND
running command...
$ hash (--version)
hash/0.0.0 linux-x64 node-v18.12.1
$ hash --help [COMMAND]
USAGE
  $ hash COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`hash hello PERSON`](#hash-hello-person)
* [`hash hello world`](#hash-hello-world)
* [`hash help [COMMANDS]`](#hash-help-commands)
* [`hash plugins`](#hash-plugins)
* [`hash plugins:install PLUGIN...`](#hash-pluginsinstall-plugin)
* [`hash plugins:inspect PLUGIN...`](#hash-pluginsinspect-plugin)
* [`hash plugins:install PLUGIN...`](#hash-pluginsinstall-plugin-1)
* [`hash plugins:link PLUGIN`](#hash-pluginslink-plugin)
* [`hash plugins:uninstall PLUGIN...`](#hash-pluginsuninstall-plugin)
* [`hash plugins:uninstall PLUGIN...`](#hash-pluginsuninstall-plugin-1)
* [`hash plugins:uninstall PLUGIN...`](#hash-pluginsuninstall-plugin-2)
* [`hash plugins update`](#hash-plugins-update)

## `hash hello PERSON`

Say hello

```
USAGE
  $ hash hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/HashWarlock/hash/blob/v0.0.0/dist/commands/hello/index.ts)_

## `hash hello world`

Say hello world

```
USAGE
  $ hash hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ hash hello world
  hello world! (./src/commands/hello/world.ts)
```

## `hash help [COMMANDS]`

Display help for hash.

```
USAGE
  $ hash help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for hash.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.9/src/commands/help.ts)_

## `hash plugins`

List installed plugins.

```
USAGE
  $ hash plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ hash plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.4.7/src/commands/plugins/index.ts)_

## `hash plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ hash plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ hash plugins add

EXAMPLES
  $ hash plugins:install myplugin 

  $ hash plugins:install https://github.com/someuser/someplugin

  $ hash plugins:install someuser/someplugin
```

## `hash plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ hash plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ hash plugins:inspect myplugin
```

## `hash plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ hash plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ hash plugins add

EXAMPLES
  $ hash plugins:install myplugin 

  $ hash plugins:install https://github.com/someuser/someplugin

  $ hash plugins:install someuser/someplugin
```

## `hash plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ hash plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ hash plugins:link myplugin
```

## `hash plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ hash plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ hash plugins unlink
  $ hash plugins remove
```

## `hash plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ hash plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ hash plugins unlink
  $ hash plugins remove
```

## `hash plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ hash plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ hash plugins unlink
  $ hash plugins remove
```

## `hash plugins update`

Update installed plugins.

```
USAGE
  $ hash plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
