# RecordMyDesktop

An advanced utility to record your desktop for screencasts.

## Installation

Open terminal and type:

```
$ sudo apt-get install recordmydesktop
```

## Usage

First, if you are using multiple monitors and want to record both, find out the actual display resolution size by typing into terminal:

```
$ xdpyinfo  | grep 'dimensions:'
```

Once you have the full resolution size, make sure you are CDed in the folder you want the video output to go, then you can use these parameters to record your full desktop:

```
$ recordmydesktop --width 1280 --height 720 --full-shots --fps 15 --channels 1 --delay 3
```

This would record a single monitor desktop where the monitor's resolution is 1280x720 with a delay of 3 seconds to allow you to hide your terminal.

```
$ recordmydesktop --width 2560 --height 720 --full-shots --fps 15 --channels 1 --delay 3
```

This would record a dual monitor set up where both monitors are set to a 1280x720 resolution with a delay of 3 seconds.

## Notes


