<details name="lang">
<summary><kbd>中文</kbd></summary>

# 《底特律：变人》Kara 和 Todd 的房子浏览器复刻

这是游戏中“新家”一章里那栋房子的非官方同人复刻，作为个人项目制作，没有任何商业目的。它不包含游戏中的任何素材，与索尼互动娱乐、Quantic Dream 均无关联。如果权利人提出要求，我会把它撤下。

**状态：制作中。** 本仓库只有截图，源代码未公开。

![在浏览器里走过厨房、门厅、用餐区和客厅，画面中是灰色的占位人物](images/00_walkthrough.gif)

*在浏览器里走过一楼，画面中是灰色的占位人物。*

## 这是什么

这是整栋房子的 3D 模型，可以在网页浏览器里走动。你将以第三人称操控一个为本项目设计的新仿生人，由它顶替 Kara 的位置来做家务。这个角色做出来之前，先由一个灰色的占位人物顶上。

## 我是怎么用 AI 来做的

所有代码都由 Claude Code 编写，包括在 Blender 里搭建房子的 Python 脚本，和让房子在浏览器里运行的 three.js 代码。我负责决定游戏要做成什么样，评判做出来的结果，并在做法行不通的时候换路。

* 之前的几版房子是用浏览器代码搭的。有一晚 AI 跑了七个小时，做出来的东西跟前一晚只跑一个小时的是一个水平。我追问它为什么不用 Blender，让它先在 Blender 里重做厨房的一个角落当小试验，交给另一个 AI 来评判。结果 Blender 明显胜出，我就让 AI 把整栋房子改用 Blender 重做。
* 我注意到客厅里茶几和电视之间的走道比原版游戏窄了很多，而 AI 自己的检查一直没有发现。之后我要求 AI 每次和原版对比都要量五样东西：格局、陈设、材质、光线和镜头构图。AI 照这条规矩把每个房间重新量了一遍，重新调整了整栋房子的格局。
* 仿生人的设定图是我用 AI 生图工具试了很多次才做出来的，从发型到衣服都是我挑的。AI 做的第一版头部花了六个小时，结果仍然很差，眼睛我只给 1 分（满分 10 分），于是我决定头部改用 Epic 的 MetaHuman 重做。
* 范围和底线是我定的。游戏做整整一章，包括二楼和后院，在我那台没有风扇的 MacBook Air 上要跑到每秒 30 帧以上。费功夫、拖帧率、玩家又感受不到的东西都可以砍掉，所以门前的街道只做成布景。
* AI 写的剧情草稿，我已经提了好几轮意见。比如我指出至少一半玩家玩过原作，所以不用把主角的身份藏得太深。我还要求照顾只想随便逛五分钟的玩家。

## 目前进度

* 整栋房子已经建好，光照也已做好，包括厨房、门厅、客厅和餐厅、洗衣房、楼上的房间、后门廊和后院。
* 一楼已经摆好家具，还堆放了杂物。楼上的房间大部分还没有家具。
* 可以走动、开门、开冰箱、开厨房的灯、捡垃圾、洗碗。
* 可以在两种镜头之间切换。一种和原版游戏一样，随着你从一个区域走到另一个区域，在预设的角度之间切换。另一种跟在你身后。

## 接下来

* 重做门厅、用餐区和厨房的一部分，让它们更贴近原版。
* 给楼上的房间布置家具。
* 制作仿生人角色，取代灰色的占位人物。
* 加入剧情、其余的家务、动画和声音。

## 更多图片

![由台灯照亮的客厅](images/01_living_room.jpg)

*由台灯照亮的客厅。*

![用餐区](images/02_dining_area.jpg)

*用餐区，左边是楼梯，穿过拱门是厨房。*

![从厨房望向门厅](images/03_kitchen_to_hall.jpg)

*从厨房穿过拱门望向门厅。*

![门厅和楼梯](images/04_entry_hall.jpg)

*门厅和楼梯。*

![楼上的一间卧室](images/05_upstairs_bedroom.jpg)

*楼上的一间卧室。*

![早期版本里洗碗的场景，画面中是灰色的占位人物](images/06_washing_up_placeholder.jpg)

*早期版本里的洗碗场景，画面中是灰色的占位人物。*

## 致谢

* 贴图：[Poly Haven](https://polyhaven.com/)和[ambientCG](https://ambientcg.com/)，均为 CC0。
* 界面字体：Instrument Sans（SIL Open Font License）。
* 占位人物：来自[Mixamo](https://www.mixamo.com/)的 Y Bot。

</details>

<details name="lang" open>
<summary><kbd>English</kbd></summary>

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

</details>
