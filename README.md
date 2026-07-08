# FiuBox Testing

FiuBox is an online tool for sketching and sharing instrumental music.
You can find it [here](https://github.com/slarmoo/slarmoosbox/).
It is a modification of [Jukebox](https://jukeebox.github.io/#J4N08Untitledn511s0k08l00e00t2ma7g0fj07r1O_c000U00000000000000i0o32100T0v0pu1j0Vf0000q0wB16110O0dd030wh0h0y0000000000000w000000E1cb60H0aT1v0pu0y01f031752m60q900q0ND010m700330Oa4583d060AcF0B0Q44a4Pf8d4R31251E2cb100ab60t0aTbv0pu0W0cf0000q0DC000000380Oa554d0a0A3F4BeQ9ed4j6Paf1379R000000E6c6260t0a6360H0a770t0a6460X0a6560t0a0000aT5v0pu0-02f011a6010q09620O0438d040HU5000004000000hdE0cT0v0pu1j2Lf021562ka00q0oL010s10031200O023d060ws0hCy0000000000000f000000E3cb100a4400ala0D0aT3v0Ou0003f0000q0wB14410O0vd080SLXtHrrsksrzrrrrh0E1cb60X0aTav0pu0a04f0000q08520O01d230E0cb4h400000000h4g000000014h000000004h400000000h4g000000014h000000004h400000000p1c00000000__00), which is a modification of [Slarmo's Box](https://slarmoo.github.io/slarmoosbox/website/#s5N08Untitledn311s0k02l00e03t2ma7g0fj07r1O_c000U0000000000i0o321T1v0pu25f0000q00A010v3000O0d080h0A5F4B0Q444nPc696R0000E2cb60t0a6360t0aT9v0pu1hf010o500q0040O0d030h0w20MMMDDxxkkoobb550000eeoohhhhoouukkrrkkrrrrxxDDDDuukkkkkkkkkkrrAAMME0cT6v0pu75f010n900q08420O0d030h0WO00E1c270X0aT4v0puf0f1a0q0050O01h0z9999pobqbq5pSBKSJJAArriiiiii07JCABrzrrrrrrr00YrkqHrsrrrrjr005zrAqzrjzrrqr1jRjrqGGrrzsrsA099ijrABJJJIAzrrtirqrqjqixzsrAjrqjiqaqqysttAJqjikikrizrHtBJJAzArzrIsRCITKSS099ijrAJS____Qg99habbCAYrDzh00E0cTav0puh9f0000q0o7120O029d040E0cb4h400000000h4g000000014h000000004h400000000h4g00000000p1900000f_M0), which inturn is a modification of the [ UltraBox](https://ultraabox.github.io/#u5N08Untitledn310s0k02l00e03t1Ua7g0fj07r1O_U00000000i0o321T0v0pue6f0000q0C010ob000O07d4a0w50h2y0000000000000w000000E1c0b6T5v0pua5f060lc2dd2j02e02fd17800q8540O0ad260HK_Sziiirrqih99h0E0c0T1v0pu35f0000qwB16210O01d080A6F0B0Q4ak4Pa660R0000E2c0bn628T2v0pu15f180q040O0d030w0h0E0c0b4h400000000h4g000000014h000000004h400000000p16000000).Wich os a mod of Jummbox(https://jummb.us/#j6N07Unnamedn310s0k0l00e03t2ma7g0fj07r1O_U00000000i0o321T1v0puebf0000q8C010ob0020Oa7d080A9F6B9Q0681Pd756R0000E3c0b862c632T5v0pu88f0000q0B1930Oa1d350HKT-DRJABBBszrrh2E1c0b2T8v0pu1gf010r900q050Oald020x670WOE0c0T4v0puf0f1a0q050Oa1z6666ji8k8k3jSBKSJJAArriiiiii07JCABrzrrrrrrr00YrkqHrsrrrrjr005zrAqzrjzrrqr1jRjrqGGrrzsrsA099ijrABJJJIAzrrtirqrqjqixzsrAjrqjiqaqqysttAJqjikikrizrHtBJJAzArzrIsRCITKSS099ijrAJS____Qg99habbCAYrDzh00E0c0b4h400000000h4g000000014h000000004h400000000p16000000)and the original project.beepbox by John nesky.

FiuBox is a mod of Jukebox that aims to advance Beepbox's capabilities. Feel free to contribute!


All song data is packaged into the URL at the top of your browser. When you make
changes to the song, the URL is updated to reflect your changes. When you are
satisfied with your song, just copy and paste the URL to save and share your
song!

JukeBox, as well as the beepmods which it's based on, are free projects. If you ever feel so inclined, please support the original creator, [John Nesky](http://www.johnnesky.com/), via
[PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=QZJTX9GRYEV9N&currency_code=USD)!

## Compiling

The compilation procedure is identical to the repository for BeepBox. I will include the excerpt on compiling from that page's readme below for convenience:

The source code is available under the MIT license. The code is written in
[TypeScript](https://www.typescriptlang.org/), which requires
[node & npm](https://www.npmjs.com/get-npm), so install those first. Then to
build this project, open a command line ([Git Bash](https://gitforwindows.org/)) and run:

```
git clone https://github.com/slarmoo/slarmoosbox.git
cd slarmoosbox
npm install
npm run build
```

JummBox (and by extension, Slarmoo's Box) makes a divergence from BeepBox that necessitates an additional dependency:
rather than using the (rather poor) default HTML select implementation, the custom
library [select2](https://select2.org) is employed. select2 has an explicit dependency
on [jQuery](https://jquery.com) as well, so you may need to install the following
additional dependencies if they are not picked up automatically.

```
npm install select2
npm install @types/select2
npm install @types/jquery
```

## Code

The code is divided into several folders. This architecture is identical to BeepBox's.

The [synth/](synth) folder has just the code you need to be able to play JukeBox
songs out loud, and you could use this code in your own projects, like a web
game. After compiling the synth code, open website/synth_example.html to see a
demo using it. To rebuild just the synth code, run:

```
npm run build-synth
```

The [editor/](editor) folder has additional code to display the online song
editor interface. After compiling the editor code, open website/index.html to
see the editor interface. To rebuild just the editor code, run:

```
npm run build-editor
```

The [player/](player) folder has a miniature song player interface for embedding
on other sites. To rebuild just the player code, run:

```
npm run build-player
```

The [website/](website) folder contains index.html files to view the interfaces.
The build process outputs JavaScript files into this folder.

## Dependencies

Most of the dependencies are listed in [package.json](package.json),although jukebox also has an indirect, optional dependency on
[lamejs](https://www.npmjs.com/package/lamejs) via
[jsdelivr](https://www.jsdelivr.com/) for exporting .mp3 files. If the user
attempts to export an .mp3 file, jukeBox will direct the browser to download
that dependency on demand. 
Additionally, random envelopes rely on [js-xxhash](https://npmjs.com/package/js-xxhash) for fast hashing. 


## Offline version

If you'd like to BUILD the offline version, enter the following into the command line of your choice:
```
npm run build-offline
```


After building, you can then enter the following to run it for testing purposes:
```
npm run start
```

And to package, run (do ```npm run package-host``` for your host platform; you may need to run git bash as an administrator for non-host platforms):
```
npm run package
```
