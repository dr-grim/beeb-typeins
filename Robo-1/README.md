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

## Overview

This game was written very early when learnig how to code BBC BASIC, so it's rather simple - but, not a GOTO in sight!

The graphic were before I knew about assembler and sprites, so multiple custom characters defined - as they are single colour, multiple passes were required for Robo-1. I ran out of steam for the ghost and money...

The collision detection is rudimentary - check colour of pixel to top right of Robo-1; if yellow - congratulations! Collect the money. Note that yellow is only used (outside Robo-1) for the money bags...