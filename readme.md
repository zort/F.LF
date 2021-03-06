# F.LF - the open source LF2
[F.LF Main Project Page](http://tyt2y3.github.io/LFrelease/)
F.LF attempts a clean room implementation of the famous fighter game [LF2](http://lf2.net). The F stands for [Project F](http://project--f.blogspot.hk).

### Motivation

LF2 has received significant recognition and popularity since its initial release. Being the most sophisticated fighter game ever built, LF2 is also extremely customizable with its data file architecture. Over the years, numerous modifications have been made, ranged from spriting, data changing to exe editing. A vast amount of related work, including comics, animations and novels, have been created by thousands of people from all over the world, creating a strong and truly amazing community.

It is very limiting of what we can do with a compiled executable even with techniques like exe editing. But development of LF2 has been dormant for some years while the author has no plan to open source it. In order to move forward, the community has to own a code base and have right and ability to develop on it. Let us take this first step to the continuity of LF2.

### Philosophy

F.LF attempts to re-create LF2 in a web browser, and be an open source clean room implementation. F.LF respects original LF2 in every detail, that data file compatibilty and program behavior will be regarded carefully. F.LF will leverage web technologies as much as it can to make games native to browsers.

I believe the web, open source and fine software will enable anyone, from novices to experts, to create great interactive contents and bring them to any other one.

### Architecture
The open LF2 project is divided into three repositories, [F.core](https://github.com/tyt2y3/F.core), [F.LF](https://github.com/tyt2y3/F.LF) and [LFrelease](https://github.com/tyt2y3/LFrelease). F.LF is the game engine which implements ___the LF2 standard___ and provides gaming functionalities. F.core provides the engine components to build a HTML5 game. LFrelease contains material (sprites,data,sound,etc) converted from original LF2. Such division is to ensure that F.LF is 100% original work containing no third party copyrighted material.

### Compatibility
F.LF thrives for 99% compatibility with LF2.

- data
	- F.LF provide a [tool](http://tyt2y3.github.com/LFrelease/tools/data_file_converter.html) to convert xml-like LF2 data files into JSON.
- sprite
	- LF2 sprite images are in 24bit bmp and must be converted to 24bit png with defined transparent index (or 32bit png with transparency). in addition, F.LF requires XXX.png to be mirrored into XXX_mirror.png.
- sound
	- LF2 sounds are in wav and must be converted to ogg and mp3 for use with HTML5 audio.
- in general, materials should be compressed and converted to a format suitable for distribution and consumption on the web.

### Development
F.LF is still in mid-stage [development](http://tyt2y3.github.com/LFrelease/docs/develop.html). For details read the [documentation](http://tyt2y3.github.com/LFrelease/docs/index.html). try the [latest demo](http://tyt2y3.github.com/LFrelease/demo/demo3.html).

#### Call for contributors
F.LF has been a personal project for one year. Much of the foundational work has been done. May I now call for any one who love and know LF2 to involve in this project as programmer or tester to accelerate development and bring F.LF to production quality.

#### Install
The three repositories must be named and placed as below:
```
 F
 |---F.core
 |---LF
 |---LFrelease
```

### Project F
<img src="http://2.bp.blogspot.com/-k-My1B-YlaU/T8JUBAYpu9I/AAAAAAAAACI/OnCvkzFF5jw/s1600/logo_l1_s.png" height="80"/>
F.LF is an effort of [Project F](http://project--f.blogspot.com).

### License
Generally have complete freedom except commercial use. For exact terms see [license](http://project--f.blogspot.hk/2012/05/license.html).
