---
title: npm-repo
section: 1
description: Open package repository page in the browser
redirect_from:
  - /cli/repo
  - /cli/repo.html
  - /cli/commands/repo
  - /cli-commands/repo
  - /cli-commands/repo.html
  - /cli-commands/npm-repo
github_repo: npm/cli
github_branch: latest
github_path: docs/content/commands/npm-repo.md
---

### Synopsis

```bash
npm repo [<pkgname> [<pkgname> ...]]
```

### Description

This command tries to guess at the likely location of a package's
repository URL, and then tries to open it using the `--browser` config
param. If no package name is provided, it will search for a `package.json`
in the current folder and use the `repository` property.

### Configuration

<!-- AUTOGENERATED CONFIG DESCRIPTIONS START -->
<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->
#### `browser`

* Default: OS X: `"open"`, Windows: `"start"`, Others: `"xdg-open"`
* Type: null, Boolean, or String

The browser that is called by npm commands to open websites.

Set to `false` to suppress browser behavior and instead print urls to
terminal.

Set to `true` to use default system URL opener.

<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->

#### `workspace`

* Default:
* Type: String (can be set multiple times)

Enable running a command in the context of the configured workspaces of the
current project while filtering by running only the workspaces defined by
this configuration option.

Valid values for the `workspace` config are either:

* Workspace names
* Path to a workspace directory
* Path to a parent workspace directory (will result to selecting all of the
  nested workspaces)

When set for the `npm init` command, this may be set to the folder of a
workspace which does not yet exist, to create the folder and set it up as a
brand new workspace within the project.

This value is not exported to the environment for child processes.

<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->

#### `workspaces`

* Default: false
* Type: Boolean

Enable running a command in the context of **all** the configured
workspaces.

This value is not exported to the environment for child processes.

<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->

<!-- AUTOGENERATED CONFIG DESCRIPTIONS END -->

### See Also

* [npm docs](/cli/v7/commands/npm-docs)
* [npm config](/cli/v7/commands/npm-config)
