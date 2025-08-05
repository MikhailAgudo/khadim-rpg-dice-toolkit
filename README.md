# Khadim RPG Dice Toolkit

Khadim is a fork of this wonderful plugin (https://github.com/alexkurowski/solo-toolkit).

It is similar to Alex Kurowski's Solo RPG Toolkit, but with a different philosophy in terms of usage and bookkeeping. It aims to not only support solo roleplaying but also aims to help with bookkeeping. In this author's personal experience, bookkeeping is absolutely key for the health of a long-term campaign.

## Features

### Dice roller


### Custom random tables

In addition to default random word generators, you may add any number of your own random tables by creating notes inside a special folder in your vault (default folder name is "Tables", you can change it in plugin settings). To create more table categories, organize your notes into subfolders.


### Inline elements

This plugin also adds a few inline elements that can be helpful when playing TTRPGs.

Note that these elements are disabled by default and can be enabled in plugin settings.

#### Dynamic counters

Code blocks with a single number in it (e.g. `` `5` ``) will be rendered with - and + buttons for quick adjustment.

#### Progress trackers

Code blocks with two numbers separated by a slash (e.g. `` `1/5` ``) will be rendered as a set of checkable boxes or as a clock. Useful for PbtA-style clocks and general progress tracking.

To use specific tracker style:
- Boxes — `` `boxes: 1/5` `` or `` `b:1/5` ``
- Clock — `` `clock: 1/5` `` or `` `c:1/5` ``
- Smaller clock — `` `smclock: 1/5` `` or `` `sc:1/5` ``
- Larger clock — `` `lgclock: 1/5` `` or `` `lc:1/5` ``

#### Dice

Code block with dice notation (e.g. `` `d6` `` or `` `2d8` ``) will be rendered as a dice button that can be rolled by clicking on it.

To change a die color — `` `d6,red` `` or `` `d6,#fb464c` ``

#### Tab stops

Code blocks with only spaces (e.g. `` ` ` ``) will be rendered as a blank space with a set width. Useful when you need a table-like formatting without an actual table.

Example of formatted stats with dynamic counters:

```markdown
Wounds ` ` `1`
Stress `  ` `2`
```

## Installation

### From GitHub Release

Download solo-rpg-toolkit.zip from the latest release, and extract the plugin folder into your vault's plugins folder: `<path-to-vault>/.obsidian/plugins/`.

Note that `.obsidian` folder in your vault may be hidden on Linux and MacOS.

### From source

You'll need at least node-18 to be installed on your machine. Run the following commands while inside the source folder:

```
npm install
npm run build
npm run deploy
```

You will find a newly generated plugin folder `solo-rpg-toolkit` inside folder `dist`. Move the `solo-rpg-toolkit` plugin folder into your vault's plugins folder: `<path-to-vault>/.obsidian/plugins/`.

Note that `.obsidian` folder in your vault may be hidden on Linux and MacOS.

### Updating

Simply replace `<path-to-vault>/.obsidian/plugins/solo-rpg-toolkit` folder with a new one.

Note that plugin settings are stored in the file `<path-to-vault>/.obsidian/plugins/solo-rpg-toolkit/data.json`. You may want to keep it after updating to a newer version.

## Feature and content requests

If you have an idea for a new feature or new content, feel free to create an "issue" on github or reach me at kurowski.dev@gmail.com!
