# Init script for managing a NodeJS apps via forever

## Installation

Just check out this repository and put directories to your /etc folder.

On BSD system you will probably need to put script to /usr/local/etc/rc.d (in this case, changing path for configuration files is also required)

## Configuration

Edit /etc/forever.d/example.conf with your settings.

You may rename it corresponding to your application name for better identification with multiple NodeJS apps

## Usage

The usage options are simple:
``` bash
  $ /etc/init.d/forever [action] CONFIGURATION-FILE

  actions:
    start               Start the application described in CONFIGURATION-FILE
    stop                Stop the application described in CONFIGURATION-FILE
    restart             Restart the application described in CONFIGURATION-FILE
```

Example:
``` bash
$ /etc/init.d/forever start /etc/forever.d/example.conf
```
