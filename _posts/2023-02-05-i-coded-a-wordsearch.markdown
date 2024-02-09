---
layout: post
title:  "I Coded... A Wordsearch"
date:   2023-02-05 21:00:00 +0100
categories: I Coded
---
I coded a wordsearch maker.

![Command line wordsearch](/assets/images/posts/wordsearch-console.png)

I'm currently working on an activity book for my son with a bunch of different puzzles in it. One of the types of puzzles is a wordsearch and I figured it be a nice little weekend project to create a wordsearch maker in Go. It both prints to console for ease of copy and paste as well as create a printable PNG laid out, for ease of creating one off page puzzles for him.

A lot of acitivity books for his age keep wordsearches simple, lower case and words that only go down or from left to right. No backwards and no diagonals. I put a bunch of flags in to control all these elements partly for him but also for my youngest as she gets older.

It's been a while since I've dived in to GO and it was mainly a success, however originally I was aiming to produce a PDF, but the options were very limited and not fully rounded. Producing a PNG with freetype was the simplier option.

Just for speed I limited it to a single monospaced font, long term I'd like to go back and allow it to accept multiple fonts. I did this so I could implement font scaling and centering within the PNG without having to read in each glyph and work out it's size.

Check out the code on github: [https://github.com/Altrozero/go-wordsearch-maker](https://github.com/Altrozero/go-wordsearch-maker)

![Printable wordsearch page](/assets/images/posts/wordsearch.png)