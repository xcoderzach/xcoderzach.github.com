---
layout: post
title: Flow Control Library
published: false
---

  It seems everyone has an opinion on how to do flow control in node.js. 
I thought I'd join in on the fun, so I wrote _insert name here_.

  It's heavily influenced by Tame.js which is an awesome project.  This
is just a slightly more verbose functional version of that, intended for
use with coffeescript.

First, some code:
```coffeescript

await (defer) -> 
  getCurrentUserFromDatabase defer "currentUser"
  possibleTagsForPosts defer "tags"
, ({currentUser, tags}) ->
  getPostsByAuthor currentUser.id, defer "posts"
  sendListOfTagsToUser currentUser.id, tags, defer()
, ({posts, currentUser}) ->
  for i in [[0..10]
    getTagsFromUser defer "tags[]"

```


