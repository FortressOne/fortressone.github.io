---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: FortressOne
---


## Installation

### Windows

Download and install [FortressOne](https://github.com/FortressOne/fortress-one-installer/releases/latest).

_Note: You might get a notifcation that Windows prevented and unknown app from
running. You can click 'More info' > 'Run anyway'._

### Linux

Coming soon.


## Configuration

Most configuration can be done in-game from the options menu. Save your
configuration by selecting `Options > Config > Save Settings` or with the
`cfg_save` command.

Team Fortress specific settings are not accessible from the in-game menu. You
can adjust these settings in the `ezquake/configs/config.cfg` file.


## Controls

Currently most controls cannot be set via the in-game menu. Bindings can be
changed via the console. E.g: `bind z throwflag`. Or by editing
`ezquake/configs/config.cfg`.

The default TF2-style key bindings as listed below, can be restored with `exec
cfg/tf2_bindings.cfg`.

zel's bindings, can be loaded with `exec cfg/zeltf_bindings.cfg`.

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

- [x] Support for [Classic Fortress](http://classicfortress.net/)
- [ ] Support for [TF 2.9](https://github.com/QWTF/server)
- [ ] Support for [megaTF](https://github.com/QWTF/server/tree/master/MegaTF_ClanEdition)
- [ ] Support for [huetf](https://github.com/gmtandi/huetf)
- [x] Console background
- [ ] Edit server-mod options directly from ezQuake menu
- [ ] Menu graphics
- [x] HUD
- [x] Curation of Team Fortress models and textures
- [ ] Player model textures
- [ ] Textures
- [ ] Skyboxes
- [ ] Linux Support
- [ ] Server Installer


## The stack

FortressOne is minimal curated collection of Quake and Team Fortress related
files and configurations optimised for competetive play, it includes:


| Client    |
|-----------|----------------------------------------------------------|
| client    | [ezQuake](https://ezquake.github.io/)                    |
| Quake gfx | [Quake Revitalization Project](http://qrp.quakeone.com/) |
| TF gfx    | various sources                                          |


It is designed to run with the following server configuration:

| Server          |                                                                                       |
|-----------------|---------------------------------------------------------------------------------------|
| server          | [mvdsv](https://github.com/deurk/mvdsv)                                               |
| server-side mod | [Classic Fortress](http://classicfortress.net/)                                       |
| server-side cfg | [Classic Fortress server-scripts](https://github.com/Classic-Fortress/server-scripts) |


## Community

Join the conversation in Discord:

| Region        | Mod              | Language   | Invite link                  |
|---------------|------------------|------------|------------------------------|
| Oceania       | classic-fortress | English    | <https://discord.gg/3CVEAch> |
| North America | megatf           | English    | <https://discord.gg/FStt9pw> |
| Brazil        | heutf            | Portuguese | <https://discord.gg/Ew3NY2Z> |


## A note to those coming from TF 2.8, OZTF and MegaTF

FortressOne is currently only configured for [this fork](https://github.com/FortressOne/server-qwprogs)
of the [classic-fortress](http://classicfortress.net) mod, itself a
continuation of TF 2.9.

* Weapons for all classes can now be found at `impulse 1` through to `impulse
  4`, with `impulse 5` being the class menu.
* `+slot1` through to `+slot4` quickly fire an alternative weapon then select
  the previous weapn. E.g. With RL as the active weapon, `+slot4` will swing
  the axe before switching back to the RL.
* A `reload_next` command has been added to reload the next alternative weapon.
* You can disable the server-side grenade timer with `setinfo nt 2`
* For push to prime, and again to throw, bind a key to `gren1` or `gren2`.
* The command to throw the flag has been changed from `dropitems` to
  `dropflag`.


## Server commands for running a quad on qw://fortressone.ga

Begin:

```
rcon_password <password>
rcon localinfo clan on
rcon localinfo prematch 1
rcon timelimit 11
rcon password <server_password>
rcon map <map>
```

End:

```
rcon localinfo clan off
rcon localinfo prematch 0
rcon timelimit 15
rcon password none
rcon map <map>
```


## Small maps

This is just a recommended list of small maps to try.

- 1on1forts
- 2mach1
- 2octa4v1
- amth1
- cloudy
- dbox1a
- desperat
- duel2
- egypt
- excel
- frozen
- genders2
- koth3
- ktod
- lms_siege
- long
- metal
- mini32s
- mininoheros
- mininoheros2
- minitf2k
- optics5
- preskool
- rrbat1
- rs_zz1
- rstrong
- soulsq1
- sq1
- swamp3
- well1on1
- xpress2
- xpress3
{: #maps}
