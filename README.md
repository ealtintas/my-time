# my-time

**Turkish:** Bash ile yazılmış bu betik, basitçe zamanı uygun bir biçimde basar.

## Description

Print, type (from keyboard) or copy to clipboard time in various forms.

## Info

This is a simple bash script which helps command line hackers to type time in various convinient forms...

If you use a window manager like openbox you may use this script as a handy keyboard shortcut for printing time.

An example snippet for ~/openbox/rc.xml:

```
...
    <keybind key="W-S-t">
      <action name="Execute">
        <command>/{PATH-TO-THIS-SCRIPT}/my-time -k</command>
      </action>
    </keybind>
...
```

You may also use it in your own scripts to refer to time information in a cleaner way than 'date +FORMAT'.

## Usage

```
Usage: my-time [options]
	-h	show this help
	-f	use modfication of the specified file instead of current time. If this option is not specified current system time is used.
	-s	time in short form
	-c	time in compact form
	-n	time in normal form (default)
	-l	time in long form
	-d	use just day portion
	-t	use just time portion
	-k	type it with keyboard (will also push to clipboard, will not print to stdout)
	-b	just push it to clipboard (will not print)
	-p	just print it stdout (default option)

```

## Examples

```
$ my-time
201016_073253

$ my-time -s
201016_0732

$ my-time -l
2020-10-16_07-32-21

$ my-time -d
201016

$ my-time -t
073231

```
