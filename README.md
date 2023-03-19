![preview](https://media.discordapp.net/attachments/799303953912168469/945058909520035880/unknown.png)

# Brawl-Stream-Tool
Forked from [Ultimate-Stream-Tool](https://github.com/pokerobybeto/Ultimate-Stream-Tool)
*Also available for [Melee](https://github.com/Readek/Melee-Stream-Tool), [Rivals of Aether](https://github.com/Readek/RoA-Stream-Tool) and [Rushdown Revolt](https://github.com/Readek/Rushdown-Revolt-Stream-Tool)!*

So you're interested in doing SSBB streams, huh? Luckily for you, with this tool you'll be able to update all the variables you need for the provided overlays with the provided GUI, and easily customize the overlays to make them your own! 


---

## Features
- [Handy interface](.ReadmeImgs/Interface.png) to quickly change everything you need, like player names, characters, scores, round, casters...
- Easy and fast setup using a browser source. Drag and drop!
- A [game overlay](./ReadmeImgs/Ingame.png) is included, with renders for all characters and skins!
- A [VS Screen](./ReadmeImgs/VSScreen) is also included, to be used in pauses between games.
- A Caster Screen is also included, with a simple overlay on which to write nicks and social networks .
- Easy to customize! Made in html/javascript, every file can be edited at will!
- This is **not** a Stream Control clone. It doesn't have anything to do with it, everything is custom made.
- If you have any feedback, whether it's an issue with the program or a feature you'd like to see in a future release, ping RekRP in the [Brawl Central Discord](https://discord.gg/brawlcentral)

---

## Setup Guide
You can watch [this video](https://www.youtube.com/watch?v=417QjymeOMk) beto made for the ultimate tool, or follow the steps below. 

These are instructions for regular OBS Studio, but I imagine you can do the same with other streaming software:
- Dowmload the ZIP file.
- Extract somewhere.
- Drag and drop `Game Scoreboard.html` into OBS, or add a new browser source in OBS pointing at the local file.
- If the source looks weird, manually set the source's propierties to 1920 width and 1080 height, or set your OBS canvas resolution to 1080p, or make the source fit the screen.
- In the source's propierties, change *Use custom frame rate* -> `60` (if streaming at 60fps of course).
- **Also tick** `Refresh browser when scene becomes active`.
- Manage it all with the `Brawl ST` executable.

Repeat from the 3rd step to add the `VS Screen.html` and `Caster Screen.html`, though I recommend you to do so on another scene.

### Interface shortcuts!
- Press `Enter` to update.
- Press either `F1` or `F2` to increase P1's or P2's score.
- Press `ESC` to clear player info.

2 basic transitions are included in the `Resources/OBS Transitions` folder, if you don't have a transition yourself of course. To use them on OBS:
- Add a new stinger transition.
- Set the video file to `Game In.webm` or `Swoosh.webm`.
- Transition point -> `350 ms`.
- I recommend you to set the Audio Fade Style to crossfade, just in case.
- On the scene's right click menu, set it to Transition Override to the transition you just created.

The interface will also update basic text files with the match info at `Resources/Texts/Simple Texts/` so you can add them to OBS with ease.


---

## Customizing stuff

If you want to customize the GUI, thats going to be a bit complicated since you will have to learn how electron works yourself. In any case, the source code is also on this github!

It is possible to customize how your Scoreboard, VS Screen and Caster Screen look by replacing the files in the overlay folder.

You can also replace the logo simply by adding a 200x200 resolution one.

While to change the position of the icons and writings you should modify parts of the code contained in the `html` and `js` files.

---

If someone wants to upload upscaled renders that would be great :)

--- 
All the renders were taken from [The Spriters Resource](https://www.spriters-resource.com/wii/ssbb)
