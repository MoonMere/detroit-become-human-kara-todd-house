<p align="right"><a href="https://github.com/MoonMere/detroit-become-human-kara-todd-house/blob/main/README.zh-CN.md"><kbd>中文</kbd></a></p>

# Kara and Todd's House from Detroit: Become Human, Recreated in the Browser

This is an unofficial fan recreation of the house from the game's 'A New Home' chapter, made as a personal project with no commercial purpose. It contains no assets from the game and is not affiliated with Sony Interactive Entertainment or Quantic Dream. If a rights holder asks, I will take it down.

**Status: work in progress.** This repository holds screenshots only. The source code is private.

![Walking through the kitchen, entry hall, dining area and living room in the browser, with the grey placeholder figure](images/00_walkthrough.gif)

*Walking through the ground floor in the browser, with the grey placeholder figure.*

## What it is

A 3D model of the whole house that you can walk around in a web browser. You will play in third person as a new android designed for this project, who takes Kara's place and does the housework. Until that character is made, a grey placeholder figure stands in.

## How I am making it with AI

Claude Code writes all of the code, from the Python scripts that build the house in Blender to the three.js code that runs it in the browser. My part is deciding what the game should be, judging the results and changing course when something is not working.

* Earlier versions of the house were built in browser code. One night the AI worked for seven hours, and the result was no better than an hour's work the night before. I asked why it was not using Blender and had it rebuild one kitchen corner in Blender as a small test, judged by a separate AI. Blender clearly won, so I had the whole house rebuilt in Blender.
* I noticed the walkway between the coffee table and the TV was far narrower than in the game, which the AI's own checks had missed. I then required the AI to measure five things in every comparison with the game: layout, furnishings, materials, light and camera framing. Working to that rule, the AI measured every room again and reworked the layout of the whole house.
* I generated the android's concept art with an AI image generator over many attempts, and I chose her look, from the hairstyle to the outfit. When the first head the AI built was still poor after six hours, with eyes I rated 1 out of 10, I decided to rebuild the head with Epic's MetaHuman.
* I set the scope and the limits. The game covers the whole chapter, upstairs and the backyard included, and must run at 30 frames per second or more on my fanless MacBook Air. Anything that costs a lot of work or frame rate and that players would not notice can be cut, so the street out the front is only scenery.
* I have given several rounds of feedback on the AI's story drafts. For example, I pointed out that at least half the players will have played the original game, so the story need not hide who the main character is. I also asked that players who only want to wander around for five minutes be looked after too.

## Where it is up to

* The whole house is built and lit: the kitchen, entry hall, living and dining room, laundry, the upstairs rooms, the back porch and the backyard.
* The ground floor is furnished and cluttered. The upstairs rooms are still mostly unfurnished.
* You can walk around, open doors and the fridge, switch on the kitchen light, pick up rubbish and wash the dishes.
* You can switch between two kinds of camera. One cuts between preset angles from area to area, like the original game. The other follows behind you.

## What comes next

* Rework parts of the entry hall, dining area and kitchen to match the original more closely.
* Furnish the upstairs rooms.
* Make the android character to replace the grey placeholder figure.
* Add the story, the remaining chores, animation and sound.

## More pictures

![The living room, lit by a table lamp](images/01_living_room.jpg)

*The living room, lit by a table lamp.*

![The dining area](images/02_dining_area.jpg)

*The dining area, with the stairs on the left and the kitchen through the arch.*

![Looking from the kitchen into the entry hall](images/03_kitchen_to_hall.jpg)

*Looking from the kitchen through the arch into the entry hall.*

![The entry hall and the staircase](images/04_entry_hall.jpg)

*The entry hall and the staircase.*

![An upstairs bedroom](images/05_upstairs_bedroom.jpg)

*An upstairs bedroom.*

![Washing up in an earlier build, with the grey placeholder figure](images/06_washing_up_placeholder.jpg)

*Washing up in an earlier build, with the grey placeholder figure.*

## Credits

* Textures: [Poly Haven](https://polyhaven.com/) and [ambientCG](https://ambientcg.com/), both CC0.
* Interface font: Instrument Sans (SIL Open Font License).
* Placeholder figure: Y Bot from [Mixamo](https://www.mixamo.com/).
