---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---


## Installation

### Windows

Download and install [FortressOne](https://github.com/FortressOne/fortress-one-installer/releases/latest)


### Linux

Coming soon


## Configuration

Most configuration can be done in-game from the options menu. Save your
configuration by selecting `Options > Config > Save Settings`, or with the
`cfg_save` command.

Team Fortress specific settings are not accessible from the in-game menu. You
can manually edit the .cfg files in the `fortress/` directory.


## Controls

| action                          | key                        | command         |
|---------------------------------|----------------------------|-----------------|
| move forward                    | <kbd>W</kbd>               | `+forward`      |
| move back                       | <kbd>S</kbd>               | `+back`         |
| move left                       | <kbd>A</kbd>               | `+moveleft`     |
| move right                      | <kbd>D</kbd>               | `+moveright`    |
| primary weapon attack           | <kbd>MOUSE1</kbd>          | `+slot1`        |
| secondary weapon attack         | <kbd>MOUSE2</kbd>          | `+slot2`        |
| tertiary weapon attack          | <kbd>MOUSE3</kbd>          | `+slot3`        |
| melee attack                    | <kbd>LSHIFT</kbd>          | `+slot4`        |
| prime / throw hand grenade      | <kbd>Q</kbd>               | `gren1`         |
| prime / throw secondary grenade | <kbd>E</kbd>               | `gren2`         |
| class special action            | <kbd>F</kbd>               | `special`       |
| jump                            | <kbd>SPACE</kbd>           | `+jump`         |
| reload                          | <kbd>R</kbd>               | `reload`        |
| reload next weapon              | <kbd>T</kbd>               | `reloadnext`    |
| select primary weapon           | <kbd>1</kbd>               | `impulse 1`     |
| select secondary weapon         | <kbd>2</kbd>               | `impulse 2`     |
| select tertiary weapon          | <kbd>3</kbd>               | `impulse 3`     |
| select melee weapon             | <kbd>4</kbd>               | `impulse 4`     |
| class menu                      | <kbd>5</kbd>, <kbd>C</kbd> | `impulse 5`     |
| next weapon                     | <kbd>MWHEELUP</kbd>        | `weapnext`      |
| previous weapon                 | <kbd>MWHEELDOWN</kbd>      | `weapprev`      |
| throw flag                      | <kbd>G</kbd>, <kbd>L</kbd> | `dropflag`      |
| drop ammo                       | <kbd>V</kbd>               | `dropammo`      |
| drop backpack                   | <kbd>B</kbd>               | `discard`       |
| call for a medic                | <kbd>M</kbd>               | `saveme`        |
| message everyone                | <kbd>Y</kbd>               | `messagemode`   |
| message team                    | <kbd>U</kbd>               | `messagemode2`  |
| change class                    | <kbd>,</kbd>               | `changeclass`   |
| change team                     | <kbd>.</kbd>               | `changeteam`    |
| map information                 | <kbd>I</kbd>               | `maphelp`       |
| flag information                | <kbd>O</kbd>               | `flaginfo`      |
| inventory                       | <kbd>P</kbd>               | `inv`           |
| show scores                     | <kbd>TAB</kbd>             | `+showscores`   |
| menu                            | <kbd>ESCAPE</kbd>          | `togglemenu`    |
| console                         | <kbd>~</kbd>               | `toggleconsole` |


### Todo

  - [x] Support for [Classic Fortress](http://classicfortress.net/)
  - [ ] Support for [TF 2.9](https://github.com/QWTF/server)
  - [ ] Support for [megaTF](https://github.com/QWTF/server/tree/master/MegaTF_ClanEdition)
  - [ ] Support for [huetf](https://github.com/gmtandi/huetf)
  - [x] Console background
  - [ ] Menu graphics
  - [x] HUD
  - [x] Curation of Team Fortress models and textures
  - [ ] Player model textures
  - [ ] Textures
  - [ ] Skyboxes
  - [ ] Linux Support
  - [ ] Server Installer


### The stack

FortressOne is minimal curated collection of Quake and Team Fortress related files and configurations optimised for competetive play, it includes:


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


### Community

Join the conversation in Discord:

| Region        | Mod              | Language   | Invite link                |
|---------------|------------------|------------|----------------------------|
| Oceania       | classic-fortress | English    | https://discord.gg/3CVEAch |
| North America | megatf           | English    | https://discord.gg/FStt9pw |
| South America | oztf             | Portuguese | https://discord.gg/Ew3NY2Z |


### A note to those coming from TF 2.8, OZTF and MegaTF

* Each classes weapons can now be found at numbers 1 - 4, with 5 being the
  class menu.
* There is a server-side grenade timer. If you have a script to play a grenade
  timer locally, you will likely hear both timers. For push to prime, and again
  to throw, simply bind a key to `gren1` or `gren2`.
* New `+slotx` commands to quickly fire an alternative weapon then return to
  the current weapon have been implemented. E.g. With RL as the active weapon,
`+slot4` will swing the axe before switching back to the RL.
* A `reload_next` command has been added to reload the next alternative weapon.
* The command to throw the flag has been changed from `dropitems` to
  `dropflag`.


### Small maps

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
