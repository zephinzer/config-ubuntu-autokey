# AutoKey Configuration for Ubuntu
This repository contains AutoKey configuration data for Mac OS X keybindings.

## Pre-Requisites
Install AutoKey:

```bash
sudo apt install autokey-gtk;
```

Verify that the configuration directory exists:

```bash
stat ~/.config/autokey;
```

## Usage
1. Navigate to your AutoKey configuration directory
2. Make a backup of the `data` directory
3. Clone this repository into the `data` directory

This can be achieved using the following shell commands:

```bash
set -x;
cd ~/.config/autokey \
  && mv data data.backup.$(date +'%Y%m%d%H%M%S') \
  && git clone git@github.com:zephinzer/config-ubuntu-autokey.git data;
```

Then start AutoKey and you should have the shortcuts applied.

Enjoy!

## Tested On
- Ubuntu 16.04
