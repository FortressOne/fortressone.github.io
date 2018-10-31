---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: FortressOne
---


## Installation

### Windows

Download and install [FortressOne for Windows](https://github.com/FortressOne/fortress-one-installer/releases/latest).

_You might get a notifcation that Windows prevented and unknown app from
running. You can click 'More info' > 'Run anyway'._


### Linux

Download [FortressOne for Linux](https://github.com/FortressOne/linux-installer/releases/latest).

```bash
$ sh fortressone-0.2.2.run
```

_Has been tested for Ubuntu 18.04+. It might work on other distros and versions,
but if it doesn't, please
[raise an issue](https://github.com/FortressOne/linux-installer/issues/new)
on GitHub._


## Configuration

Most configuration can be done in-game from the options menu. Save your
configuration by selecting 'Options' > 'Config' > 'Save Settings' or with the
`cfg_save` command.

Team Fortress specific settings are not accessible from the in-game menu. You
can adjust these settings in the `ezquake/configs/config.cfg` file.


## Controls

Currently most controls cannot be set via the in-game menu. Bindings can be
changed via the console. E.g: `bind z throwflag`. Or by editing
`ezquake/configs/config.cfg`.

The default TF2-style key bindings as listed below, can be restored with `exec
cfg/tf2_bindings.cfg`.

[zel's bindings](zels_bindings.md), can be loaded with `exec cfg/zeltf_bindings.cfg`.

Save changes with `cfg_save`.

### Movement

| move forward | <kbd>W</kbd>     | `+forward`   |
| move back    | <kbd>S</kbd>     | `+back`      |
| move left    | <kbd>A</kbd>     | `+moveleft`  |
| move right   | <kbd>D</kbd>     | `+moveright` |
| jump         | <kbd>SPACE</kbd> | `+jump`      |


### Attack

| fire              | <kbd>MOUSE1</kbd> | `+attack` |
| hand grenade      | <kbd>E</kbd>      | `gren1`   |
| secondary grenade | <kbd>F</kbd>      | `gren2`   |
| melee attack      | <kbd>LSHIFT</kbd> | `+slot4`  |


### Action

| class special      | <kbd>MOUSE2</kbd>          | `special`    |
| class menu         | <kbd>C</kbd>, <kbd>5</kbd> | `impulse 5`  |
| reload             | <kbd>R</kbd>               | `reload`     |
| reload next weapon | <kbd>T</kbd>               | `reloadnext` |
| throw flag         | <kbd>G</kbd>, <kbd>L</kbd> | `dropflag`   |
| drop ammo          | <kbd>V</kbd>               | `dropammo`   |
| drop backpack      | <kbd>B</kbd>               | `discard`    |
| call for a medic   | <kbd>M</kbd>               | `saveme`     |
| suicide            | <kbd>K</kbd>               | `kill`       |


### Weapon Switching

| select primary weapon   | <kbd>1</kbd>          | `impulse 1`  |
| select secondary weapon | <kbd>2</kbd>          | `impulse 2`  |
| select tertiary weapon  | <kbd>3</kbd>          | `impulse 3`  |
| select melee weapon     | <kbd>4</kbd>          | `impulse 4`  |
| previous weapon         | <kbd>MWHEELUP</kbd>   | `impulse 11` |
| next weapon             | <kbd>MWHEELDOWN</kbd> | `impulse 12` |
| last weapon             | <kbd>Q</kbd>          | `impulse 13` |


### Menu

| main menu    | <kbd>ESCAPE</kbd> | `togglemenu`    |
| console      | <kbd>~</kbd>      | `toggleconsole` |
| change class | <kbd>,</kbd>      | `changeclass`   |
| change team  | <kbd>.</kbd>      | `changeteam`    |


### Communication

| message everyone | <kbd>Y</kbd> | `messagemode`  |
| message team     | <kbd>U</kbd> | `messagemode2` |


### Information

| show scores      | <kbd>TAB</kbd> | `+showscores` |
| map information  | <kbd>I</kbd>   | `maphelp`     |
| flag information | <kbd>O</kbd>   | `flaginfo`    |
| inventory        | <kbd>P</kbd>   | `inv`         |


## Todo

[Todo list on FortressOne Pivotal Tracker](https://www.pivotaltracker.com/n/projects/2176336)


## Community

Join the conversation in Discord:

| Region        | Mod              | Language   | Invite link                            |
|---------------|------------------|------------|----------------------------------------|
| Oceania       | classic-fortress | English    | <https://discord.fortressone.org>      |
| North America | megatf           | English    | <http://discord.megateamfortress.com> |
| Brazil        | heutf            | Portuguese | <https://discord.gg/Ew3NY2Z>           |


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

Ensure you have `cl_crypt_rcon 1`.

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
- midground2
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
- optics5


### 4v4

- mbasesl
- bam4
- blitzkrieg2
- well6
- tf2k
- turtler
- 2fort5r
- h4rdcore
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
