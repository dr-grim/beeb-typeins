# Robo-1

Publication | Detail
-|-
Published | [Computer & Video Games](https://archive.org/details/Computer_Video_Games_Issue_037_1984-11_EMAP_Publishing_GB)
Date | November 1984
Page | 184
Author | Ian Grimstead

## Notes

Game line numbers stripped to enable [jsbeeb](https://github.com/mattgodbolt/jsbeeb) to autorun - you'll need to:
```
AUTO
*EXEC Robo-1
```
...to enter it manually.

The code needs to load from cassette at `PAGE=&0E00`, otherwise `LOMEM` sneaks above `&3000` and `MODE 2` is no longer available. I've struggled to get `jsbeeb` to go straight to `*TAPE` with a lower `PAGE` value, so lazy workaround for `jsbeeb` is to get it to emulate a BBC Master... argument in url is `&model=Master`.

## Overview

This game was written very early when learnig how to code BBC BASIC, so it's rather simple - managed to use `PROC` rather than `GOSUB` but there are still some `GOTO`s in there...

The graphic were before I knew about assembler and sprites, so multiple custom characters defined - as they are single colour, multiple passes were required for Robo-1. I ran out of steam for the ghost and the money.

Sound effects were as complex! A rather clunky 2001 extract to start with, and a beep to let you know Robo-1 has moved... and let you know when you're dead.

Strangely enough, when rooting around I found an earlier version of the code (check the history of Robo-1.txt); I thought `jsbeeb` had gone loopy - no, it was me. The older version didn't have audio or a countdown timer ("energy bar")...

The collision detection is rudimentary - check colour of pixel to top right of Robo-1; if yellow - congratulations! Collect the money. Note that yellow is only used (outside Robo-1) for the money bags...