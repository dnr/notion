---
layout: default
title: Home
---

_**Not**ion_ is a tiling, tabbed window manager for the X window system:

* **Tiling**: you divide the screen into non-overlapping 'tiles'. Every window occupies one tile, and is maximized to it
* **Tabbing**: a tile may contain multiple windows - they will be 'tabbed'
* **Static**: most tiled window managers are 'dynamic', meaning they automatically resize and move around tiles as windows appear and disappear. _**Not**ion_, by contrast, does not automatically change the tiling. You're in control.

Features include:

* **Workspaces**: each workspace has its own tiling
* **Multihead**: the [mod_xinerama](https://github.com/raboof/notion/tree/master/mod_xinerama) plugin provides very nice dual-monitor support
* **RandR**: [mod_xrandr](https://github.com/raboof/notion/tree/master/mod_xrandr) picks up changes in the multihead configuration, without the need for restarting _**Not**ion_.
* **Extensibility**: Notion can be extended with [lua](https://www.lua.org/) scripts. Browse through the [scripts collection](https://github.com/raboof/notion/tree/master/contrib).

Supported platforms:

_**Not**ion_ primarily targets Linux, with version 4.0.0 making its way into
distributions now. In the past _**Not**ion_ has also successfully ran on Solaris
(Solaris 10, OpenSolaris and OpenIndiana), NetBSD and OSX. This is not currently
actively supported, however, so running _**Not**ion_ there might need some code
changes.

# Get Notion

Get _**Not**ion_ from our [git repo](https://github.com/raboof/notion), either
by checking out the latest master or downloading a source package for the latest
[release](https://github.com/raboof/notion/releases)

# Documentation

Check out this [quick reference to the keyboard commands](./notionkeys.html)

The manual page is a good reference. For an introduction, you may follow the [tour](tour.html)

For advanced configuration documentation, see [Configuring and extending Notion with Lua](https://raboof.github.io/notion-doc/notionconf/)

For writing patches and modules, see [Notes for the module and patch writer](https://raboof.github.io/notion-doc/notionnotes/)

# Support, bugs and feature requests

See [Contact](contact.html).

# Donations

If you'd like to support Notion, you can donate. I will not spend the donations on myself, as I wouldn't find that fair to all the other contributors. Rather I'll use the funds to cover any costs for Notion or other community projects, or pass on the donations to other organizations doing important work in the open source world.

<div style="width: 100%; align: center">
  <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
     <input type="hidden" name="cmd" value="_s-xclick">
     <input type="hidden" name="hosted_button_id" value="3KPEBSEDFNNJ8">
     <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" name="submit" alt="PayPal - The safer, easier way to pay online!" border="0">
     <img alt="" src="https://www.paypalobjects.com/nl_NL/i/scr/pixel.gif" width="1" height="1" border="0">
  </form>
</div>

If you'd like to associate your donation with a particular support/documentation request, bug or other goal, you can make a note of that.

# History

## Notion 3

The current major version of Notion is Notion 4.
This release includes a number of changes that are either not backwards
compatible, or change the (default) behavior. Those are described in more detail
in the [migration notes](migration.md).

## Ion3

_**Not**ion_ was originally a fork of [Ion](https://tuomov.iki.fi/software/#TOC-Ion-2000-2009-), which has been abandoned by its original author, [Tuomo Valkonen](http://tuomov.iki.fi/).

Former Ion3 users will be glad to hear any changes to configuration will be backwards-compatible, so you can simply drop your `~/.ion3` tweaks into `~/.notion` and rename `cfg_ion.lua` to `cfg_notion.lua`.

# License

Notion 3 is available under a slightly modified LGPL license: in short, the only extra restriction is you cannot release it under the name 'Ion' and cannot mix it with GPL code, but read the license itself for details.

Notion 4, which is not yet released, will be plain LGPL again. You can build a prerelease of Notion 4 from the 'master' branch.