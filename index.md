---
title: site
layout: default
cmd: bat -p about.md
---


# YUSUF BHAM

## About Me

this space intentionally left blank

* * *

## Projects

+ **[zbl]: A hobby UEFI bootmanager**  

  I created zbl as a for-fun bootmanager which aims at feature
  parity with rEFInd. It currently has auto-detection support
  for EFI chainloading and linux kernels, and allows
  configuring the kernel command line arguments. Uniquely, 
  it allows for dynamic selection of the root filesystem for
  kernels with no config set, which makes it plug-and-play
  in situations where you'd otherwise have a difficult time.
  There's also EFI driver loading support.

+ **[hk-modding/api][hk-api]: A modding api for Hollow Knight**  
 
  I'm the current maintainer of the HK modding api, and
  a long-time contributor. The api is a mod loader using
  [MonoMod] for assembly patching and the addition
  of hooks and mod management features.

+ **[scarab]: A Hollow Knight mod installer**  
 
  I created Scarab as a modern cross-platform successor to previous
  [ModInstaller]. It's built on Avalonia and has the typical
  features you'd expect with installing/uninstalling, toggling,
  and auto-updating.

+ **[runic]: toy language**

  `runic` is a language I started as a final project for an advanced functional
  programming class. It's aimed at being a 'low-level' functional language.
  The backend is LLVM using `llvm-hs-pure`. Ideally it'd be a way
  to write low level code without sacrificing functional paradigms,
  but for now it doesn't do much.

+ **[zig.SteamManifestPatcher][zig-smp]: A steam patcher to re-enable downpatching**

  At some point, Valve had updated Steam such that the `download_depot` command,
  no longer functioned within the client - though it's since been re-enabled. 
  This is used by a lot of speedrunning communities, with one example being 
  Hollow Knight - a game I ran myself. People found it a bit more difficult 
  to use something like DepotDownloader, so I found and fixed a no-longer-working
  version, the [SteamManifestFixer]. I initally just re-found the updated 'egg'
  to patch, but it was prone to breakage on every Steam update. I ended up 
  rewriting in zig, for fun, and changing it to dynamically find what to
  patch based on the error it displayed.

+ **[keyjoy]**: a keyboard adapter providing a virtual controller

  After experiencing keyboard hell at a fighting game local,
  I decided to make sure it would never happen again. This
  is a program for the Teensy 4 which allows you to connect
  it to a computer, and a keyboard to it, and then set
  bindings from keyboard keys to controller keys. Then,
  it simply shows up as a generic XInput controller.

[zbl]: https://github.com/fifty-six/zbl
[hk-api]: https://github.com/hk-modding/api
[MonoMod]: https://github.com/MonoMod/MonoMod
[ModInstaller]: https://github.com/ricardosouzag/ModInstaller
[scarab]: https://github.com/fifty-six/Scarab
[runic]: https://github.com/fifty-six/runic
[zig-smp]: https://github.com/fifty-six/zig.SteamManifestPatcher
[SteamManifestFixer]: https://github.com/ioncodes/SteamManifestFixer
[keyjoy]: https://github.com/fifty-six/keyjoy

* * *

## Links

+ code on [github](https://github.com/fifty-six)
+ [mastodon](https://social.treehouse.systems/@fiftysix)

### Contact

+ e-mail: `fiftysix (AT) fiftysix (DOT) dev`
+ discord: `@56`
+ matrix: `@fifty-six:matrix.org`

* * *
