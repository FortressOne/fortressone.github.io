---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: FortressOne
---


FortressOne is an all in one [QuakeWorld][] [Team Fortress][] package for
Windows and Linux.

It is powered by a modified [ezQuake][], and includes graphical enhancements
from the [Quake Revitalisation Project][], [dox's models][] and
[Plagues pak][], as well as dozens of custom improvements.


## Client Installation

### Windows

Download and run the [FortressOne for Windows installer][].

_You might get a notification that Windows prevented and unknown app from
running. You can click 'More info' > 'Run anyway'._


### Linux

Download the [FortressOne for Linux installer][].

```bash
$ sh fortressone-linux-installer-1.0.0.run
```

_Has been tested for Ubuntu 18.04 and 18.10. It might work on other distros and
versions, but if it doesn't, please [raise an issue][] on GitHub._


## Running a quad on FortressOne servers

### Begin

```
cmd adminpwd <adminpwd>
quadmode
cmd map <map>
```


### End

```
quadmode
cmd timelimit 35
cmd map <map>
```


### Download demo

```
cmd dlist
cmd dl <demo_id>
```


## Community

| Region        | Mod                 | Language   | Invite                      |
|---------------|---------------------|------------|-----------------------------|
| Oceania       | [FortressOne mod][] | English    | [FortressOne Discord][]     |
| North America | [MegaTF][]          | English    | [QWTF NA Discord][]         |
| Brazil        | [hueTF][]           | Portuguese | [Quadclub Brasil Discord][] |
| Russia        | [TF2003][]          | Russian    | [QWTF.RU Discord][]         |


## FortressOne Mod

The [FortressOne mod][] is a continuation of the [Classic Fortress][] mod,
itself a fork of the original Team Fortress 2.9.


### Config changes from Team Fortress 2.9

_This is only relevant to those not using the FortressOne client._

* Weapons for all classes can now be found at `impulse 1` through to `impulse
  4`, with `impulse 5` or `menu` opening the class menu.
* `+slot1` through to `+slot4` quickly fire an alternative weapon then select
  the previous weapn. E.g. With RL as the active weapon, `+slot4` will swing
  the axe before switching back to the RL.
* For push to prime, and again to throw grenades, bind a key to `gren1` or
  `gren2`.
* A `reload_next` command has been added to reload the next alternative weapon.
* Status bar can be enabled and positioned with `setinfo sb n` where n is the
  number of newlines from the top of your screen.
* Auto ID can be activated with `setinfo ai 1`.
* Reading of class config files can be activated with `setinfo ec 1`.
* You can optionally enable a server-side grenade timer with `setinfo nt 2`.


## Maps

There are thousands of QuakeWorld Team Fortress maps. This is a curated list
mostly to remind me of the most playable maps.

### Duel

- 1on1r
- amth1
- sq1
- 1on1forts
- well1on1


### Tiny

- frag
- poop
- xpress3
- xpress2
- minitf2k
- mini32s
- preskool
- mininoheros
- desperat
- 2mach1
- midground
- 2phaze5r


### Small

- drop2
- well6small
- stag2r
- fatta1
- frozen1
- genders2
- rs_zz1
- optics5r


### Medium

- mbasesl
- bam4
- well6
- tf2k
- 2fort5r
- sewer1
- rstrong
- cloudy
- ff-schtop
- ff-destroy
- mordor2
- ff-phantom


### Large
- 2night2
- h4rdcore
- turtler
- blitzkrieg2
- 32smooth
- excel
- ff-monkey
- ff-aardvark
- ff-shutdown2
- lastresort


### 4-team

- spaz4
- king
- koth3
- 2octa4v1


### Pub / Misc

- kotc
- invade4a


[QuakeWorld]:                        https://www.idsoftware.com/en-gb#section-games
[Team Fortress]:                     https://web.archive.org/web/20131005123834/http://www.planetfortress.com/teamfortress/
[ezQuake]:                           https://ezquake.github.io/
[Quake Revitalisation Project]:      https://qrp.quakeone.com/
[dox's models]:                      https://www.quaddicted.com/webarchive/www.planetfortress.com/tfdone_easy/dox/index.html
[Plagues pak]:                       http://members.optusnet.com.au/~plaguespak/
[FortressOne for Windows installer]: https://github.com/FortressOne/windows-installer/releases/latest
[FortressOne for Linux installer]:   https://github.com/FortressOne/linux-installer/releases/latest
[raise an issue]:                    https://github.com/FortressOne/linux-installer/issues/new
[FortressOne Server for Linux]:      https://github.com/FortressOne/linux-server-installer/releases/latest
[FortressOne mod]:                   https://github.com/FortressOne/server-qwprogs
[FortressOne Discord]:               https://discord.fortressone.org
[MegaTF]:                            https://github.com/alissa0/MegaTFCE
[QWTF NA Discord]:                   http://discord.megateamfortress.com
[hueTF]:                             https://github.com/gmtandi/huetf
[Quadclub Brasil Discord]:           https://discord.gg/Ew3NY2Z
[TF2003]:                            https://github.com/angeld29/TF2003-qvm
[QWTF.RU Discord]:                   https://discord.gg/FVuG7br
[Classic Fortress]:                  http://classicfortress.net/
