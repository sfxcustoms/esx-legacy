# es_extended
es_extended is an extention that is developed on top of [EssentialMode](https://essentialmode.com/) (aka ES), thus commonly named ESX - the EssentialMode Extended framework for FiveM.

### Links & Read more
- [Official Discord community](https://discord.me/fivem_esx)
- [ESX Documentation](https://esx-org.github.io/) (things are missing!)
- [ES Documentation](https://docs.essentialmode.com/)

### Screenshot preview (todo)

![screenshot](http://i.imgur.com/aPFdJl3.jpg)

### Features
- Accounts (bank / black money) you can also add others accounts
- Advanced inventory system (press `F2` ingame)
- Job system
- Loadouts and position synced in database
- The best framework out there for RP servers
- i18n (locate) system
- Loads of plugins available

### Requirements
This order also applies in the startup order.
- Base events
- [mysql-async](https://github.com/brouznouf/fivem-mysql-async/releases/latest)
- [EssentialMode](https://essentialmode.com/) (es_admin2 included, a basic admin tool)
- [esplugin_mysql](https://forum.fivem.net/t/release-essentialmode-base/3665/1181)
- [async](https://github.com/ESX-Org/async/releases/latest)

### Download & Installation

**1) Using [fvm](https://github.com/qlaffont/fvm-installer)**

```
fvm install --save --folder=essential esx-org/es_extended
fvm install --save --folder=esx esx-org/esx_menu_default
fvm install --save --folder=esx esx-org/esx_menu_dialog
fvm install --save --folder=esx esx-org/esx_menu_list

```

**2) Manually**

- Download https://github.com/ESX-Org/es_extended/releases/latest
- Put it in the resource/[essential] directory
- Download https://github.com/ESX-Org/esx_menu_default/releases/latest
- Put it in the resource/[esx]/[ui] directory
- Download https://github.com/ESX-Org/esx_menu_dialog/releases/latest
- Put it in the resource/[esx]/[ui] directory
- Download https://github.com/ESX-Org/esx_menu_list/releases/latest
- Put it in the resource/[esx]/[ui] directory

**3) Using git**

```
cd resources
git clone https://github.com/ESX-Org/es_extended [essential]/es_extended
git clone https://github.com/ESX-Org/esx_menu_default [esx]/[ui]/esx_menu_default
git clone https://github.com/ESX-Org/esx_menu_dialog [esx]/[ui]/esx_menu_dialog
git clone https://github.com/ESX-Org/esx_menu_list [esx]/[ui]/esx_menu_list
```

## Installation

1) Import es_extended.sql in your database
2) Configure your `server.cfg` to look like this

```
start baseevents

start mysql-async
start essentialmode
start esplugin_mysql
start es_admin2

start es_extended

start esx_menu_default
start esx_menu_list
start esx_menu_dialog
```
