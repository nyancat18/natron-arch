# Inox Browser (inox-patchset)

Inox patchset is applied on the chromium source code and tries to prevent data transmission to Google to get a minimal Chromium based browser. The patches are split up based on features, so it's easy to patch only a subset of them.

Table of Contents
* [Download](#download)
* [Building](#building)
    * [OptDeps](#OptDeps)
    * [Build flags](#build-flags)
* [Credits](#credits)
* [License](#license)
* [Donations](#donations)



## Download
* **Arch Linux**:
Pre-built binaries are hosted in the AUR: [inox-bin](https://aur.archlinux.org/packages/natron/)

## Building

*The build process takes about ½ hour on a shitty pc and 10 min with a good hardware, i5-3550 CPU @ 3.90GHz and 16GB ram. (without ccache)*



### OptDeps

##### firejail-extras
Lets you run Natron at an isolated, network-less enviorment, without run an expensive VM.

##### natron-plugins
A set of python plugins

##### natron-openfx-gmic-bin
Lets you use the GMIC API at Natron

### Build flags
qmake-qt4 -r "$srcdir/natron/Project.pro" PREFIX=/usr CONFIG+=release DEFINES+=QT_NO_DEBUG_OUTPUT QMAKE_CFLAGS_RELEASE="${CFLAGS}" QMAKE_CXXFLAGS_RELEASE="${CXXFLAGS}" QMAKE_LFLAGS_RELEASE="${LDFLAGS}"


## Credits
* [Natron](https://github.com/mrkepzie/natron)


## License
GPLv3. See [LICENSE](LICENSE)

## Donations
Donations are welcome and keep me motivated :-)
* BTC: `1JUhp2T15jPM9Y5r3uWmiyzMbAaRMNdoQg`
* LTC: 'LfDZfSaoyGtm8nEmfE4tsz8MtajPXfDAYd'
