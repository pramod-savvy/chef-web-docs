+++
title = "knife configure"
description = "DESCRIPTION"
draft = false

aliases = "/knife_configure.html"

[menu]
  [menu.docs]
    title = "knife configure"
    identifier = "knife configure/knife_configure.html"
    parent = "chefdk/knife"
    weight = 70
+++    

[\[edit on
GitHub\]](https://github.com/chef/chef-web-docs/blob/master/chef_master/source/knife_configure.rst)

{{% knife_configure_summary %}}

Syntax
======

This subcommand has the following syntax when creating a config.rb file:

``` bash
$ knife configure (options)
```

and the following syntax when creating a client.rb file:

``` bash
$ knife configure client DIRECTORY
```

Options
=======

<div class="note" markdown="1">

<div class="admonition-title" markdown="1">

Note

</div>

{{% knife_common_see_common_options_link %}}

</div>

This subcommand has the following options for use when configuring a
config.rb file:

`--admin-client-name NAME`

:   The name of the client, typically the name of the admin client.

`--admin-client-key PATH`

:   The path to the private key used by the client, typically a file
    named `admin.pem`.

`-i`, `--initial`

:   Create a API client, typically an administrator client on a
    freshly-installed Chef Infra Server.

`-r REPO`, `--repository REPO`

:   The path to the chef-repo.

`--validation-client-name NAME`

:   The name of the validation client, typically a client named
    chef-validator.

`--validation-key PATH`

:   The path to the validation key used by the client, typically a file
    named chef-validator.pem.

<div class="note" markdown="1">

<div class="admonition-title" markdown="1">

Note

</div>

{{% knife_common_see_all_config_options %}}

</div>

Examples
========

The following examples show how to use this knife subcommand:

**Configure config.rb**

``` bash
$ knife configure
```

**Configure client.rb**

``` bash
$ knife configure client '/directory'
```