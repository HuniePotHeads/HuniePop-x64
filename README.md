# HuniePop x64

#### What?
This repository contains 64-bit executables that allow you to run HuniePop in 64-bit on macOS and Windows.

#### Why?
There are no official 64-bit versions of HuniePop available for macOS and Windows. This is a problem especially for Mac users due to the fact that macOS 10.15 (Catalina) has dropped 32-bit support, meaning they can't play the game on their system without installing Windows/Linux or a virtualization program such as Parallels.
<p align="center">
  <img src="Images/Screenshot_01.png?raw=true" alt="Official HuniePop on macOS Catalina"/>
</p>

#### What's the catch?
**The Steam version is not supported**. Steam will just overwrite the executables with the originals upon launching the game or not launch at all. Tryinddg to circumvent this limitation is a gray area and not the aim of this project.

#### How?
* [Download](https://github.com/HuniePotHeads/HuniePop-x64/archive/master.zip) this repository as a ZIP and extract it anywhere or [clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) it using Git.
* Open the `HuniePop-x64` or `HuniePop-x64-master` directory you just downloaded/extracted. We will call this the ***x64 package***.

###### Windows
* Copy the contents of the `Binaries\Windows` directory from the *x64 package* into your HuniePop directory, overwriting/merging `HuniePop.exe` and `HuniePop_Data`.
* Run the game as usual.

###### macOS
* Open the `Binaries\macOS` directory from the *x64 package*, right click `HuniePop` (or `HuniePop.app`) and click *Show Package Contents*.
* Open another Finder window (Command+N) and go to the directory with your original HuniePop game in it and again, right click on `HuniePop` and click *Show Package Contents*.
* Drag and drop the `Contents` directory from the *x64 package* directory into your HuniePop game directory. If done right, it will ask you to Stop, Replace or Merge, select **Merge**.
* Run the game.

###### macOS troubleshooting
* If you are still getting the *`“HuniePop” needs to be updated`* message, rename the app or move it to another directory, macOS will then re-check it's contents and run it.
* If you get a message saying *`“HuniePop” can't be opened because it is from an unidentified developer`*, right click on the app and select *Open*.

## More Info

#### "64-bit" releases of HuniePop
HuniePop is officialy released in six different flavors: 32-bit and 64-bit, for Windows, Mac and Linux, as can be seen on the [SteamDB](https://steamdb.info/app/339800/depots/) depots page. [Humble Bundle](https://www.humblebundle.com/store/huniepop) also has six different versions of HuniePop. [GOG](https://www.gog.com/game/huniepop) on the other hand includes a statement about the game being only 32-bit.

There are a couple of known release names with indicators of what architecture they are, such as `HuniePop_Mac64bit_v1.2.0.zip` and `HuniePop (Windows 64bit)`. However, after several tests, including forcing Steam to download specific depots, we've come to the conclusion that these are identical to the 32-bit releases, and do in fact, run in 32-bit. The only exception is the Linux release, both on Steam and Humble Bundle/GOG, these have the executable name `HuniePop.x86_64` and are truly 64-bit.

#### Full screen mode on macOS
During the testing of this project, we experienced issues with running HuniePop in full screen on macOS, while it works fine on Windows. We are unsure whether this is caused by this 64-bit version or if it is a problem with HuniePop itself. If you get stuck on a full black screen, you should be able to get out of it by pressing Escape.

#### Legality
This repository contains no data from the game, not even it's icon. It is a collection of project files and compiled binaries from a free version of the [Unity Editor](https://unity.com). The binaries that are included are complete replacements and unrelated to the original game files.

#### SHA1 hashes
The included binaries are standard files from Unity 4.2.2, and thus you may come across [different filenames](https://www.virustotal.com/gui/file/6157fc4a15ff0be3b2bc6845d9a93d9bca3bff51/detection) with the same hash.
```
2b64554fd8e562dbd443def3ecb40354e3b119d6  Binaries/macOS/HuniePop.app/Contents/Frameworks/MonoEmbedRuntime/osx/libmono.0.dylib
2f049c1b0e1d99ad50fb57bff207dfeed848de26  Binaries/macOS/HuniePop.app/Contents/MacOS/HuniePop
ef7fdce6d7dcdb307c4a09d330ca540f9a7f218d  Binaries/Windows/HuniePop_Data/Mono/mono.dll
6157fc4a15ff0be3b2bc6845d9a93d9bca3bff51  Binaries/Windows/HuniePop.exe
```

#### Screenshots
<p align="center">
  <img src="Images/Screenshot_02.png?raw=true" alt="HuniePop 64-bit on macOS Catalina"/>
</p>

<p align="center">
  <img src="Images/Screenshot_03.png?raw=true" alt="HuniePop 64-bit on Windows 10"/>
</p>