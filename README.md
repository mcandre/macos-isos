# macos-isos: Scripts for generating macOS installation images in standard ISO format

# ABOUT

macos-isos provides scripts for generating digital installation images in a standard ISO format for a variety of macOS versions for archival and educational purposes. macos-isos is NOT intended to promote piracy, but rather to assist in maintaining high quality archives of past operating systems.

# EXAMPLE

```console
$ sudo time lib/generate-iso.macos.sh 10.13 isos
...
       95.91 real        40.93 user        14.85 sys

$ ls isos
macos-10.13.iso  macos-10.13.iso.sha512
```

Unfortunately, the process of generating installation images is unstable, resulting in slightly different ISO content and checksums on each run. So the best way to promote ISO integrity is to build the images from your Apple host. Even worse, the process of generating installation images can be faulty, yielding corrupt images. When in doubt, regenerate your ISO's and test them on an old Apple device or virtual machine. If the ISO works, then make a backup somewhere.

# REQUIREMENTS

## Apple hardware

Buy Apple!

## macOS

Preferably the same or lower version than the desired ISO to be generated.

## macOS installer application

* 10.13 - `Install macOS High Sierra.app`
* 10.12 - `Install macOS Sierra.app`
* 10.11 - `Install OS X El Capitan.app`
* 10.10 - `Install OS X Yosemite.app`
* 10.9 - `Install OS X Mavericks.app`
* 10.8 - `Install OS X Mountain Lion.app`
* 10.7 - `Install OS X Lion.app`

Modern macOS installations are provided via the Mac App Store. Unfortunately, older versions of macOS are regularly removed from the Mac App Store. If you have previously upgraded to one of these installers, it may be accessible via the Purchased tab in the Mac App Store. Or, legacy physical installation media are sold on [apple.com](https://www.apple.com/).

Alternatively, installation media may be available unofficially on [archive.org](https://archive.org/) or peer-to-peer networks, though beware that malware is likely to be inserted into kernels obtained from unofficial sources. When in doubt, compare the checksums for installation media against public consensus [checksums](https://github.com/notpeter/apple-installer-checksums).
