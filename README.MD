
# Cato - a fork of GNU Nano 2.3.99pre3.

## About this fork

I decided to make this fork because this is my CLI editor of choice,
and I was missing some features and customization that I wanted,
while not being forced to learn Vim.

Some improvements include:

* Improved syntax coloring, based on the files in [scopatz/nanorc](https://github.com/scopatz/nanorc/).
* Cleaner status bar.

More is to come later.

## Nano overview

The nano project was started because of a few "problems" with the
wonderfully easy-to-use and friendly Pico text editor.

First and foremost is its license: the Pine suite does not use the
GPL or a GPL-friendly license, and has unclear restrictions on
redistribution.  Because of this, Pine and Pico are not included
with many GNU/Linux distributions.  Also, other features (like go
to line number or search and replace) were unavailable until
recently or require a command line flag.  Yuck.

nano aims to solve these problems by emulating the functionality of
Pico as closely as possible while addressing the problems above and
perhaps providing other extra functionality.

The nano editor is now an official GNU package.  For more
information on GNU and the Free Software Foundation, please see
http://www.gnu.org/.

## Building

Download the nano source code, then:

	tar zxvf nano-x.y.z.tar.gz
	cd nano-x.y.z
	./configure
	make
	make install

It's that simple.  Use --prefix with configure to override the
default installation directory of /usr/local.

If you haven't configured with the "--disable-nanorc" option, after
installation you may want to copy the doc/nanorc.sample to your
home directory, rename it to ".nanorc", and then edit it according
to your taste.

## Current Status

GNU nano has reached its fourth stable milestone, 2.2.x.
Development of new features continues in the 2.3.x branch, while
2.2.x versions are dedicated to bug-fixing and polishing.
