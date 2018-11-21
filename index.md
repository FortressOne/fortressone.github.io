---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: FortressOne
---


FortressOne is a stand-alone
[QuakeWorld](https://www.idsoftware.com/en-gb#section-games)
[Team Fortress](https://web.archive.org/web/20131005123834/http://www.planetfortress.com/teamfortress/)
(QWTF) package for Windows and Linux.

It is powered by a modified [ezQuake](https://ezquake.github.io/), and includes
graphical enhancements from the [Quake Revitalisation Project](https://qrp.quakeone.com/),
[dox's models](https://www.quaddicted.com/webarchive/www.planetfortress.com/tfdone_easy/dox/index.html)
and [Plagues pak](http://members.optusnet.com.au/~plaguespak/), as well as
dozens of custom improvements.


## Client Installation

### Windows

Download and run the [FortressOne for Windows installer](https://github.com/FortressOne/windows-installer/releases/latest).

_You might get a notification that Windows prevented and unknown app from
running. You can click 'More info' > 'Run anyway'._


### Linux

Download the [FortressOne for Linux installer](https://github.com/FortressOne/linux-installer/releases/latest).

```bash
$ sh fortressone-linux-installer-1.0.0.run
```

_Has been tested for Ubuntu 18.04 and 18.10. It might work on other distros and versions,
but if it doesn't, please
[raise an issue](https://github.com/FortressOne/linux-installer/issues/new)
on GitHub._


## Server Installation

### Linux

Download [FortressOne Server for Linux](https://github.com/FortressOne/linux-server-installer/releases/latest).

```bash
$ sh fortressonesv-0.1.0.run
```


### Usage

```bash
$ ./mvdsv
```


## Community

Join the conversation in Discord:

| Region        | Mod         | Language   | Invite link                            |
|---------------|-------------|------------|----------------------------------------|
| Oceania       | fortressone | English    | <https://discord.fortressone.org>      |
| North America | megatf      | English    | <http://discord.megateamfortress.com>  |
| Brazil        | huetf       | Portuguese | <https://discord.gg/Ew3NY2Z>           |


## Playing on a FortressOne server without the FortressOne package

This isn't recommended or supported, but if you insist, some of the breaking
changes from TF 2.9 are listed below:

* Weapons for all classes can now be found at `impulse 1` through to `impulse
  4`, with `impulse 5` or `menu` opening the class menu.
* `+slot1` through to `+slot4` quickly fire an alternative weapon then select
  the previous weapn. E.g. With RL as the active weapon, `+slot4` will swing
  the axe before switching back to the RL.
* A `reload_next` command has been added to reload the next alternative weapon.
* You can disable the server-side grenade timer with `setinfo nt 2`.
* For push to prime, and again to throw, bind a key to `gren1` or `gren2`.
* The command to throw the flag has been changed from `dropitems` to
  `dropflag`.
* Status bar can be enabled and positioned with `setinfo sb n` where n is the
  number of newlines from the top of your screen.
* Auto ID can be activated with `setinfo ai 1`.


## Commands for running a quad on FortressOne servers

Ensure you have `cl_crypt_rcon 1`. (This is default in the FortressOne client)

### Begin

```
rcon_password <password>
rcon quadmode
rcon map <map>
```

Ask in the [Discord server](https://discord.fortressone.org) for the password.


### End

```
rcon pubmode
rcon map <map>
```


## Maps


### 1v1

- 1on1r
- amth1
- frag
- sq1
- soulsq1
- 1on1forts
- well1on1


### 2v2

- poop
- xpress3
- xpress2
- minitf2k
- mini32s
- preskool
- mininoheros
- desperat


### 3v3

- 2phaze5r
- drop2
- well6small
- stag2r
- fatta1
- frozen1
- genders2
- rs_zz1
- rstrong
- egypt
- optics5r


### 4v4

- mbasesl
- bam4
- blitzkrieg2
- well6
- tf2k
- turtler
- 2fort5r
- h4rdcore
- 32smooth
- 2night2
- sewer1
- excel
- cloudy


### 4-team

- spaz4
- king
- koth3
- 2octa4v1


### Pub / Misc

- kotc
- invade4a


Many of these maps will work with less or more players than suggest above.
